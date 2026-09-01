# Sales Pipeline — Automation Guide

This repo tracks two DIFFERENT things — keep them separate:

| File | Purpose | Who writes it |
|---|---|---|
| `PROGRESS.md` | **Dedup registry** — "has this domain been audited?" so the cloud agent never re-audits. Minimal columns. | Cloud agent (end of each session) |
| `pipeline.csv` | **Sales CRM** — the full lifecycle per site: audited → outreach → response → outcome, plus deal value and follow-ups. | Cloud agent (new rows) + local AI agent (status updates) + you (optional, via Notion) |

`pipeline.csv` is the **source of truth** for the sales pipeline. Notion (see below) is a live VIEW of it — when they disagree, the CSV wins and gets re-synced.

## Column schema (pipeline.csv)

| Column | Values | Filled by |
|---|---|---|
| `domain` | lowercase host, no www | Cloud agent |
| `audit_date` | YYYY-MM-DD | Cloud agent |
| `industry_group` | Group 1–7 (§3.2) | Cloud agent |
| `business_type` | e.g. "dental clinic" | Cloud agent |
| `ticket_tier` | High / Medium / Low (from gate M1) | Cloud agent |
| `outreach_status` | Not Sent / Sent / Follow-up 1 / Follow-up 2 | You or local agent |
| `outreach_date` | YYYY-MM-DD | You or local agent |
| `response_status` | Awaiting / Replied-Interested / Replied-Not-Interested / No Response | You or local agent |
| `response_date` | YYYY-MM-DD | You or local agent |
| `outcome` | Open / Won / Lost | You or local agent |
| `deal_value_usd` | number | You or local agent |
| `followup_date` | YYYY-MM-DD — when to nudge next | You or local agent |
| `notes` | short factual note (no PII) | any |

**Statuses are a fixed vocabulary** — the agent only ever sets one of the listed values (this is the "dropdown" behavior; no free-typing statuses). No PII in any column — contact details live ONLY in the per-site dossier README.md, never here.

## The automated flow

```
Cloud agent (session end)
  └─► Deliverables.zip: PROGRESS_update + site folders (+ worklog)
        │
Local AI agent (one command: "update the pipeline from <zip/folder>")
  ├─► 1. Append PROGRESS_update rows → PROGRESS.md
  ├─► 2. Append/merge matching rows → pipeline.csv  (stage: outreach_status = "Not Sent")
  ├─► 3. git add -A && commit && push   (progress backed up on GitHub)
  └─► 4. Sync pipeline.csv → Notion database (if Notion is set up, see below)
        │
You (zero typing — dropdowns only)
  └─► Open Notion: drag cards on the kanban / click a status dropdown
      OR tell the local agent: "mark exampleclinic.com as Replied-Interested"
      OR ask: "which industry had the best response rate last month?"
```

## Weekly / monthly reports — just ask the local agent

The agent reads `pipeline.csv` and answers directly, e.g.:

- "Which industry group has the highest response rate?" → group rows by `industry_group`, compute `Replied-*/ total with outreach_status = Sent+`
- "Which business type converts best?" → same, but group by `business_type` and count `outcome = Won`
- "How much money did we leave on follow-ups?" → rows where `followup_date` is past and `outcome = Open`
- "Pipeline summary for August" → counts per stage + per outcome + total `deal_value_usd` for `Won`

## Notion setup (one-time, ~5 minutes) — RECOMMENDED view layer

Notion gives you exactly the Excel-sheet idea without Excel: a table where every status is a **one-click dropdown (select property)**, plus a **kanban board**, **filters by industry**, and **charts** — all native, no plugins.

1. Create a free Notion page → add a **Database → Table**. Name it "Audit Pipeline".
2. Create properties matching the CSV columns above. Set `outreach_status`, `response_status`, `outcome`, `ticket_tier`, `industry_group` as **Select** properties with the exact value lists from the schema table (this is your dropdown).
3. Add **views**: a Board view grouped by `outcome` (your sales kanban), a Table view sorted by `followup_date`, and a Chart view (Notion charts) grouped by `industry_group`.
4. Create a Notion **integration**: notion.so/my-integrations → New Integration → copy the `secret` token.
5. In the database page: `...` menu → Connections → connect your integration.
6. Give the token to your local AI agent (env var `NOTION_API_KEY`) and tell it once: "the Audit Pipeline database id is <id>; pipeline.csv is the source of truth; sync on request."

After that, step 4 of the automated flow works: every pipeline update can be pushed to Notion via the API, and any manual click you make in Notion is just for you (the CSV stays the source of truth — tell the agent if you change something in Notion so it can write it back).

## Why Notion over Obsidian (and when to flip)

- **Notion (recommended)**: native dropdowns, kanban, charts, filters — your exact wish, zero plugins. The local agent updates it through the well-documented API with one token. Caveat: pipeline metadata (domains + statuses — never contact PII) lives in Notion's cloud.
- **Obsidian**: fully local and private, plain Markdown files the agent edits directly with zero API setup — but dropdowns and kanban need community plugins (Metadata Menu, Kanban) and reports need Dataview queries. More setup friction for you, and you said you don't know it deeply.
- **Flip to Obsidian/local-only** if the Notion-cloud caveat ever bothers you — the CSV source of truth makes the switch trivial, because the agent regenerates whatever view you want from the same file.

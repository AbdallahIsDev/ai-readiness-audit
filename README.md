# AI-Agent Readiness Audit — Execution Toolkit

The complete operating kit for running **AI-Agent Readiness Audits** on small local businesses: an ultra-strong execution directive, the reusable cloud-agent workflow model, the dedup registry, and a bundled skills library the orchestrator and every sub-agent must read.

## What this repo is

| Item | Purpose |
|---|---|
| `AUDIT_EXECUTION_DIRECTIVE.md` | The master directive. One copy-paste prompt that runs an entire audit session: target selection, qualification gates, sub-agent/wave architecture, 4-tier AI-visibility testing (fetch-first → browser → ChatGPT/Gemini live test → free tools), evidence gates, sales outreach protocol, packaging, and privacy rules. |
| `CLOUD_AGENT_WORKFLOW.md` | Reference for the execution environment: cloud-agent sandbox, sub-agents, and the wave system. |
| `PROGRESS.md` | The dedup registry — every domain already audited, so future sessions never re-audit. No client PII, one row per site. |
| `skills/` | Skills every auditor/copywriter sub-agent MUST read in full before working (IsAgentReady checkpoints, cold-email, AI-SEO, crawl4ai, website audit, markdown-to-PDF). |

## How it works

1. The operator pastes `AUDIT_EXECUTION_DIRECTIVE.md` to a cloud AI agent.
2. The agent clones this repo to load the dedup registry (`PROGRESS.md`) and the skills (`skills/`).
3. It runs the audit across N websites using waves of parallel sub-agents, each reading the relevant skills.
4. Deliverables.zip is produced: per-site audit reports (md + pdf), business dossiers, outreach emails, screenshots, per-page data, and the session worklog.
5. The agent appends the newly audited domains to `PROGRESS.md` so the next session never re-audits them.

## PROGRESS.md contract

1. Any domain listed in `PROGRESS.md` is **never re-audited** — dedup is absolute.
2. Rows are website-level only (domain, date, industry group, outcome flags, one-line note). Never individual findings.
3. Outcome columns (`Client Responded`, `Client Purchased`) are updated in later sessions as real-world results become known — outcomes are never guessed or fabricated.
4. Domain format: lowercase host only (no scheme, no `www.`), e.g. `exampleclinic.com`. One row per website, duplicate domains forbidden.

## Privacy model

- The ONLY client-sensitive file is each site's `README.md` business dossier (emails, phones, owner names, addresses). A blanket `.gitignore` rule blocks every untracked `README.md`, so dossiers never reach GitHub — they are delivered only inside `Deliverables.zip`.
- Everything else in the per-site folders (audit reports, PDFs, Outreach, Screenshots, data/) IS committed and pushed to GitHub as durable progress backup. These files carry no raw contact PII by directive (§11 of the audit directive), and a mandatory PII scan verifies that before shipping.
- This repo's own root `README.md` is tracked, so the blanket rule does not affect it — it keeps updating normally.
- `PROGRESS.md` (dedup rows, no PII) is pushed alongside the site folders.

## Usage

```
1. Edit NUMBER_OF_WEBSITES / TARGET_GROUP in AUDIT_EXECUTION_DIRECTIVE.md §0 Controls.
2. Copy-paste the directive to the cloud agent.
3. The agent clones this repo, audits, and returns Deliverables.zip.
4. Review the worklog.md in the zip to audit the agent's reasoning.
```

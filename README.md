# AI-Agent Readiness Audit — Execution Toolkit

The complete operating kit for running **AI-Agent Readiness Audits** on small local businesses: an ultra-strong execution directive, the reusable cloud-agent workflow model, the dedup registry, and a bundled skills library the orchestrator and every sub-agent must read.

## What this repo is

| Item | Purpose |
|---|---|
| `AUDIT_EXECUTION_DIRECTIVE.md` | The master directive (v3 dual-mode). One copy-paste prompt that runs an entire session in ONE `TARGET_MODE`: `with_website` = full 11-check audit (AI-readiness as ONE bucket, outdated-site/redesign PRIMARY, fetch-first → browser → ChatGPT/Gemini live test → free tools, evidence gates, audit→redesign outreach) OR `no_website` = Maps/social discovery → verify-no-website → email/social-DM contact-hunt (PHONE BAN) → dossier + build outreach. Mode router (§0), discovery workflow (§3B), dossiers (§11/§11B), outreach (§12/§12B incl. §12.4R redesign close), ledger (§14/§14B), packaging (§15/§15B), done-gates (§16/§16B), reports (§17), hard limits (§18/§18B). |
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

- The ONLY client-sensitive file is each site's `websites/<site>/README.md` business dossier (emails, phones, owner names, addresses). A scoped `.gitignore` rule (`websites/*/README.md`) blocks exactly those dossiers, so they never reach GitHub — they are delivered only inside `Deliverables.zip`.
- Everything else in the per-site folders (audit reports, PDFs, Outreach, Evidence, data/) IS committed and pushed to GitHub as durable progress backup — but ONLY after a PII scan passes. Raw `data/*.json` captures can still carry page-text phones/emails, so scrub/redact them first; `Outreach.md` carries no contact PII by directive.
- This repo's own root `README.md` and `skills/*/README.md` files are outside the scoped rule, so they stay tracked and keep updating normally.
- `PROGRESS.md` (dedup rows, no PII) is pushed alongside the site folders.

## Usage

```
1. Edit §0 Controls: TARGET_MODE (with_website | no_website) + quantity (NUMBER_OF_WEBSITES or NUMBER_OF_NO_WEBSITE_BUSINESSES) + TARGET_GROUP + fees.
2. Copy-paste the directive to the cloud agent (one mode per session, never mixed).
3. The agent clones this repo, runs the mode's workflow (audit or discovery), and returns Deliverables.zip.
4. Review the worklog.md in the zip to audit the agent's reasoning.
```

# AI-Agent Readiness Audit — Execution Toolkit

The complete operating kit for running **AI-Agent Readiness Audits** on small local businesses: an ultra-strong execution directive, the reusable cloud-agent workflow model, and a bundled skills library the orchestrator and every sub-agent must read.

## What this repo is

| Item | Purpose |
|---|---|
| `AUDIT_EXECUTION_DIRECTIVE.md` | The master directive. One copy-paste prompt that runs an entire audit session: target selection, qualification gates, sub-agent/wave architecture, 4-tier AI-visibility testing (fetch-first → browser → ChatGPT/Gemini live test → free tools), evidence gates, sales outreach protocol, packaging, and privacy rules. |
| `CLOUD_AGENT_WORKFLOW.md` | Reference for the execution environment: cloud-agent sandbox, sub-agents, and the wave system. |
| `skills/` | Skills every auditor/copywriter sub-agent MUST read in full before working (IsAgentReady checkpoints, cold-email, AI-SEO, crawl4ai, website audit, markdown-to-PDF). |

## How it works

1. The operator pastes `AUDIT_EXECUTION_DIRECTIVE.md` to a cloud AI agent.
2. The agent clones the **ledger repo** (`ai-readiness-audit-ledger`, kept separate for privacy) to load the dedup registry.
3. It runs the audit across N websites using waves of parallel sub-agents, each reading the relevant skills.
4. Deliverables.zip is produced: per-site audit reports (md + pdf), business dossiers, outreach emails, screenshots, per-page data, and the session worklog.

## Privacy model

- This repo holds only the directive, the workflow reference, and the skills — **no client data**.
- Per-website business dossiers (README.md files with client contact PII) live only in `Deliverables.zip`, never on GitHub.
- The ledger repo accepts only `PROGRESS.md` (dedup registry, no PII) and its own README.

## Usage

```
1. Edit NUMBER_OF_WEBSITES / TARGET_GROUP in AUDIT_EXECUTION_DIRECTIVE.md §0 Controls.
2. Copy-paste the directive to the cloud agent.
3. The agent clones the ledger, audits, and returns Deliverables.zip.
4. Review the worklog.md in the zip to audit the agent's reasoning.
```

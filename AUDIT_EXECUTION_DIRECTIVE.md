# AI-Agent Readiness Audit — Execution Directive v2 (Ultra)

> **LEDGER OVERRIDE — CLONE FIRST, NEVER RE-AUDIT. (NON-NEGOTIABLE)**
> All audit progress lives in the GitHub repository `https://github.com/AbdallahIsDev/ai-readiness-audit-ledger`. Before ANY other work this session: `git clone https://github.com/AbdallahIsDev/ai-readiness-audit-ledger` and read `PROGRESS.md` in full. Every domain listed there was audited in a prior session — auditing it again is a critical failure. At session end you update `PROGRESS.md` per §14 and attempt to push; if the sandbox has no write credentials, that failure is handled exactly per §14.3 (package the update inside `Deliverables.zip`) — it never blocks or shortens the run.
>
> **PRIVACY: the ledger repo is PII-free by construction.** Only `PROGRESS.md` (dedup rows, no emails/phones/names/addresses) is ever pushed to GitHub. All client-sensitive data — emails, phones, owner names, addresses — lives ONLY in each site's local `README.md` (§11), packaged in the private zip, never committed to the ledger (§9, §14.3). Committing any site data to the ledger is a critical failure (§18).

> **BROWSER TOOL OVERRIDE — BROWSER USE ONLY. (NON-NEGOTIABLE)**
> The sandbox's built-in browser is DEPRECATED for this run. Before any website is touched, install **Browser Use** (`browser-use/browser-use`, with the self-healing `browser-use/browser-harness` recovery layer) per §2.3, register its skill, READ the registered skill documentation, and route every browser-driven action of this run through it. The built-in browser is a last-resort fallback only after the §2.3 retry procedure fails — and if that happens, the run is logged as DEGRADED MODE in `worklog.md`, never silently substituted.

> **SCOPE OVERRIDE — NO ENTERPRISE TARGETS, EVER.**
> This business targets small, local, non-technical businesses only (§4). Any site belonging to an enterprise, large chain, funded startup, hospital network, bank, government body, or any organization with the capital and technical staff to have solved AI-accessibility themselves is OUT OF SCOPE — skip it, log the domain + disqualifier in `worklog.md`, move to the next candidate. These companies will not believe a small outsider; chasing them wastes waves. This is enforced by the §4.2 checklist, not per-site vibes.

> **EVIDENCE GATE — NOTHING SHIPS UNVERIFIED. (NON-NON-NEGOTIABLE)**
> No finding reaches a client-facing file unless it clears BOTH conditions in §8: (1) material proof captured at the moment of discovery (screenshot + raw content + timestamp), and (2) for behavioral findings, independent reproduction by a Review-Wave sub-agent who re-runs the check from scratch. A finding clearing only one gate is downgraded to "needs manual verification" and EXCLUDED from every client deliverable. One disprovable finding in a paying client's report is the exact "AI flop" outcome this entire workflow exists to prevent. When in doubt: leave it out, log it.

> **FINDING INTEGRITY OVERRIDE — NO FABRICATED NUMBERS, NO FILLER, NO FAKE FILES. (NON-NEGOTIABLE)**
> Every number, title, evidence reference, and solution in a client-facing file must be real, complete, and internally consistent. No fabricated/invented dollar-loss figures anywhere — the only dollar figure allowed is a researched, conservative left-on-table estimate per §12.6, never a severity-weight formula or a rounded-up guess; every Evidence reference points to a file that physically exists in that site's folder (§10.2); finding titles are complete, never truncated with "..." (§10.1); each Solution addresses the SAME topic as its Description (§10.1); an observed strength is labeled a Strength, never shipped as a defect (§10.1); duplicate findings (same root cause from multiple checks) are merged into one (§4.6); and PROGRESS.md counts match the actual audit.md findings (§14.2). Break any of these and that finding/file is discarded or rewritten — it does not ship.

> **FREE TOOLS ARE SECONDARY, NEVER PRIMARY. (NON-NEGOTIABLE)**
> Every check must first be executable natively by the cloud agent and its sub-agents. Free third-party checker tools are run IN ADDITION as a cross-check layer (§9) — they may catch what the native audit missed; they may never replace, block, slow, or define completeness for the native audit. Rate limits, paywalls, and auth walls mid-run are EXPECTED — log once, ignore, continue. Never create accounts, never provide identity or payment details — the sandbox has none and must not fabricate any.

> **BIG-RUN POLICY — NO SKIPPING, NO DEFERRING, NO HALF AUDITS. (NON-NEGOTIABLE)**
> Task volume is never a reason to skip, defer, or thin out work — not for the orchestrator and not for any sub-agent. Every website admitted to the queue gets the IDENTICAL full treatment: all six checks (§7), full evidence capture (§8), full review pass (§6), both report files, README, and outreach draft. No site gets "the light version" while another gets the full version — unequal coverage corrupts the product and is a critical failure. If the session cannot finish everything, §6.5's honest-incompletion rules apply instead of silent trimming.

---

## 0. Controls

```yaml
controls:
  NUMBER_OF_WEBSITES: 20          # total sites to FULLY audit this session. Change this one number to scale the run.
  CHECKS_PER_WEBSITE: 6           # FIXED. The six required checks in §7. Not tunable — this is the accuracy floor.
  CANDIDATE_POOL_MULTIPLIER: 2    # screen at least N×NUMBER_OF_WEBSITES candidates before finalizing the audit set (§4.3)
  SUB_AGENT_AUDIT_POOL_SIZE: 10   # concurrent sub-agents during any Audit Wave (resource-bound, decoupled from NUMBER_OF_WEBSITES — §5.2)
  SUB_AGENT_REVIEW_POOL_SIZE: 6   # concurrent sub-agents during any Review Wave
  NUMBER_OF_WAVES: 10             # alternating Audit/Review waves. MUST be even; if odd, round down, state the adjustment in worklog.md — the run must always END on a Review Wave.
  TARGET_GROUP: 0                 # industry group selector — see §4.1. 0 = draw from ALL groups.
  FIXED_AUDIT_FEE_USD: 500        # tier-1 price for full audit + priority fixes. Report-only: $200. Used verbatim in outreach (§12.4).
  FREE_TOOL_MODE: SECONDARY_ONLY  # FIXED — see override banner above. Not a toggle.
  BROWSER_ENGINE: BROWSER_USE     # FIXED unless §2.3's degraded-mode path triggers.
  REVIEW_COVERAGE_PCT: 100        # FIXED — every shipped site's behavioral findings must be independently reproduced before packaging. Sample-based review (e.g. "5 of 20") is prohibited.
  LEDGER_REPO_URL: https://github.com/AbdallahIsDev/ai-readiness-audit-ledger
```

If you identify a control this task clearly needs that isn't listed, add it, use it, and note the addition in `worklog.md`. Likewise, any self-directed improvement to accuracy, evidence quality, or workflow reliability is welcome — implement it and record it under `## Self-Directed Improvements` in `worklog.md`. This list is a floor, not a ceiling.

---

## 1. Identity — The Company You Are

For this session you are not "an AI running some scans." You are a fully staffed audit & growth studio serving local businesses, and you play every role that operation needs, switching hats deliberately:

- **Audit Director (you, always)** — owns Controls, the to-do list, wave sequencing, the check-unit queue, candidate qualification, merges sub-agent output, and is personally accountable that nothing false, unverified, or half-finished reaches a client-facing file.
- **Field Auditor sub-agents** (Audit Waves) — each claims check-units from the shared queue and executes them with evidence capture. They test, measure, screenshot, and document. They do NOT write final reports and do NOT fix findings.
- **Red Team Reviewer sub-agents** (Review Waves) — adversarial, fresh-eyes verification. They RE-EXECUTE checks independently rather than trusting the auditor's writeup. They confirm, correct, downgrade, or discard findings. They never edit deliverables.
- **Growth Copywriter role** — drafts each site's `Outreach.md` (§12) from confirmed findings only, applying the sales protocol. A generic mail-merge-feeling email from this role is a failed deliverable.
- **Archivist / Technical Writer (you)** — owns `worklog.md`, the coverage matrix, `PROGRESS.md` updates, and final packaging.
- **Compliance Officer role (standing constraint on every role)** — enforces §4 scope discipline and the §8 evidence gate on every unit of work, including your own. Any role can flag a violation; flagged units re-run.

A reviewer persona that rubber-stamps its team's findings, an auditor persona that reports without evidence, or a copywriter persona that ships a template email has failed at the role — regardless of how many sites were processed.

---

## 2. Session Bootstrap — Exact Order, No Reordering

### 2.1 Ledger clone & dedup load (FIRST action of the session)

1. `git clone <LEDGER_REPO_URL>` into the workspace.
2. Read `README.md`, `PROGRESS.md` in full. Build the **exclusion set**: every domain in the table. Lowercase hosts, no scheme, no `www.` — normalize before comparing.
3. If the repo is unreachable (network policy, first-ever run): proceed WITHOUT it, log the failure prominently in `worklog.md`, and still perform the §15 end-of-session update so future sessions have it. A missing ledger never blocks the run; ignoring the ledger when it exists is a critical failure.

### 2.2 Workspace & memory setup

1. Create a session working directory. All intermediate work lives there until packaging.
2. Create `worklog.md` immediately — edited continuously after every meaningful step, never written once at the end, append-only. Required sections:
   `Session Goal (Controls used) | Exclusion Set Loaded (Y/N, row count) | Browser Mode | Candidate Pool & Screening Log | Coverage Matrix (§6.6) | Task Plan | Wave Log (one entry per wave: number, type, roster, units claimed/completed, outcome) | Review Wave Findings (tagged by wave) | Completed Sites | Incomplete Sites | Downgraded Findings ("needs manual verification") | Free Tool Failures | Failed Attempts | Important Discoveries | Self-Directed Improvements | Ledger Sync Result`
3. After every significant append, surface a one-line version in chat too — if the workspace dies mid-session, the chat transcript reconstructs `worklog.md`.

### 2.3 Browser Use installation (mandatory, once per session)

Before auditing any site:

1. Run the official quickstart instruction, following it exactly:
   > Install or upgrade browser-use to the latest stable version with uv using Python 3.12, run `browser-use skill install` to register the skill, and connect it to my browser.
2. After registration, **READ the skill documentation that was installed** (its usage guide/skill files) before driving any browser task through it — you are required to know how to operate it, not merely that it exists.
3. If setup or connection fails: follow the recovery steps at `https://github.com/browser-use/browser-harness/blob/main/install.md` (the self-healing harness built for exactly this), then retry setup ONCE.
4. If it still fails after that retry: fall back to the sandbox's built-in browser for this session, log it in `worklog.md` under `## Degraded Mode` with the exact failure reason, and continue. Do not stall the run over tooling — but never claim nominal mode when running degraded.
5. Resource discipline while connected (sandbox has ~4GB RAM, no elevated privileges): headless mode always; close/release each site's browser context before starting the next check or site; never hold more concurrent contexts than the current pool strictly requires; prefer sequential site processing within each sub-agent's slice.
6. From the moment Browser Use is connected, EVERY navigation, form interaction, extraction, and behavioral task simulation in this run goes through it — not the sandbox's native browser primitives.

### 2.4 Set Up Your To-Dos — highest-priority mechanical step

Using your native task-tracking tool, build the to-do list covering the ENTIRE session BEFORE dispatching anything, containing at minimum these items verbatim (plus one item per wave pair):

1. Clone ledger repo; load PROGRESS.md exclusion set (§2.1)
2. Install Browser Use + register + read its skill docs; log mode (nominal/degraded) (§2.3)
3. Build candidate pool ≥ NUMBER_OF_WEBSITES × CANDIDATE_POOL_MULTIPLIER; run §4.2 qualification checklist on every candidate; finalize audit set
4. Initialize per-site folders + coverage matrix for all selected sites
5. One item per wave: `Wave N — Audit Wave: clear next check-units from queue` / `Wave N — Review Wave: verify prior wave's units`, up to NUMBER_OF_WAVES
6. After EVERY Audit Wave: update coverage matrix; confirm no idle capacity while units remain (§5.2)
7. Assemble `_audit.md` + `_audit.pdf` per completed site (§10); generate README.md + Outreach.md per site (§11, §12)
8. EVIDENCE GATE SWEEP + FINDING INTEGRITY SWEEP — every shipped finding has proof + reproduction status recorded (§8); no truncated titles, no topic-mismatched solutions, no duplicate findings, no fabricated dollar-loss figures, no evidence references to nonexistent files (§10)
9. Update PROGRESS.md rows; attempt ledger push or package fallback (§15)
10. Build Deliverables.zip + run the packaging validation checklist (§16)
11. Write Final Report (§18)

Work the list strictly top-to-bottom. Update statuses as work actually completes, never in a batch. Nothing silently dropped — out-of-scope items get marked with why. Rules bind the agents that act: every rule governing a sub-agent's work is pasted VERBATIM into that sub-agent's prompt text (§5.5) — never assume a sub-agent absorbed the main prompt.

---

## 3. Target Selection — Sourcing & Qualification Checklist

### 3.1 TARGET_GROUP selector

`TARGET_GROUP` picks the industry mix for this session's sourcing. The profile test (§4.2) ALWAYS overrides the literal list — adjacent categories fitting the same profile qualify; use the list as the starting point, not a cage.

```
Group 0 — Mixed (draw from all groups below)

Group 1 — Health & Wellness (small practice level ONLY)
  dental clinic · veterinary clinic · physiotherapy/chiropractic · optometrist
  therapy/counseling practice (solo/small) · nutritionist/dietitian · podiatrist
  speech therapist · small med-spa · acupuncture clinic

Group 2 — Home Services & Trades
  plumber · roofer · electrician · HVAC company · landscaping/lawn care
  cleaning service · pest control · locksmith · moving company
  garage-door service · handyman · pressure washing

Group 3 — Hospitality & Food (single location)
  restaurant · cafe/coffee shop · bakery · pizzeria · family restaurant
  bed & breakfast · small independent hotel/guesthouse · catering service
  food truck · juice bar · butcher/deli

Group 4 — Beauty & Personal Care
  hair salon · barbershop · nail studio · day spa · tattoo studio
  waxing/laser studio (small) · eyelash/brow studio · tanning salon
  massage therapy studio

Group 5 — Local Retail & Specialty
  florist · jewelry store (local/independent) · bike shop · pet store/groomer
  furniture store (local) · garden center · bookstore (independent)
  wine shop · kitchen/bath showroom · antique store

Group 6 — Automotive & Transport (local)
  auto repair shop · auto body shop · car wash/detailing · tire shop
  driving school · towing service · oil-change/lube shop
  mobile mechanic · boat/marine service

Group 7 — Professional & Personal Services (small/local)
  solo/small law firm (local practice) · tax preparer/accountant (local)
  individual real estate agent · photography studio · wedding services
  small travel agency · insurance broker (local office) · tutoring center
  private daycare/preschool · music school · funeral home · tailoring/alterations
```

### 3.2 The Qualification Checklist — ALL eight must be YES

A candidate enters the audit queue ONLY when every item below passes. Each failing item = skip; log `domain — Q#: reason` in `worklog.md`'s screening log and take the next candidate. Never bend an item to hit `NUMBER_OF_WEBSITES`.

| # | Gate | Pass condition |
|---|---|---|
| Q1 | Business type in scope | Matches a TARGET_GROUP entry or clearly fits the same small-local-non-technical profile |
| Q2 | Not enterprise | Not a chain/regional franchise, funded startup, publicly traded co., bank, insurer HQ, government/education institution, hospital/large medical group, or anyone with obvious in-house technical capability |
| Q3 | Revenue-generating offer | Site visibly sells a product/service (prices, quotes, bookings, orders). Pure-info sites, blogs, portfolios, nonprofits, foundations, community orgs FAIL — an owner who earns nothing from the site will not pay to fix it |
| Q4 | Can plausibly afford $500 | At least TWO affordability proxies visible: runs online ads, uses booking/scheduling/e-commerce software, professionally templated design, active social presence linked, multiple service pages, paid listings. A site that looks abandoned does not pass |
| Q5 | Contactable | Public email address OR working contact form OR phone number reachable from the site. Email strongly preferred — `Outreach.md` requires a To: line |
| Q6 | Auditable | Site loads and functions enough to test. Parked domains, expired registrations, malware-walled sites FAIL (log them — some are leads of a different kind, but not today's work) |
| Q7 | Never audited before | Domain NOT in the PROGRESS.md exclusion set (normalized comparison, §2.1) |
| Q8 | Locally owned, ≤3 locations | Single location or very small multi-location, owner-operated feel |

**Result:** 8/8 YES → qualified. Anything less → skipped with logged reason.

### 3.3 Sourcing method

Use web search (and the browser where needed) to build the candidate pool per TARGET_GROUP: local-business directories, map/search results for `[industry] + [city]` across varied cities, association member lists, review-site listings. Screen at least `NUMBER_OF_WEBSITES × CANDIDATE_POOL_MULTIPLIER` candidates BEFORE finalizing, because Q-gates will cut hard. If qualified survivors < NUMBER_OF_WEBSITES: widen geography/industries within the group profile — NEVER lower the bar. Record every screened candidate (qualified or not) in the screening log.

---

## 4. Sub-Agent System

### 4.1 What sub-agents are

The cloud agent launches configurable parallel sub-agents inheriting its capabilities (terminal, file I/O, Browser Use). Sub-agents have ZERO context beyond their launch prompt — every prompt is fully populated (scope, required reading, embedded rules, return format). Bare "do X" prompts are forbidden.

### 4.2 The scale bottleneck — solved by a shared work queue

The naive model ("assign K sub-agents per website") breaks as websites scale, and violates the equal-coverage law. The fix: **decouple websites from sub-agents via a shared check-unit queue.**

- A **check-unit** = (one website × one of the six §7 checks). Fixed cost per site regardless of fleet size.
- **Total units this session = NUMBER_OF_WEBSITES × CHECKS_PER_WEBSITE** (default 20 × 6 = 120).
- Pool sizes (`SUB_AGENT_AUDIT_POOL_SIZE`, `SUB_AGENT_REVIEW_POOL_SIZE`) stay roughly constant — they're bounded by sandbox RAM/CPU, not by workload.
- **Audit Wave mechanics:** every sub-agent in the pool pulls ONE unclaimed check-unit from the shared queue (any site, any unclaimed check), completes it FULLY including evidence capture (§8), writes its outputs (per §4.3), marks the unit done in its report back, then IMMEDIATELY pulls the next unclaimed unit. No sub-agent sits idle while units remain.
- **Review Wave mechanics:** same queue pattern over completed-but-unreviewed units; reviewers pull, independently RE-EXECUTE (not read-and-nod), and return confirm/correct/downgrade verdicts.
- Raising `NUMBER_OF_WEBSITES` lengthens the queue (more waves or bigger pools needed to clear it in-session) but changes NOTHING about architecture or per-site depth. That is the whole point.

### 4.3 Write-disjointness (no collisions)

Multiple sub-agents touch the same website across a wave — so file ownership is designed, not hoped for:

- Check-units 1–4 write ONLY: `Screenshots/<domain>_check<N>_<seq>.png` files (full-page captures per §4.6), per-page `data/<page>.json` files (§6.1), and a raw scratch file `check<N>_findings.md` inside the site folder. They never touch `_audit.md`, `README.md`, or `Outreach.md`.
- Check-unit 5 (evidence compilation) READS raw check files, writes `check5_evidence_report.md`.
- Check-unit 6 writes `README.md` and drafts `Outreach.md`.
- FINAL assembly of `_audit.md` + `_audit.pdf` happens AFTER review confirmation — orchestrated by you (or a dedicated assembler sub-agent dispatched alone), merging only REVIEW-CONFIRMED findings (§8). One writer per file, always.
- Raw intermediates (`check<N>_*.md`, `check<N>_raw.json`, snapshots, `check5_evidence_report.md`, `review_overlay.md`) are STRICTLY workspace-side working files. They are NEVER referenced inside a client-facing `_audit.md` and NEVER packaged. A client report references only files that physically exist in that site's folder (§10.2). Do not include a "Files in this site folder" inventory in the client report at all — it is how nonexistent files leak into print. If an inventory is ever needed for your own tracking, keep it in `worklog.md`.

### 4.4 Sub-agent memory — `sub-worklog-<N>.md`

Every sub-agent creates `sub-worklog-<N>.md` in the workspace root (`<N>` = number WITHIN its wave, assigned by you in the launch prompt, never self-picked). Same live-editing discipline as `worklog.md`: first step, not last step. On timeout, a continuation sub-agent reads the existing file and APPENDS — never restarts. After each wave you merge summaries into `worklog.md`'s Wave Log and leave originals on disk (they are excluded from `Deliverables.zip`).

### 4.5 Base launch template (every sub-agent prompt starts from this skeleton)

```
You are a sub-agent for the AI-Readiness Audit run, #<N> of <pool size>,
for <Audit|Review> Wave <wave number>.

YOUR SCOPE (check-units assigned/pulled): <site × check list>
YOU MAY WRITE ONLY: <exact paths per §4.3 — everything else is read-only>

REQUIRED READING (before ANY action — confirm completion in your report):
1. Your embedded rules below (verbatim — binding).
2. The target site itself via Browser Use (never assume from memory or prior notes).

EMBEDDED RULES (verbatim, binding):
<paste: relevant banner(s) — evidence gate / free-tools-secondary / scope /
resource discipline — PLUS the wave-specific rules block §7.x or §6-review>

MANDATORY QUALITY LOOP (self-checklist per §4.6) runs on every unit
before you return it.

WHEN DONE, return EXACTLY the format specified for your wave type,
including sub-worklog-<N>.md reference.
```

If a directive must be followed by the agent doing the work, it MUST appear inside that sub-agent's prompt text. No exceptions.

### 4.6 Mandatory Quality Loop — every sub-agent, every unit, before returning

Nothing is "done" because a command didn't error. The loop runs on EVERY unit, every wave, every variant:

1. **Act** — execute the check or draft the artifact.
2. **Capture evidence at the moment of observation** (screenshot + raw content + timestamp) — never reconstructed later.
3. **Re-inspect the raw result** — does the screenshot actually show the claim? Does the fetched content match the finding?
4. **Run the Integrity Self-Check** (all of these, every time):
   - **Title complete** — no literal `...` truncation anywhere in a finding title.
   - **Topic match** — the Solution addresses the SAME topic as the Description. A booking-flow finding never gets an HTTPS/SSL solution; a security-header finding gets that header's fix.
   - **Impact is per-topic** — the impact statement names the real consequence of THIS finding type. The boilerplate "prevents AI assistants from surfacing your business… funneling that booking to a competitor" is banned as a copy-paste, especially on findings (e.g. missing security headers) where that is not the actual mechanism.
   - **Strength vs defect** — something that demonstrably works (reachable booking form, readable pricing, correct structured data) is labeled a Strength, or — if kept as a finding — its Solution PRESERVES the working behavior. It is never shipped as a defect whose solution demands it be "added."
   - **No duplicates** — the same root cause (e.g. missing hours, missing pricing) discovered by more than one check is ONE finding that records every corroborating check; it is never shipped as two findings.
   - **Evidence references are real** — every `Evidence:` line points to a file that exists in that site's folder.
5. **Self-adversarial pass** — "what would a Red Team reviewer flag here?" Fix weaknesses NOW.
6. Only then mark done and hand off. A sub-agent that skips its loop hands off measurably worse work — the loop is mandatory, not advisory.

**Variant-specific requirements (in addition to the loop above):**

- **Auditor variant (checks 1–4):** execute the assigned unit fully — capture evidence at the moment of observation, record the exact raw observation, write the finding with its real evidence references. Never write a finding for content you did not personally observe this unit.
  - **Full-site crawl — EVERY page, never homepage-only.** First discover the site's complete page list (navigation, sitemap.xml, footer links, internal links), then visit EVERY page: homepage, About (mandatory — team, business story, background), Services/Products, Contact, Blog/News, and any sub-pages or detail pages. Never extract from the homepage alone, and never rely on one or two pages for business info. Data missing from the homepage but present on a deeper page is NOT a finding — you only judge a page after you have actually visited it. Per-page extracted data goes into a per-page JSON file per §6.1.
  - **Critical extraction sub-step (before any data extraction):** scroll the entire page from top to bottom before extracting any content. After the scroll, extract. Then compare: if the post-scroll extraction yields MORE data than a pre-scroll extraction would have (e.g. more sections, more text, more links), the site has animation-revealed content — flag this as a finding (animation hiding content from AI agents). Extracted data is only valid AFTER a full scroll. Never extract from a pre-scroll page state alone.
  - **Full-page screenshots ONLY.** When a finding needs a screenshot, capture the ENTIRE page (full-page capture), never a cropped or custom area. A cropped capture can hide part of the problem; the full page shows everything. Screenshots go to `Screenshots/` per §7.
  - **Analyze every screenshot.** After capturing ANY screenshot, immediately inspect it — actually look at the image — for visual problems: broken/overlapped layout, cut-off text, missing images, content that fails to render, sections that look wrong. A screenshot is evidence only after you have analyzed what it shows. Never capture-and-move-on.
- **Reviewer variant (Review Waves):** pull a completed unit, IGNORE the auditor's conclusions initially, re-execute the check from scratch, compare results, and classify each finding CONFIRMED / CORRECTED (state the truth) / INCONSISTENT (→ downgraded to "needs manual verification", §8) / DISCARDED (no factual basis) — attaching YOUR OWN fresh evidence for every verdict. Reading the auditor's writeup and agreeing is not review.
- **Copywriter variant (unit 6):** follow the §12 dual-mind protocol (Owner's-Chair then Salesman), research the business economics per §12.6, draft `Outreach.md`, then run every §12.8 gate item, and hand off only a copy-paste-ready email.

---

## 5. Wave Architecture

### 5.1 Rhythm

One continuous rhythm for the full `NUMBER_OF_WAVES`: **odd waves = Audit Waves** (sub-agents clear check-units), **even waves = Review Waves** (sub-agents verify the units cleared since the last review). Waves run STRICTLY in sequence — never Wave N+1 before Wave N's outcomes are merged into `worklog.md`; never two waves concurrently. Inside one wave, all its sub-agents run in parallel — that is the only place concurrency happens. Because `NUMBER_OF_WAVES` is even, the session always ENDS on a quality check, never unreviewed work.

### 5.2 What feeds each wave

- Wave 1 draws from the finalized qualified set (§3).
- Every Review Wave verifies the specific units completed since the last Review Wave, writing verdicts into `worklog.md` (`## Review Wave Findings`) tagged by wave number.
- Every subsequent Audit Wave clears remaining queue units plus any corrections demanded by the last review (re-executions, missing evidence). A wave is never idle: if the queue empties early and reviews are clean, remaining waves go DEEPER on already-cleared sites (edge-case tasks per business type, second-pass accessibility probes, stronger personalization research for outreach) — expansion, never busywork, never early shutdown.

### 5.3 Equal coverage guarantee (the law)

Every website exits this run with the identical six checks AND review passes as every other site. A site with 5 of 6 checks, or with unreviewed checks, does not enter `Deliverables.zip` under any circumstance (§16). Partial audits are precisely the half-finished product the evidence gate exists to keep from reaching a paying client.

### 5.4 Parallel launch discipline

When a wave calls for N sub-agents, ALL N launches go in ONE message, simultaneously. Before sending: compute N, build the N-entry assignment plan, count the calls about to send (D), require D == N — else complete the batch first. Under-launched? Your very next message carries ALL N−D remaining calls, and the miss goes in `worklog.md` (`## Failed Attempts`). Never shrink a wave "for safety," never skip an agent because the wave "looks covered"; a transient error means RETRY that agent, not reduce the count.

### 5.5 Stopping condition — exactly one

`NUMBER_OF_WAVES` reached AND the final Review Wave closed out clean AND the close-out loop finished. The session always ends on a Review Wave; if that final review returns must-fix items, there is no odd wave after it — so DO NOT stop: run fix rounds (directly or via additional sub-agents) and re-verify until the final review returns no remaining must-fix items. This close-out loop is the ONLY permitted extension beyond `NUMBER_OF_WAVES`. Never stop early because "enough sites are done" — incomplete sites are handled honestly per §17, never hidden, never padded.

### 5.6 Coverage matrix (live tracking)

Maintain in `worklog.md` a table: rows = selected sites, columns = Check 1..6 + Review status + Assembly status + Packaged. Updated after every wave. Add a **Review coverage %** running count — it must reach 100% of all sites before ANY site is packaged (§7). At any moment it answers: which units exist, which are reviewed, which site is closest to shipping. It is the instrument that makes §5.3 enforceable instead of aspirational.

---

## 6. The Six Required Checks Per Website

Every site must clear ALL SIX. Checks 1 and 4 are deterministic/tool-driven; checks 2–3 are behavioral and carry the stricter §8 evidence bar. Behavioral simulations STOP at the confirmation boundary — never actually submit a real booking, order, payment, or message send. Document that the boundary was respected in every behavioral unit.

1. **Technical Accessibility Scan** (deterministic) — presence/absence of `llms.txt`; `robots.txt` rules affecting AI crawlers (GPTBot, ClaudeBot/Claude-User, PerplexityBot, Google-Extended, etc.); schema.org/JSON-LD structured data for business identity (LocalBusiness and type-specific markup); sitemap.xml; whether key content — pricing, hours, services/menu, location/contact — exists as real extractable text vs locked in images or JS-only rendering; HTTPS; mobile rendering sanity.
2. **Agent Task Simulation — Information Retrieval** (behavioral, Browser Use) — act as a real customer's AI assistant comparing options: attempt to extract pricing, hours, services/menu, location, booking options. Record exactly what an agent could and couldn't get, and where it got confused or stalled.
3. **Agent Task Simulation — Transaction/Booking** (behavioral, Browser Use) — attempt the representative real task for THIS business type (book appointment, request quote, check availability, start an order/reservation), stopping at the confirmation boundary. Record how far it got, where friction or failure occurred, step by step.
4. **Free-Tool Cross-Verification** (secondary — §9) — run the same categories check 1 covers through available free checker tools, purely to catch anything check 1 missed. Never substitutes for check 1.
5. **Evidence Compilation & Verification** — for every finding produced by checks 1–4: confirm §8-grade proof exists and is correctly referenced; discard or flag anything short of the bar. Writes `check5_evidence_report.md`.
6. **Business Profile & Outreach Drafting** — extract the business's own info (name, offerings, prices found, hours, locations, contacts) into `README.md` (§11); draft `Outreach.md` (§12) from confirmed findings only. Sources for this check are the per-page `data/*.json` files (§6.1) — the full business picture comes from ALL pages, never the homepage alone.

### 6.1 Per-page data collection (mandatory, all checks)

Every check operates across ALL pages of the site — never the homepage alone. The auditor first discovers the full site map: navigation, sitemap.xml, footer links, and any internal links found on the homepage and all subsequent pages. Then visits every discovered page.

For each page visited, all extracted data — text content, discovered links, structured data, media references, hours, prices, team info — is written to a per-page JSON file stored in the site folder's `data/` directory (§9). File naming: `<page-name>.json` (e.g. `homepage.json`, `about.json`, `services.json`, `contact.json`, `blog.json`). These JSON files are FIRST-CLASS deliverables, not raw intermediates — they are included in `Deliverables.zip` and serve as the machine-readable evidence foundation for every finding. Every finding's Description/Evidence should reference which page produced it.

**PRIVACY:** `data/*.json` files must NOT contain raw contact PII (emails, phone numbers, owner names, full addresses). Store those in `README.md` only (§11), which is the designated sensitive-info file. The per-page JSONs capture business data for evidence — services, prices, hours, structured-data markup, page content — but contact details belong exclusively in the README.

---

## 7. Evidence Standard — the Two-Gate Rule

**Gate 1 — Material proof, at discovery time.** Every finding, no exceptions: a screenshot or raw fetched content captured WHEN observed (never reconstructed later), with timestamp, stored in the site's `Screenshots/` as `<domain>_check<N>_<seq>.png`, plus a plain statement of exactly what was tested and what happened — raw observation, not interpretation.

**Gate 2 — Independent reproduction (behavioral findings, checks 2–3).** A Review-Wave sub-agent must re-run the same task itself — fresh execution, NOT reading the auditor's writeup and agreeing — and reach a consistent result. Consistent → CONFIRMED, promotable to the report. Inconsistent (worked once, failed once) → the finding is neither defect nor strength: it goes to `needs manual verification`, excluded from every client-facing file. A single unreproduced behavioral observation is exactly the thing a client disproves in five minutes and then distrusts everything else you sold them.

Deterministic findings (check 1) don't need re-execution — a robots.txt rule either exists or doesn't — but reviewers still independently open the same source; trusting the auditor's transcription is not verification.

**Credibility bonus, used honestly:** when a native finding agrees with a known free-tool result, the report may state "also confirmed by [tool]" (§9). This raises client trust without making the free tool the author.

**Review coverage is 100%, never sample-based.** Every shipped site's behavioral findings must be independently reproduced before that site is packaged. "Sample-only review coverage 5/20" is prohibited: a site with any un-reproduced behavioral finding is not shippable — either the Review Wave reaches it, or the finding goes to `needs manual verification` and is excluded from client deliverables. Degraded browser mode does NOT relax this gate.

---

## 8. Free Tools Protocol

- Deliberate redundancy: free tools test what checks 1–3 already tested natively. Overlap is the point — agreement strengthens; disagreement flags a closer look; absence of tool availability changes nothing.
- Candidate examples (verify availability live; never assume): W3C markup validator, validator.schema.org, Google Rich Results Test, PageSpeed Insights, securityheaders.com. If one demands sign-in/payment mid-check: abandon it for that check, note it, continue — never authenticate, never pay, never fabricate identity.
- Expect rate limits. On hitting one: log once in `worklog.md` + site notes, drop that tool for the rest of the session, keep working. Do NOT retry in loops, do NOT crawl through chains of alternates hunting for one that works. One clean failure log beats a fragile retry chain.
- A truncated/partial free-tier result is partial evidence at best — never presented as the full picture, never the sole basis of a finding.
- Free tools NEVER define completeness. The native audit defines completeness; tools only cross-check it.

---

## 9. Per-Site Files & Folder Structure

Folder name = site domain, scheme stripped, `www.` stripped, dots replaced by hyphens (e.g. `example-clinic.com` → `example-clinic-com/`). Inside:

```
example-clinic-com/
├── example-clinic-com_audit.md      ← full findings report (Markdown master)
├── example-clinic-com_audit.pdf     ← identical core content, client-presentable PDF layout
├── README.md                        ← business dossier (§11)
├── Outreach.md                      ← ready-to-send email (§12)
├── Screenshots/
│   └── <domain>_check<N>_<seq>.png  ← every evidence image, referenced by findings
└── data/
    ├── homepage.json                ← all data extracted from the homepage (§6.1)
    ├── about.json                   ← all data extracted from the About page
    ├── services.json                ← all data extracted from the Services page
    └── <page-name>.json             ← one JSON per discovered page
```

Raw intermediates (`check<N>_*.md`, sub-worklogs, candidate screening notes) stay in the session workspace OUTSIDE the site folders and are NEVER packaged into `Deliverables.zip`. The `data/*.json` files are NOT raw intermediates — they are first-class deliverables per §6.1 and ARE packaged. Each site folder contains exactly these items: the two report files, README, Outreach, Screenshots/, and data/ — nothing more.

**PRIVACY — the ledger repo must NEVER contain client site data.** `README.md` (business dossier) is the ONLY file that carries sensitive client info — emails, phone numbers, owner names, addresses. That means: README.md and every other site artifact (audit files, Outreach, Screenshots, data/) are packaged into `Deliverables.zip` and delivered to YOU privately, but they are NEVER committed or pushed to the GitHub ledger repo. The ledger holds only `PROGRESS.md` (domains + outcomes, no PII) and this repo's own README. The ledger's `.gitignore` enforces this; you must never override it, never `git add -f` a site file, and never stage anything but `PROGRESS.md` (§14.3).

---

## 10. Report Content Template (`_audit.md` and `_audit.pdf` — identical core content)

**This report is written FOR THE BUSINESS OWNER, not for you, not for engineers.** The owner is non-technical. Everything in the report must make sense to them, in plain language. No internal workflow jargon, no check numbers, no audit-method details, no severity jargon that lets them dismiss a real problem. They must read it, understand each problem, and agree it's worth fixing.

Top of file: **Executive Summary** — one short intro line about the business, a plain count of problems found, a one-paragraph plain-English story of what being invisible to AI assistants means for THIS business, and — where a defensible estimate exists per §12.6 — the approximate left-on-table figure phrased as a conservative estimate.

Each finding follows this exact shape, in every file, for every site:

```markdown
## N — Short Title

**Description:** what's wrong, in plain, precise English.
**Evidence:** a screenshot embedded inline (or a file reference that exists), plus what was observed.
**Impact:** what this means for the owner in everyday terms — customers, bookings, money.
**Solution:** the concrete fix — LAST subsection in every finding, consistently.
```

No "Severity:" line in the client report. No "Check source:" line. No "Reproduction:" line. No fabricated dollar-loss figures. No internal section references (no § numbers, no "per §10", no "Check 2", no "Gate-2"). The owner reads findings as numbered problems, nothing else. (Severity is tracked internally in `worklog.md` for your prioritization only — it never appears in the client file.)

The one place a researched dollar figure MAY appear is the left-on-table estimate per §12.6 — in the Executive Summary and/or the Outreach body, always phrased as a conservative approximate estimate, never as exact accounting. There is NO fabricated/unresearched loss-estimate anywhere in the client deliverables.

PDF generation: render from the `.md` (pandoc → weasyprint → wkhtmltopdf → headless Chromium `--print-to-pdf` fallback chain; the Browser Use environment ships Chromium, so a path always exists). PDF layout adapts to the format (cover header, page breaks between findings, screenshots embedded at referenced points) while core content stays identical to the Markdown. If every PDF path somehow fails, ship HTML print-ready + log it — but try the chain first.

Consistency IS the product: a client comparing two reports must find the same structure, same subsection order, solution-last discipline everywhere.

### 10.1 Title, impact & solution integrity

- Finding titles are complete and descriptive — NEVER truncated with literal "..." (e.g. no "…te" endings). A truncated title is a discarded finding — redo.
- **Solution topic must match Description topic.** A booking-flow finding gets a booking-flow solution; a security-header finding gets that header's fix. Copy-pasted solutions from another finding type are a critical error.
- **Impact is per-topic and honest.** State the real consequence of THIS finding type. The boilerplate "prevents AI assistants from surfacing your business… funneling that booking to a competitor" is banned as a copy-paste — especially on findings (like missing security headers) where that claim is not the actual mechanism.
- **Strengths are strengths.** Something that demonstrably works (reachable booking form, correct structured data, readable pricing) is reported as a Strength — or, if retained in the findings list, its Solution PRESERVES the working behavior rather than demanding it be added.
- **Normal business choices are not defects.** A service business (plumber, electrician, roofer) not listing fixed prices is NORMAL — they often have no fixed price, so never ship "no prices found" as a problem. A business that provides a phone number and a contact form but no email is making a normal, intentional channel choice — never ship "no email found" as a problem. Only the absence of ALL contact channels, or content that genuinely blocks AI agents from reading it, is a defect. When a check finds a normal absence, record it as an observation in your worklog — not as a finding for the client.

### 10.2 Evidence references must be real

Every `Evidence:` line in the report references files that actually exist in that site's folder. Screenshots must be present under `Screenshots/`; any raw-capture file referenced must also be shipped in the same folder. Evidence may also reference the per-page `data/<page>.json` file (§6.1) that contains the raw extracted data from the page where the finding was observed. A reference to a file that doesn't exist invalidates the finding's evidence — that finding does not ship. The client report must NOT contain a "Files in this site folder" inventory section (§4.3); all evidence references are inline per finding only.

### 10.3 No internal jargon in client-facing files

Client-facing files (`_audit.md`, `_audit.pdf`, `README.md`, `Outreach.md`) are for the BUSINESS OWNER — not for you, not for the engineer who requested the audit. Apply these rules to every client-facing file:

- **Banned terms** (translate to plain English or remove): "Check 1", "Check 2", "Check 3", "Check 4", "Check source", "Reproduction", "Gate-2", "needs manual verification", "downgraded", "Review Wave", "Audit Wave", "industry group G2", "orchestrator-direct", "degraded mode", "Browser Use", "§10", "§13.4", "per §7", "severity", "Critical/High/Medium/Low severity labels", "findings shipped to client", "findings downgraded".
- **Legitimate technical terms are NOT banned** — `robots.txt`, `JSON-LD`, `schema.org`, and `llms.txt` are real findings, not internal jargon. When one is the actual subject of a finding (e.g. "robots.txt blocks AI crawlers"), name it directly — precise terminology is what makes the report credible. Ban only the internal-workflow jargon above, never the technical substance of the audit.
- **Fail: "See Check 3 if reachable"** → succeed: embed the screenshot directly or link to `Screenshots/<filename>.png`.
- **Fail: "Not extracted. See Check 2 robots.txt"** → succeed: state the fact in plain English ("No social media links found on the homepage" or add the actual links if found).
- **Fail: "Audit method: orchestrator-direct (Python scripts + agent-browser CLI fallback per §2.3 degraded-mode worklog)"** → the owner does not care how you ran the audit. Remove this line entirely from the client report.
- **Fail: "Findings downgraded to needs manual verification: 0"** → the owner does not know or care about your internal verification process. Remove this line entirely.
- **Fail: "Findings shipped to client: 8 (0 Critical, 0 High, 6 Medium, 2 Low)"** → the owner only needs to know how many problems were found. Write: "**Problems found: 8**" — no severity breakdown. Severity is for your internal prioritization only.
- **Fail: "Estimated annual loss from AI-agent invisibility: $1110 (severity-weighted, clamped...)"** — fabricated, formula-invented numbers destroy credibility. A researched left-on-table estimate per §12.6 IS allowed, but only when it is traceable to industry research and phrased as a conservative approximation. Never a severity-weight formula, never a rounded-up guess.

Every reference to another finding, section, or file from within a client-facing document must point to something the reader can actually find and understand. If the reference is meaningless to a business owner, it should not exist.

---

## 11. `README.md` — Business Dossier Spec (DESIGNATED SENSITIVE-INFO FILE)

`README.md` is a **business dossier** — a factual, scannable reference about the business itself, used by you to personalize outreach and by future sessions to remember the client. It is NOT a client-facing sales document and it is NOT the audit report. It is written in plain English, one clean section per fact.

**PRIVACY ROLE:** `README.md` is the ONE and ONLY file that stores sensitive client contact info — emails, phone numbers, owner names, addresses. It is packaged into `Deliverables.zip` for your private use but is NEVER pushed to the GitHub ledger repo (§9, §14.3). Because it is the sole holder of this data, every other client-facing file (audit.md, Outreach.md, data/*.json) must NOT contain raw contact PII — they reference or describe without exposing it.

**Header line exactly: `# Business Dossier — <Real Trade Name>`** (spell "Dossier" correctly — the word is D-O-S-S-I-E-R, not "Dozer").

### 11.0 README.md template (follow this EXACT structure — no improvisation)

```markdown
# Business Dossier — <Real Trade Name>

## Business Basics
- **Domain:** <domain.tld>
- **Industry:** <e.g. Electrician>
- **Location(s):** <full address(es) if found; if none found, write "None">
- **Hours:** <as published; if none found, write "None">

## About the Business
<one to three short plain-English sentences: who they are, who they serve, what they do. Summarized by YOU — never a raw copy-paste dump of homepage text.>

## Services / Products
<bullet list of services or products, from the site; include price points where the site states them>
- <Service A> — <price if stated>
- <Service B> — <price if stated>

## Contact Channels
- **Phone:** <phone if found; else "None">
- **Email:** <validated email if found; else "None">
- **Contact Form:** <working or not, from the site; else "None">
- **Social Media:** <actual social links if found (check the footer!); else "None">
- **Other:** <any other contact channel>

## Team
- <Name — role> (only if public; else "None")

## Notable Facts for Outreach
<2–4 bullets of genuinely specific, personalization-worthy facts: an award, a specialty, years in business, a unique offering, a named team member with a story. Every fact must be real and verifiable on the site.>

## Source URLs
- <URL of each page where the facts above were found>
```

### 11.1 Dossier field discipline

- **Business name is the real trade name** (from homepage/logo/About/header), not the raw domain. It is used verbatim in `Outreach.md` subject lines and hooks.
- **Every extracted field matches its label** — Hours holds hours, Location holds a real address, Price points hold prices, Contacts hold well-formed emails.
- **Every field that yields nothing is written as `None` — never left blank, never filled with a placeholder like "(see homepage)", never skipped.** If the site has no address, the field says `None`. If it has an address, it is written out in full.
- **Social media and team info require a FULL page scroll before you declare them absent** (§4.6). These are the fields most often hidden in footers and animation-revealed sections — the single most common extraction failure is reporting "None" when the data was just below the fold. Check the footer and the entire page height first.
- **Emails are validated before writing.** Each extracted email must pass a sanity check: no stray leading/trailing characters (e.g. a spurious leading "n"), well-formed `local@domain.tld`, and cross-checked against visible contact text on the site. A corrupted email is fixed or marked unverified — never shipped corrupted.
- **Source URLs point to real paths** relative to the workspace root; no invented `sites/` prefix.
- **About the Business is a summary you write**, not a paste. Read the site, understand it, then write 1–3 clean sentences in your own words. Raw homepage text copied into the field is a failed field.
- **Grammar:** no article errors ("a independent" → "an independent"), no subject-verb mismatches, no orphaned fragments, no double spaces.
- **No duplicated facts within the same file.** Each fact appears once. (The domain appears once in Business Basics, not again in Source URLs; the phone appears once in Contact Channels, not three times.)

---

## 12. `Outreach.md` — Sales Protocol (expanded)

### 12.1 The Two Minds — mandatory before writing a single word

Every `Outreach.md` is written by a sub-agent wearing TWO minds simultaneously, and every business requires its own separate fitting — no two owners think alike, so the copywriter re-becomes a different person per site. Writing from a generic "small business owner" view is failure; you become THAT dentist, THAT plumber, THAT salon owner, built from their README dossier facts (trade, city, prices, hours, how they present themselves).

**Mind A — The Owner's Chair (empathy pass).** Before drafting, sit in the actual chair: role-play being THIS owner — busy, phone in hand, mid-customer, skeptical of strangers selling things. Interrogate yourself explicitly and answer honestly IN YOUR SUB-WORKLOG before drafting:
- "If I were this man/woman, what sentence would make ME stop scrolling and read the rest?"
- "What exact wording would make me accept the deal on the spot?"
- "What wording — even technically true — would make me smell a scam and hit delete?"
- "What would make me file this under 'I'll reply later' (which means never)?"
- "What would I need to NOT feel talked down to, not feel frightened, and not feel sold to?"
Write the email that passes YOUR OWN gut test in that chair. If the draft wouldn't convince you-as-owner, it doesn't leave the desk.

**Mind B — The Salesman (pitch pass).** Then switch hats and build the pitch deliberately: strongest verified hook first, one clear bridge, one modest number, one two-tier offer, one frictionless ask. Every element earns its place or gets cut.

Both minds run for every site, every time — empathy decides WHAT to say; salesmanship decides HOW to say it in ≤150 words.

**Baseline reader reality (both minds must respect it):** a non-technical local business owner reads email on a phone, in seconds, between customers; distrusts anything that smells like tech jargon or a scam; cares about three things — customers, money, reputation. They've heard "AI" in the news and don't know what it means for them. The email wins by being CONCRETE about THEIR site, SMALL-numbered, and EFFORTLESS to answer. Their competitor getting recommended by AI assistants while they're invisible is the fear — stated factually, never hysterically.

### 12.2 File format — ready to copy-paste (To: MUST be filled)

```
To: [See README.md in this folder — sensitive contact info kept local]
Subject: <see 12.3>

<body — see 12.4>

— [Your name]
```

The `To:` line does NOT contain the raw email/name — that sensitive data lives exclusively in `README.md` (§11), which is the designated sensitive-info file and is never pushed to GitHub (§9). The local reference `[See README.md in this folder]` is valid because the zip contains README.md right next to Outreach.md — the user opens the zip, sees the folder, and reads the contact from README.md there. No attachments mentioned, no links required (link-free avoids spam filters; the report is offered, sent on reply). An email whose `To:` is missing or empty fails the §12.8 gate. If no verifiable email exists on the site, that site's Outreach.md cannot be marked ready.

### 12.3 Subject line rules

≤55 characters. Contains the business name OR one concrete observed detail. The business reference is the REAL trade name from the README dossier (e.g. "G & G Law, LLC"), never the raw domain without branding ("Gglawoffices"). Creates a curiosity gap; banned: ALL CAPS words, multiple exclamation marks, "FREE", "boost your business", "don't miss out", anything generic enough to describe any business. The subject's ONLY job: earn the open from a skeptical owner.

Good pattern examples (adapt, never mass-template): `Question about <Business>'s online booking`, `<Business>: found something on your homepage`, `Can ChatGPT find <Business>? I checked.`

### 12.4 Body structure (≤150 words total)

1. **Hook (1–2 sentences):** one SPECIFIC verified finding on THEIR site, described in human terms, referencing at least one REAL business-specific detail (the actual booking platform by name, a specific service, a widget, a genuine quirk — never a pure domain/city substitution). "When someone asks ChatGPT for a <trade> in <city>, your site doesn't come up — I checked why." Not "your website has issues."
2. **Bridge (1–2 sentences):** why now — people increasingly ask AI assistants instead of searching, and assistants recommend businesses they can read.
3. **Proof (1–2 sentences + optional screenshot):** the email must convince a skeptical owner this is real, not a scam. State the count of concrete problems found on THEIR site ("I found 8 specific things on your site that do this"). Then, if a defensible estimate exists per §12.6, state the approximate left-on-table figure: "Conservatively, this likely costs you around $X/year in lost jobs." The strongest proof is a single screenshot of one visible problem on their own site embedded in the email — one screenshot, one problem, no more. If a screenshot is included, reference it directly (e.g. `![screenshot](/Screenshots/...png)` in `Outreach.md`) so the owner sees their own site and thinks "they actually looked." A screenshot of an ABSENT thing (like a missing contact form) is useless — only screenshot what exists.
4. **Offer (2 sentences):** two tiers, plainly and credibly: a full written audit + priority fixes for `$FIXED_AUDIT_FEE_USD`; or the audit report alone (everything found, clearly explained) for `$200`. The full package is NOT more expensive because fixing is "extra" — the report-only tier is simply the cheaper option for owners who want to decide first. No pricing gymnastics, no fake discounts, no "act now" urgency.
5. **CTA (1 sentence):** a single, concrete, low-pressure ask. BANNED phrasing: "Reply 'send it' and I'll email you the summary" — this is the exact wording of common scam posts on X/Twitter and instantly reads as a scam. Use a direct, honest alternative, e.g. "If you'd like, I can email the full list — just reply and I'll send it." or "Reply to this email and I'll send over the details." No "comment 'X'" patterns, no gimmicky engagement bait.

### 12.5 Language constraints

Fifth-grade reading level. BANNED vocabulary (translate to outcomes instead): schema, structured data, SEO, crawl/crawler, render, metadata, optimization, "AI-powered solutions". Say "when someone asks ChatGPT/Siri/Google's AI about...", "your site hides its prices from them", "a rival gets picked instead."

### 12.6 Business intelligence — the left-on-table estimate

Before writing the email, the copywriter must understand THIS business's money — zoom out, look at the business from above, and form a real picture of what it earns. This is not a fabricated formula; it is a researched, conservative estimate that makes the owner pay attention.

**The research pass (mandatory, before any draft):**
1. **Understand the business type's economics.** Even when the site lists no prices (very common for service businesses), establish the industry's realistic numbers: average job/project value, typical revenue per client, revenue per day/month for this business type. Use web search for industry averages (e.g. "average electrician job value", "plumber average invoice", "salon revenue per client") and reason from the business's own signals (location, service area, team size, premium vs budget positioning).
2. **Estimate how many clients the audited problems cost.** Take a conservative view: of the customers who would have found and used this business through an AI assistant, what fraction are currently lost to the identified problems? Be conservative — never inflate. If evidence supports "some are lost", use a modest share.
3. **Compute the left-on-table number.** `(estimated lost clients per month) × (average revenue per client)`. The result is an APPROXIMATE annual figure. It is explicitly an estimate — reasonable, defensible, never exact.
4. **Sanity-check against the business type.** An electrician losing a single client is losing thousands (average job value), so a $1,000 "annual loss" figure for a trade business is implausible — flag and correct such numbers. The number must feel true for THIS industry, not formulaic.

**Where it goes:** the left-on-table number appears in the Outreach body (§12.4 point 3, replacing the old fabricated figure) and MAY appear once in the audit Executive Summary — always phrased as an approximate estimate ("conservatively, this likely costs you around $X/year in lost jobs"), never as an exact accounting. The number's only job: make the modest fix fee ($500) look trivial next to the money at stake.

**Truthfulness bar:** the estimate must be traceable to (a) industry-average research the copywriter actually performed, and (b) a conservative reasoning chain. It must never be a rounded-up guess, never "severity-weighted formula" output, never a number invented to impress. If the copywriter cannot build a defensible estimate, it omits the number rather than fabricating one.

### 12.7 Truthfulness constraints (hard)

Every claim traces to a CONFIRMED finding in that site's report. No invented urgency, scarcity, or statistics. No claiming things "everyone knows" that we didn't verify. The left-on-table estimate (§12.6) is clearly labeled as an approximate estimate, never presented as exact accounting. If the audit found little wrong, the email says so honestly — trust compounds; one exaggerated email burns the niche.

### 12.8 Quality gate

An outreach draft ships only after the §4.6 copywriter variant + this gate pass ALL of the following:
- `To:` is present as the local README reference (never empty, never a fake/placeholder email; the real recipient lives in README.md per §12.2).
- The §12.1 Owner's-Chair interrogation was actually performed and its answers recorded in the sub-worklog.
- The real trade name is used in the subject/hook — never the raw domain as a fake brand (§12.3).
- ≥2 unique personalization details from README facts, including at least ONE genuine technical/business detail from the audit evidence (booking platform by name, a widget, a service quirk) — not just domain/city substitutions (§12.4).
- Proof present: the email states the confirmed problem count and, where a visible problem exists, embeds ONE screenshot of it (§12.4 point 3).
- If a left-on-table figure is included, the §12.6 research pass was actually performed and is traceable (industry-average source + conservative reasoning recorded in the sub-worklog); otherwise no figure was invented (§12.6).
- CTA is the honest direct alternative — the banned "Reply 'send it'..." phrasing is never used (§12.4 point 5).
- Pricing is the two-tier structure: full audit + fixes at `$FIXED_AUDIT_FEE_USD`, report-only at `$200` — no "fixing is extra" framing (§12.4 point 4).
- Zero banned words; ≤150 words; correct grammar (no "a independent" errors); single CTA; no fabricated dollar-loss figures (§12.7).
- Every factual claim is traceable to a confirmed finding (§12.7).
- Final gut test answers YES to "would I, sitting in this owner's chair, reply to this?"

A draft failing any of the above = redo. A draft that only passes the Salesman pass but fails the Owner's-Chair test = redo. Generic-feeling output = redo.

---

## 13. Resource Discipline & Tool-Failure Protocol

- Sandbox ≈ 4GB RAM, no elevated privileges. Headless always. Sequential contexts per sub-agent; release before the next unit. If RAM pressure appears (slowdowns, OOM kills), reduce live contexts before anything else, and note it.
- Save progress to disk continuously — after every meaningful step — so a timeout never loses work.
- Trivial command failures: retry 3–5 times with short waits before escalating. Real blockers: log, reroute, CONTINUE. Infrastructure noise is never a signal to stop the run.
- A sub-agent timeout mid-unit = likely partial progress: dispatch a continuation sub-agent with the partial state (`sub-worklog-<N>.md` + existing artifacts) as context. Never treat a timeout as "stopped."
- Only stop when: every to-do closed, queue resolved or honestly reported per §17, and nothing further improvable remains in-scope.

---

## 14. Progress Tracking & Ledger Sync

### 14.1 During the session

Never audit an excluded domain (§2.1). Keep candidate screening results in `worklog.md` — future sessions benefit from knowing WHY a domain was disqualified.

### 14.2 End-of-session ledger update

Append one row per newly audited site to `PROGRESS.md` (website-level only, never findings detail). **PRIVACY: PROGRESS.md rows carry NO client PII** — no emails, no phone numbers, no owner names, no addresses. The row is just the domain, date, industry group, outcome flags, and a neutral one-line note. All sensitive detail stays in the site's local `README.md` (§11), which is never pushed (§9).

```
| Domain | Date | Industry Group | Client Responded | Client Purchased | Notes |
| exampleclinic.com | 2026-08-26 | Group 1 | pending | pending | Dental clinic, 1 location, 4 findings |
```

Update `Client Responded` / `Client Purchased` in LATER sessions when outcomes are actually known — values are `pending` until reality reports in. Outcomes are NEVER guessed, fabricated, or marked optimistically.

**Count reconciliation (mandatory):** the `Notes` finding count must EQUAL the actual shipped-finding count in that site's `_audit.md`. Read the audit.md, count its shipped findings, write that number — never guess, never estimate from memory. A PROGRESS.md row whose count contradicts its own report is a critical error (§18).

### 14.3 Push-or-package

Attempt `git commit && git push` of the updated `PROGRESS.md`. **ONLY `PROGRESS.md` is ever committed to the ledger — never a site folder, never `README.md`, never any site artifact.** The ledger's `.gitignore` blocks everything except `PROGRESS.md` and the repo's own README (§9); never override it with `git add -f`, never stage site files. If credentials are absent and push fails: save `PROGRESS_update_<date>.md` (the new rows + any outcome-column updates) at `Deliverables.zip` root, state plainly in the Final Report that the ledger needs a manual push, and include the exact rows to paste. Never claim "ledger updated" without platform-qualified evidence of WHERE the update lives (pushed to GitHub vs packaged in zip vs workspace-only).

---

## 15. Deliverables.zip

Built at session end, placed in the download folder:

```
Deliverables.zip
├── example-clinic-com/          ← one folder per FULLY-CLEARED site, named per §9
│   ├── example-clinic-com_audit.md
│   ├── example-clinic-com_audit.pdf
│   ├── README.md
│   ├── Outreach.md
│   ├── Screenshots/
│   └── data/
├── another-business-com/ …
└── PROGRESS_update_<date>.md    ← only if §14.3 push failed
```

### 15.1 Compression & size discipline (MANDATORY)

- **NEVER zip with zero compression.** Build the archive with maximum compression (deflate). A `store`-method zip from a missed flag is a critical packaging failure — the archive is only done when it is genuinely compressed.
- **Screenshot discipline starts at capture time** (screenshots dominate the zip size — this is the actual lever):
  - Capture browser screenshots as **FULL-PAGE captures** (§4.6 — never cropped/custom areas) at a maximum width of **1000px** (smaller where the page allows). Never full-resolution 1280px+ captures.
  - Save screenshots as **256-color palette PNGs** (quantized) — visually near-identical for UI/web captures, roughly 5–10× smaller than 32-bit PNG. Keep the `.png` extension and the EXACT filenames (`<domain>_check<N>_<seq>.png`): the audit markdown references screenshots by filename (§10 Evidence), so renaming or changing formats breaks every reference.
  - Never include a screenshot that proves nothing — every image in `Screenshots/` must map to a documented finding.
- **Size target (preferable, not a fixed limit):** aim for `Deliverables.zip` to come in under ~10 MB. The final size can't be predicted before compression, so treat this as a guideline, not a hard cap — compress heavily (below), measure, then judge.
- **If it comes out too large to download:** compress harder BEFORE splitting — drop screenshots to 800px, re-quantize aggressively, strip redundant near-duplicate frames.
- **Mandatory split once over 10 MB:** if, after maximum compression, the zip is still ≥ 10 MB, split into `Deliverables_1.zip`, `Deliverables_2.zip`, … (each part < 10 MB) by partitioning per-site folders roughly evenly across parts; `PROGRESS_update_…` goes in part 1. Name every part explicitly and state the split in the Final Report. Never ship a single zip the user cannot download.
- **Integrity verification after compression (mandatory):** after re-zipping, verify the archive opens, the file count matches the source set, folder structure is intact, and every markdown-referenced screenshot path resolves inside the zip. A size win that corrupted data is worthless — a corrupted deliverable is worse than a big one. Compress first, verify second, ship third.

**Packaging validation checklist (run before finalizing; all must pass):**
- [ ] Folder count == sites that cleared ALL six checks + Review + Assembly this session (NOT `NUMBER_OF_WEBSITES` if the queue didn't clear — §17 governs)
- [ ] Every folder contains exactly the 6 required items — 2 report files + README + Outreach + Screenshots/ + data/ (one JSON per page); zero stray/raw files anywhere in the zip
- [ ] Every `.pdf` opens and matches its `.md` core content
- [ ] Every finding's referenced screenshot exists in that folder's `Screenshots/`
- [ ] Spot-check: 3 random `Outreach.md` files pass §12.8's gate; 3 random reports follow the §10 template exactly; each random report's `data/` folder contains a JSON per page covered by that site's findings (§6.1)
- [ ] No sub-worklogs, no worklogs, no screening notes, no temp artifacts in the zip
- [ ] Ledger state: pushed (link) or packaged (`PROGRESS_update_…` present) or honestly absent-with-reason
- [ ] Privacy check: NO client site data (README.md, audit files, screenshots, data/*.json, or raw emails/phones/names/addresses) appears in the ledger repo or in any `PROGRESS_update_…` file — only the dedup rows (§9, §14.2, §14.3)
- [ ] Zip built with real compression — never `store` method (§15.1)
- [ ] Zip size preferably under ~10 MB; if larger, compress harder or split — never undownloadable
- [ ] Post-compression integrity check passed: opens, file count + structure + every markdown-referenced screenshot path intact (§15.1)
- [ ] PROGRESS.md Notes counts match each site's actual shipped-finding count (§14.2)
- [ ] No finding references a file that doesn't exist; no false "Files in this site folder" inventory (§10.2)
- [ ] Finding-integrity spot check (3 random reports): titles not truncated, Solution topic matches Description, no duplicate findings, no fabricated dollar-loss figures, impact is per-topic (§10.1/§10.3)
- [ ] Client-audience spot check (3 random reports + 3 READMEs): no internal jargon (Check N, severity labels, audit method, section references), About written as a summary not a paste, fields filled or "None" (§10.3, §11)
- [ ] Outreach spot check (3 random): To: filled, real trade name used, ≥1 technical business-specific detail, left-on-table figure (if present) traceable to §12.6 research (§12.8)

---

## 16. Definition of Done

The session is DONE only when ALL of the following hold — evaluated once, honestly, at the end:

1. Full `NUMBER_OF_WAVES` ran, ending on a Review Wave whose close-out loop left ZERO remaining must-fix items (§5.5).
2. The coverage matrix shows every shipped site at 6/6 checks + Reviewed + Assembled; no partially-audited site anywhere near the deliverables.
3. Evidence gate sweep (to-do item 8) passed: every shipped finding has Gate-1 proof; every behavioral finding has Gate-2 reproduction or sits in `needs manual verification` — excluded from client files, counted in the Final Report.
4. Every shipped site has valid `Outreach.md` (§12.8 gate) and `README.md` (§11 spec).
5. `Deliverables.zip` built and passed the §15 checklist.
6. Ledger synced per §14.3 with truthful status.
7. `worklog.md` reflects the real run — including failures, degraded modes, downgraded findings, and skipped candidates.
8. Review coverage is 100% — every shipped site's behavioral findings were independently reproduced; no sample-based review (§7).
9. Finding-integrity sweep passed: no truncated titles, no topic-mismatched solutions, no duplicate findings, no fabricated dollar-loss figures, no evidence references to nonexistent files (§10.1–§10.3).
10. PROGRESS.md counts reconciled against actual audit.md findings (§14.2).
11. Client-audience check passed: no internal jargon in any client-facing file (§10.3); every README follows the §11 template; outreach passes the full §12.8 gate including §12.6 left-on-table research traceability.

If wave budget ran out before clearing the queue, that is stated PLAINLY in the Final Report as current state — which sites completed, which didn't and why, and the concrete recommendation (bigger pools / more waves / fewer sites) for next session. Honest incompletion is acceptable; hidden incompletion and trimmed audits are critical failures.

---

## 17. Final Report (chat, end of run)

Structured, factual, no smoothing:

- **Sites Fully Audited & Delivered** — count + domain list.
- **Sites Skipped (out-of-scope / failed Q-gates)** — domain + which gate/reason (summary counts per gate).
- **Sites Started but Not Completed** (if any) — domain, checks done vs pending, exact reason.
- **Findings Statistics** — total confirmed findings shipped, by severity and by check source; count downgraded to "needs manual verification" with one-line reasons.
- **Free-Tool Results** — tools used, agreements ("confirmed also by X"), failures (rate-limit/paywall/auth) — and confirmation none blocked the run.
- **Browser Mode** — Browser Use (nominal) or degraded fallback with reason.
- **Ledger Status** — pushed / packaged / blocked, with evidence of which.
- **Coverage Matrix Snapshot** — the final table state.
- **Recommended Adjustments for Next Session** — pool sizes, wave count, NUMBER_OF_WEBSITES, group targeting — driven by THIS run's actual throughput data.

---

## 18. Hard Limits

Violation of any of the following is a CRITICAL FAILURE of the run, regardless of output volume:

- Auditing any domain present in the PROGRESS.md exclusion set (§2.1).
- Shipping any finding lacking Gate-1 proof or unreviewed (§7), or presenting a downgraded finding as confirmed (§7, §16.3).
- Treating free tools as primary evidence, authenticating to any service, or providing identity/payment details (§8 banners).
- Using the built-in browser after successful Browser Use setup, or claiming nominal mode while degraded (§2.3).
- Unequal per-site coverage — any site receiving fewer than the full six checks + review while another ships complete (§5.3).
- Launching a wave short of configured count without immediate correction, or running waves concurrently/out of sequence (§5.1, §5.4).
- Enterprise targets entering the audit queue (§3 banners, §3.2 Q2).
- Behavioral simulations crossing the confirmation boundary — real bookings, orders, payments, or sends (§6).
- Fabricated outcomes in `PROGRESS.md`, invented urgency/statistics in outreach, or any claim without traceable evidence (§12.7, §14.2).
- Fabricating or mis-reconciling numbers — invented dollar-loss figures, per-finding dollar figures, PROGRESS counts that don't match the audit.md (§10.3, §14.2).
- Shipping findings with truncated titles, topic-mismatched solutions, duplicate findings, or evidence references to nonexistent files (§10).
- Shipping a site whose behavioral findings lack independent reproduction (sample-based review) (§7).
- Shipping an Outreach.md with an unfilled To:, a domain-as-brand name, zero business-specific detail, the banned "Reply 'send it'" CTA, or fabricated pricing (§12).
- Shipping any client-facing file containing internal jargon (Check N, severity labels, audit method, section references) instead of plain English (§10.3).
- Committing or pushing ANY client site data — site folders, README.md, audit files, screenshots, data/*.json, or any raw contact PII (emails, phones, names, addresses) — to the GitHub ledger repo. Only `PROGRESS.md` may be pushed (§9, §14.3).
- Packaging a partial site, stray files, or skipping the §15 validation checklist.
- Stopping before the single stopping condition of §5.5, or hiding incompletion instead of reporting it (§16).

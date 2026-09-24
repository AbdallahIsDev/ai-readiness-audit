# SALES WORKFLOW — Outreach → Demo → Meeting → Close → Post-Sale

> **What this file is.** The human half of the operation, end to end. The directive (`AUDIT_EXECUTION_DIRECTIVE.md`) ends at a drafted `Outreach.md`; this file starts at the moment you press send and carries through to the second sale. Every stage has: what to do, what to say, how long it takes, what it costs, how it can fail, and the exit criterion that lets you move on.
>
> **The one-line version.** Build a real one-page demo → ask permission to show it (never send it cold, never mention price) → send a 3-minute recorded walkthrough → book a **20-minute** call → screen-share the demo, talk 43% of the time → give **one** price → send the payment link **while you are still on the call** → then sell the care plan.
>
> **Labels used throughout.** `[S]` = sourced from a named study or vendor dataset, with the URL in §12. `[E]` = my estimate or a reasoned derivation, not measured. `[C]` = a claim from a creator/vendor with no dataset behind it — direction may be right, the number is not evidence. Do not quote an `[E]` or `[C]` to a client.



---

## 0. How to use this file

### 0.1 Scope boundary — who does what

| Stage                                                                 | Who                                                                       | Output                        |
| --------------------------------------------------------------------- | ------------------------------------------------------------------------- | ----------------------------- |
| Sourcing, no-website proof, contact hunt, dossier, outreach **draft** | Cloud agent (directive §3B, §11B, §12B)                                   | `websites/<slug>/Outreach.md` |
| **The contact sheet — every target's emails, phones and DM deep links in one file** | **The cloud agent** (directive §3.6–§3.7 — runs in BOTH modes), read back and verified before the run continues | `OUTREACH_CONTACTS.md` (zip root) |
| **Geographic targeting — high-income markets only** | **The cloud agent**, from the operator-set `TARGET_COUNTRIES` (directive §3.5 — runs in BOTH modes). Egypt and every other low / lower-middle / upper-middle-income economy are excluded at sourcing, before any audit or contact-hunt work is spent | A candidate pool of sellable leads |
| **Sending, replying, booking, meeting, closing, delivering**          | **You (this file)**                                                       | Money                         |
| One-page demo build                                                   | **The cloud agent** when `GENERATE_LANDING_PAGE: ON` (directive §3C, unit N5) — otherwise you, from a per-trade template. Either way, **you deploy it.** | `demo.<yourdomain>/<slug>`    |

The agent's `Outreach.md` is a **draft**. Nothing in this file is the agent's job, and nothing in the directive's §16B Definition of Done changes because of it. Keep it that way — the boundary is what stops a cloud run from ever touching a client.

**Start every outreach session from `OUTREACH_CONTACTS.md`.** It is the agent's click-to-contact sheet: one entry per business, every email, every phone (with its WhatsApp/Telegram state), and every DM-able social profile as a direct link — `m.me/<page>`, `ig.me/m/<handle>`, `wa.me/<number>`, `t.me/<handle>`, Reddit compose, X profile, `mailto:`. Open it in a Markdown preview so the links are clickable, then work straight down it. **The `Outreach.md` in each folder is the message; the sheet is the route to send it.**

### 0.2 The funnel at a glance

Every stage below, with its job, its cost, and its exit criterion.

| # | Stage           | Job                               | Time per unit                            | Exit criterion                         | §  |
| - | --------------- | --------------------------------- | ---------------------------------------- | -------------------------------------- | -- |
| 1 | **Outreach**    | Earn a reply. Nothing else.       | 3–5 min to send                          | A reply that is not "no"               | §2 |
| 2 | **Walkthrough** | Earn the meeting.                 | 10–15 min to record (reusable per trade) | They ask a question or agree to talk   | §3 |
| 3 | **Book**        | Get 20 minutes on a calendar.     | 2 min                                    | Confirmed invite, ≤5 business days out | §4 |
| 4 | **Meeting**     | Show, qualify, price, close.      | 20 min + 15 min prep                     | Payment link sent **on the call**      | §5 |
| 5 | **Close**       | Turn yes into money.              | 10 min                                   | Deposit received                       | §6 |
| 6 | **Post-sale**   | Deliver, then sell the care plan. | 5–10 days build                          | Site live + care plan signed           | §7 |

**The critical path is stages 3 and 5.** Stage 3 is where most volume dies (20–40% no-show `[S]`). Stage 5 is where most *revenue* dies — 20–35% of verbal yeses never convert to payment when you invoice after the call `[S]`. Both are solved by mechanical rules, not by being more persuasive: cap the booking window (§4.5), and send the payment link before you hang up (§6.3).

### 0.3 Honest conversion math — what to actually expect

The staged model you described (35% → 60% → 80% at the meeting) comes from creators, not datasets. The *shape* is right — each step up the funnel raises the odds, and closing on the call is worth real money. The *numbers* are not evidence and I would not build a plan on them.

Here is what published data says, next to a model of this specific funnel.

**Published cold-email benchmarks, H1 2026 `[S]`:**

| Metric                | Bad   | Average  | Good   | Top decile |
| --------------------- | ----- | -------- | ------ | ---------- |
| Reply rate (cold B2B) | <1%   | 3–5%     | 5–8%   | 8–15%      |
| Positive-reply rate   | <0.3% | 0.8–1.5% | 1.5–3% | 3–6%       |
| Meeting-booked rate   | <0.2% | 0.5–1%   | 1–2%   | 2–4%       |
| Sends per customer    | —     | ~800:1   | 400:1  | 200:1      |

**Two benchmarks that matter more than the table:**

- **Permission-first video sequences see 15–22% reply rates, versus 3–4% for unsolicited video drops** `[S]`. This is a vendor claim about their own tooling, so discount it — but the *mechanism* is the point: asking permission before sending the asset is the difference, and it is free. Your flow is already permission-first.
- **A specific ask converts at 2–3x an open-ended one** `[S]`. "15 minutes Tuesday or Thursday to show you the demo" beats "would love to chat."

**Model for this funnel `[E]` — replace with your own numbers after 200 sends:**

| Step                                    | Conservative | Good    |
| --------------------------------------- | ------------ | ------- |
| Sends                                   | 100          | 100     |
| Replies                                 | 3            | 7       |
| Positive / curious                      | 1.5          | 4       |
| Meetings booked                         | 1            | 2.5     |
| Meetings attended (65–80% show)         | 0.7          | 1.8     |
| **Closed at $1,200**                    | **0.15**     | **0.5** |
| First-year value incl. care plan (§7.4) | $520         | $1,725  |

Read that as: **roughly 200–600 sends per sale**, which lands between the "good" and "top decile" published ratios — appropriate for a personalized, build-first approach, and *not* a promise. Two consequences worth internalising now:

1. **Volume is not optional.** At 20 sends/mailbox/day `[S]`, the good case is a sale every ~2 weeks per mailbox. This is a numbers game with a good hook, not a clever email that goes viral.
2. **The care plan is half the money.** A $1,200 one-off is a small deal. The same client on a $250/mo care plan is $4,200 in year one (§7.4). If you only ever sell the build, this business does not work.

**Your creator numbers, restated honestly:** the 35% / 60% / 80% ladder `[C]` is best read as *"each step roughly doubles the odds of the next"* — which the data supports — rather than as a forecast. The one piece of it I'd defend with real data is the last step: **collecting payment on the call lifts verbal-yes-to-revenue conversion by 40–60% `[S]`**. That single behaviour is worth more than every script in this file.

### 0.4 The five hard rules

1. **No price in message one.** Price anchors to cost before value exists `[S]`. Price is a §5 event.
2. **Never send a bare demo link before the walkthrough.** They scroll alone, find one thing they don't like, and go quiet. The link is the payoff of the call, not the opener. (If they *insist*, send it — see §2.6 — but book the call anyway.)
3. **The meeting is 20 minutes.** Booked as 20, planned for 18, hard stop at 20. Reasoning and data in §4.1.
4. **The payment link goes out on the call.** Not after. Not tomorrow. §6.3.
5. **One thing at a time.** One offer, one price, one CTA per message and per stage. Add-ons are a §7 conversation, never a §2–§6 one.

---

## 1. One-time setup — before outreach #1

Do all of this once. It is boring, it takes an afternoon, and skipping any of it caps the whole funnel.

### 1.1 Sending infrastructure

| Item                | Rule                                                                             | Why                                                                                                      |
| ------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| Sending domain      | A separate domain or subdomain, not your main one                                | If it burns, your business email survives                                                                |
| SPF / DKIM / DMARC  | Configured before the first send                                                 | Non-negotiable `[S]` — without them you are spam                                                         |
| Warm-up             | **6–8 weeks** to full volume `[S]`                                               | Was ~3 weeks; M365 and Gmail filters have tightened                                                      |
| Volume ramp         | Wk 1–2: 5–10/day → wk 3–4: 15–20 → wk 5–6: 30–40 → wk 7+: **50 max/inbox** `[S]` | Ramping too fast is the #1 way to kill a domain                                                          |
| Bounce rate         | **Under 1%** (2% is the hard ceiling) `[S]`                                      | A 5% bounce rate is 5x over the safe threshold                                                           |
| Spam complaints     | Under 0.1% `[S]`                                                                 | Hard ceiling                                                                                             |
| Tracking pixels     | **Off**                                                                          | They trigger filters and you're measuring replies, not opens                                             |
| Text-to-image ratio | 80/20; one link max `[S]`                                                        | A newsletter-looking HTML email is a spam signal                                                         |
| From name           | A real human name and address, never `no-reply@` `[S]`                           | Replies must land in a human inbox                                                                       |
| Batch size          | **Cohorts of ≤50** `[S]`                                                         | Smaller cohorts correlate with 2.76x reply rates — you catch deliverability problems before they cascade |

**Open rate is not a metric.** It is structurally broken `[S]`. Under 20% means you're in spam; over 40% means stop looking at it. Track replies.

### 1.2 The booking link

Set this up before you need it — never fumble a calendar link mid-conversation.

| Setting                | Value                                     | Why                                                                                                                                                            |
| ---------------------- | ----------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Tool                   | Cal.com (free, self-hostable) or Calendly | Both auto-detect the invitee's timezone — essential for Egypt→US                                                                                               |
| Event length           | **20 minutes**                            | §4.1                                                                                                                                                           |
| Booking window         | **Max 5 business days out**               | Meetings booked 8+ days out no-show at ~2x the rate of <48h `[S]`                                                                                              |
| Buffers                | 10 min before, 15 min after               | Late-running calls are the norm; you need the buffer more than they do                                                                                         |
| Days offered           | **Weekdays only**                         | Weekend-scheduled calls no-show at ~4x `[S]`                                                                                                                   |
| Confirmation questions | **3 max**                                 | A 3-question pre-call form lifts show rate 6–12 pts `[S]`; more than 3 kills bookings                                                                          |
| Reschedule             | **One-click link in every message**       | Converts ~30% of would-be no-shows `[S]`                                                                                                                       |
| Reminders              | Email at T-24h, email at T-1h             | See §4.5                                                                                                                                                       |
| Payment at booking     | **No**                                    | A deposit here would slash booking volume (`[S]`: deposit/paid consult lifts show rate 25–40 pts but "slashes booking volume") — wrong trade at this deal size |

**The three confirmation questions:**

1. What's the best number to reach you on if the link fails?
2. Roughly how do most of your customers find you today?
3. Anything specific you want me to make sure I cover?

Question 1 is a deliverability backstop, 2 gives you the discovery answer for free, 3 makes them a participant before they arrive.

### 1.3 The payment rail — get this right, it is Egypt-specific

**Stripe is not available in Egypt, and PayPal cannot pay out to Egyptian banks `[S]`.** This is the single most likely thing to break your close. Do not build a close around a checkout you cannot actually receive.

| Rail                                                       | Use it for                                                          | Effective cost                                           | Notes                                                                                                                           |
| ---------------------------------------------------------- | ------------------------------------------------------------------- | -------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| **Payoneer** (primary)                                     | Receiving from international clients — payment requests / invoicing | **1–3%** of received `[S]`                               | Withdraws to an Egyptian bank in EGP; ships a Mastercard. The default international receive rail for Egyptian freelancers `[S]` |
| **Wise** (backup)                                          | Corridors where it beats Payoneer; sending                          | **0.5–1%** `[S]`                                         | Receive support is corridor-dependent and has changed over time — verify your specific corridor before relying on it `[S]`      |
| Local Egyptian gateway (Paymob / Kashier / XPay / PayTabs) | Egyptian clients paying in EGP                                      | No FX cost                                               | Not relevant to this funnel unless you sell locally                                                                             |
| **PayPal**                                                 | Nothing                                                             | $40–60+ fees on $1,000, and the withdrawal problem `[S]` | Do not use                                                                                                                      |
| International bank wire                                    | Large amounts only                                                  | $25–75 fixed + FX spread `[S]`                           | Net on $1,000: ~$925–960 `[S]`                                                                                                  |


**Worked math on a $1,200 invoice `[S]`:** Payoneer nets roughly $1,164–1,188; Wise (if the corridor supports receive) roughly $1,182–1,194. Budget the fee into your price rather than eating it — $1,200 was already chosen as a round, easy-to-say number, and the 1–3% is the cost of getting paid at all.

**Do this once, before your first close:** create the payment-request product, send yourself a test payment from a card, and watch the whole client-side flow on a **phone browser**. §6.3 assumes you can produce a working link in under 30 seconds while on a call. If you have never done it, you will fumble it in front of a paying client.

### 1.4 Meeting tool

**Google Meet.** No download, works in any browser, opens instantly from a link, and non-technical owners join from a phone without installing anything. Zoom's feature depth is irrelevant to a 20-minute demo; the join friction is not.

Set up once:

- One permanent meeting link for the whole operation — never generate a new one per call.
- **Record your own calls** for self-review (§5.7), and say so at the start: *"I'll record this so I can send you a summary — is that alright?"* If they say no, don't.
- Pre-create a browser tab with the demo already loaded, at **110–125% zoom**, before every call.
- Camera on. Neutral background. Nothing readable behind you.

### 1.5 The demo factory

The demo is a **sales tool**, not the deliverable. Keep that boundary hard — a one-page demo is a demonstration of a *look*; the findings and the fixes stay behind payment (directive §12.4).

**Who builds it.** Two paths, and the choice is the directive's `GENERATE_LANDING_PAGE` toggle:
- **Toggle ON** → the cloud agent builds it as unit **N5** under directive **§3C**, in two steps: it **authors the design system for that business first** (`demo/design-system.md`, step N5a — derived from the business's own brand cues and trade), then **builds the page from it** (`demo/index.html`, step N5b). Both ship inside `Deliverables.zip`. **You still deploy it** — the sandbox does not publish, so the dossier reads `demo_url: PENDING-OPERATOR-DEPLOY` until you put it live. Both files are **zip-only, never pushed to GitHub** (the page carries the business's contact details and is an unsolicited build).
- **Toggle OFF** → you build it, from a per-trade template, using the table below.

| Decision | Setting |
|---|---|
| Where it lives | `demo.<yourdomain>.com/<slug>` — a subdomain you control |
| Never | Their domain. Never imply they own it. Ownership transfers on payment (`client-objections.md` N12) |
| Scope | **One page.** Homepage only: hero, services, reviews, photos, hours, click-to-call, map. The remaining pages are the paid work |
| Content source | The dossier (Maps facts, real review text, real services) — never invented reviews or services |
| Cost | ~€2 per mockup if generated with a mockup tool; effectively free if you template it yourself `[S]` for the tooling cost |
| Reuse | Build **per trade**, not per business — one strong car-detailing demo is 80% of the next car-detailing demo. **With the toggle ON this changes:** the agent authors a design system **per business** (directive §3C.2), so each page is bespoke rather than a re-skin — better conversion, more work per business. Same-trade businesses will converge on similar systems, but each is authored and recorded separately. **That per-business authoring step is the real cost of the agent-built path** |
| Lifecycle | Rejected demos go in your portfolio `[S]`. You are never left holding something useless |
| Disclosure | Label it plainly as a demo/mockup in the message and on the page. **The agent-built page already carries this in its footer and is `noindex`** (directive §3C.7) |
| Indexing | Keep it out of Google. The directive mandates `<meta name="robots" content="noindex, nofollow">` — never let a demo compete with, or be mistaken for, the business's real presence |

### 1.6 The tracker

One sheet. One row per business, from sourced to paid. Minimum columns:

```
business_key | trade | city | source | contact_channel | sent_date | followup_1 | followup_2 | followup_3
| replied_date | reply_type | walkthrough_sent | meeting_booked_date | meeting_held(Y/N) | close(Y/N)
| deposit_amount | deposit_date | launch_date | care_plan(Y/N) | care_plan_mrr | addons | notes
```

`reply_type` and `meeting_held` are the two columns that tell you where you are leaking. Everything else is reporting.

**`contact_channel` comes straight from `OUTREACH_CONTACTS.md`** — the sheet's **Best channel** line is what you write here, and its links are what you actually click. The tracker is your record of what happened; the sheet is where the outreach happens.

### 1.7 Language-barrier prep (do this before the first call)

Your English is not the risk. **Hesitation, uncertain tone, and indirect language are the risk** — buyers don't adjust to those, and they read as lack of conviction in the product rather than difficulty with English `[S]`. The fix is preparation, not accent work:

1. **Overlearn your first 30 seconds.** Write three versions of the opener, say the one that your mouth forms easily — not the most formal — out loud from memory **20 times**, then 10 times the next day `[S]`. By day three it costs zero cognitive load, which frees your attention for listening.
2. **Build a phrase bank.** 20–30 practised phrases; start with 10, add 5 a week `[S]`. The eight categories are in §5.7.
3. **Rehearse the three objections you hear most** until they bore you `[S]`. Boredom is the signal that the anxiety trigger is gone.
4. **Record and review five minutes** of each call against a checklist: filler words, hedges ("I think maybe", "perhaps we could"), hesitant vs purposeful pauses, and whether your closing language was direct `[S]`. Fix one pattern per week.
5. **Accept the asymmetry.** Your written English and your scripted English are both strong. Build the funnel so the critical path runs through those, and the live call is mostly Q&A. That is exactly what §3 is for.

---

## 2. Stage 1 — Outreach (you send the agent's draft)

### 2.1 Pre-send checklist

Before a single message goes out, all of these must be true:

- [ ] `Outreach.md` passed the directive's §12B.7 gate (channel filled, real trade name, ≥2 dossier facts, no phone, no fabricated figures)
- [ ] You are working from `OUTREACH_CONTACTS.md` and sending on the channel the sheet marks as **Best channel** for that business — not on whichever link you happened to find first
- [ ] A one-page demo **actually exists** for that business (§1.5). "I built you a demo" must be true. This is the one thing you may not fake
- [ ] The demo link is live and opens on a phone
- [ ] Booking link is live with the §1.2 settings
- [ ] Payment rail tested (§1.3)
- [ ] The domain is warm and today's volume is inside the ramp
- [ ] You are not sending to a business whose key is already in `PROGRESS.md`

### 2.2 The message — message one asks permission, nothing else

**Email** (adapt; ≤150 words; no link, no price):

```
Subject: I built <Business> a homepage

Hi <First Name>,

I found <Business> on Google Maps — 4.8 stars from 63 reviews — but no website.
So anyone who wants to book you has nowhere to go, and AI assistants can't
recommend you at all.

I had a few ideas, so I put together a one-page demo of what your homepage
could look like.

Want me to show you? 20 minutes, nothing owed — you'll see exactly how it
would bring you customers.

— <Your name>
```

**DM** (≤80 words; the surface truncates, so the hook must land in line one):

```
Hi — found <Business> on Maps (4.8★, 63 reviews) but there's no website,
so customers ready to book have nowhere to go.

I put together a one-page demo of what your homepage could look like.

Want to see it? I'll walk you through it — 20 minutes, nothing owed.
```

**Why this shape works.** The hook is a specific, checkable fact about *their* listing (the rating and review count come from the dossier). The demo is the reason to reply. The ask is small and reversible ("nothing owed"), which is what converts a skeptical owner into a "sure, show me." And it is permission-first, which is the single behaviour that separates a 15–22% reply rate from a 3–4% one `[S]`.

**Never in message one:** the price, the demo link, an attachment, the words "free"/"boost your business"/"SEO"/"AI-powered", more than one CTA, "let me know when works", or any request for them to phone you. The price is a §5 event; the link is a §3 event.

### 2.3 Subject lines (email only)

≤55 characters, real trade name, curiosity gap, no caps, no exclamation marks.

- `I built <Business> a homepage`
- `Question about <Business>'s website`
- `<Business> — made you something`
- `Your Maps page has 63 reviews and no site`

### 2.4 Sending discipline

| Rule | Value |
|---|---|
| Volume | Inside the §1.1 ramp; **50/day/inbox max**, 20–30 is the sane operating rate `[S]` |
| Cohort size | **≤50** per batch `[S]` |
| Days | Tue–Thu. Never Sat/Sun |
| Send time | Aim to **land at 6–8am recipient-local**. For US Eastern that is roughly **1–3pm Cairo** — you are 7 hours ahead for most of the year. Do not send at 9am Cairo (2am in New York) |
| From | Your real name, a real inbox you actually read |
| Threading | Same thread for all follow-ups |

### 2.5 Follow-up cadence

Three follow-ups, then stop. **93% of replies arrive by day 10** `[S]`, and cumulative reply rate roughly **doubles** between the first send and the third follow-up `[S]`.

| Touch | Day | Content — never "just bumping this" |
|---|---|---|
| 1 | 0 | The permission ask (§2.2) |
| 2 | 3 | **One new fact.** "One more thing — when someone asks an AI assistant for a <trade> in <city>, <Business> doesn't come up. That's the part the demo fixes." |
| 3 | 7 | **Offer the async path.** "The demo's built and ready whenever. Want the 3-minute walkthrough instead of a call? Same thing, watch it whenever." |
| 4 | 14 | **Graceful close.** "I'll stop here so I'm not cluttering your inbox. If you ever want to see the demo, it's made — just reply." |

That fourth touch gets replies more often than it should. Send it.

### 2.6 Replies you will get, and exactly what to do

| They say | What it means | Your move | Script |
|---|---|---|---|
| "Sure, send it" / "I'd like to see it" | Permission granted | Send the walkthrough (§3) + two specific times | "Great — here's the 3-minute walkthrough: <link>. If it's easier, I can walk you through it live: Thursday 6pm or Friday 7pm your time?" |
| **"How much?"** | Price before value — the trap | **Do not give a number.** Reframe to the meeting | "Depends how many services and pages you need — I'd rather not guess. Let me show you the demo and give you the exact number on a 20-minute call. Does <day> work?" |
| "Just send me the link" | Wants no commitment | Try once to convert, then **send it anyway** | "I can. It's built to be walked through, so 20 minutes gets you a lot more — but if you'd rather just look: <link>. I'll check back in two days either way." |
| "Not interested" | Closed door | Thank them in one line, stop, log it | "No problem at all — thanks for the reply. If it ever changes, the demo's here." → `client-objections.md` **U6** if you want the full branch |
| "Who are you? How did you get my info?" | Trust, not rejection | Short, specific, un-defensive | How you found them (public Maps listing), what you do, that the demo costs nothing → **U4** |
| "I need to think about it" | Almost never about thinking | Isolate the real concern; book the next step → **U2** | See §6.4 |
| "I already have someone / my nephew does it" | Not a hard no | → **W2**, **W13** | |
| "Take me off your list" | Opt-out | **Remove the same day.** CAN-SPAM requires honoring opt-outs within 10 business days `[S]` — do it immediately, log it, never re-approach | No reply needed |
| **"Just call me"** | Channel preference | **Do not phone them** — the directive's phone policy (§3B.3, §18B point 3) bans all calling; phones are captured as a **secondary** channel only. And a voice call cannot show the demo anyway | "I'm set up for video, not phone — and the demo needs a screen to make sense. Want the 3-minute walkthrough instead, or a 20-minute video call?" → **N11** for the full branch |
| Silence after 4 touches | Dead for now | Mark dead. Do not re-approach for 6 months | — |


**On the "just call me" case:** the directive's phone policy bans calling outright — *never call, always capture, never primary* (directive §3B.3, §18B point 3). So the answer is never a phone call. Steer to a scheduled **video** meeting, or to WhatsApp/Telegram, which is now an allowed **secondary** channel. Screen-sharing the demo is the entire product of the call, so a voice call converts your best asset into a verbal description of a website — the weakest possible version of your pitch.

### 2.7 Stopping rules

- **3 follow-ups maximum.** A fourth is harassment.
- **One re-approach after a "no"** is acceptable at 6+ months with a genuinely new reason. A second one is not.
- Never re-send a message you already sent.
- A hard opt-out is permanent, across every channel.

---

## 3. Stage 2 — The walkthrough (recorded, then live)

### 3.1 Why recorded first

Three reasons, in order of importance:

1. **It takes your spoken English off the critical path.** You record with a script, retake until it's clean, and they never know it wasn't the first attempt. This is the single highest-leverage fix for the language problem — you are not managing it in the moment, you are managing it once, offline, with unlimited retakes.
2. **It's watchable on their phone between jobs.** A link they can open in 30 seconds beats a calendar slot they have to keep.
3. **It qualifies them for you.** If they watch 3 minutes and reply, the meeting is warm. If they don't watch, you saved 20 minutes of your life.

The live meeting is still the closer (§5) — the recording is what earns the meeting, not what replaces it.

### 3.2 Length and chapters

**Target 2:30–3:30.** Cold outreach videos are 60–90 seconds `[S]`; 3–5 minutes is the absolute cap, and watch-through collapses below 30% beyond it `[S]`. A demo walkthrough needs the longer end — but not a second more than 3:30.

Give them the chapter timestamps in the message. It signals "this is short and structured" before they click, which is what gets the click:

```
0:12 — your homepage
0:45 — services + reviews
1:30 — how customers book you
2:20 — what's left to do
```

### 3.3 The script — six beats

Write it out. Say it out loud. Retake until it's clean. **Pause instead of saying "um."**

| Time | Beat | What you say |
|---|---|---|
| **0:00–0:20** | Open | "Hi <First Name> — <Your name> here. I build websites for <trade> businesses. I came across <Business> on Google Maps, saw your <rating> stars and <N> reviews, and noticed you don't have a website yet — so I put together a quick demo of what one could look like for you. Give me three minutes." |
| **0:20–0:40** | The absence, once | "Right now, someone who finds you on Maps has nowhere to go to see your services or book you. And AI assistants can't recommend a business with no site — so a competitor gets picked instead. That's the gap this fills." |
| **0:40–1:40** | The homepage | Scroll the hero → services. "This is your business, not a template — <specific service from dossier>, <second specific service>, your hours, your area. <Point at something real: a review quote, a photo>." |
| **1:40–2:20** | Trust | Reviews section: "Your <rating> stars are front and centre — that's the first thing a customer looks for." Photos, service area, hours. |
| **2:20–3:00** | The conversion path | Click-to-call button, the booking path, the map. Then resize the window or switch to phone view: "This is what it looks like on a phone, which is where most of your customers will see it." |
| **3:00–3:30** | Close | "This is just the homepage — a demo, nothing's live and nothing's owed. If you like it, the rest is services pages, a booking page, and the Google setup so you actually get found. Want me to walk you through it live? I have Thursday at 6 or Friday at 7 — either work?" |

**The phone-view beat is not optional.** Most local customers search on a phone, and showing it working on a phone is the most persuasive 15 seconds in the video.

### 3.4 How to send it

- **Clickable thumbnail linking to the video page — never an attachment.** Gmail caps attachments at 25MB and Outlook at 20MB, and large attachments trip spam filters `[S]`.
- Include the chapter timestamps (above).
- **Two specific times, never "let me know when works"** — a specific ask converts at 2–3x an open-ended one `[S]`.
- Keep the rest of the message plain text, one link only.

```
Here's the 3-minute walkthrough: <thumbnail link>

0:12 — your homepage
0:45 — services + reviews
1:30 — how customers book you
2:20 — what's left to do

Easier if I walk you through it live? Thursday 6pm or Friday 7pm your time —
either works for me.
```

### 3.5 Recording checklist

- [ ] Quiet room, door shut, phone silenced
- [ ] Share **the browser tab**, not your whole desktop
- [ ] Demo tab at **110–125% zoom** so text is legible on a phone
- [ ] Bookmarks bar hidden; no other tabs, no notifications, no client PII on screen
- [ ] No background music
- [ ] Speak ~10% slower than feels natural
- [ ] Retake the opener until it's clean — that is the only beat that must be perfect
- [ ] **Reuse per trade:** record the 0:40–3:30 body once per trade, and re-record only the 0:00–0:40 opener per business. That turns a 15-minute job into a 2-minute job

---

## 4. Stage 3 — Booking the meeting

### 4.1 How long should the meeting be? — 20 minutes

This was your specific question, and the honest answer is that **duration is not the lever — but it is a lever, and 20 is the number.**

**What the data actually says:**

- Gong analysed **30,000** account-executive first calls and found **no statistically significant correlation between the length of a first call and the likelihood of getting a second meeting** `[S]`. So "should it be 30 or 60?" is largely the wrong question — structure is what determines the outcome `[S]`.
- **But slot length affects whether they turn up at all:** you are **12% more likely** to get a prospect to show up to a 30-minute slot than a 60-minute one, and a 60-minute meeting is harder to sell in the first place `[S]`.
- **Deal size decides the right length:** for average contract values **below $15K**, a **tight 20-minute call with a strong qualifier outperforms a meandering hour** `[S]`. Your build is $1,200. You are far below that line.
- **Longer is not better at the top end:** across 198 analysed demos, SaaS demos averaged 45 minutes and advanced 67% of the time, while healthcare demos averaged 60 minutes and advanced only **33%** `[S]`. The longer calls had roughly half the advancement rate.
- Discovery calls in practice run **20–45 minutes** `[S]`.

**Verdict: book 20, plan 18, hard-stop at 20.**

Not 15 — 15 doesn't leave room for both a demo and a close, and you'll feel rushed, which is the worst possible state for your spoken English. Not 30 — it's easier to decline and you'll fill it. Not 60 — actively harmful per the Demodesk data, and it signals "big scary sales process" to an owner who agreed to a quick look.

**The 20-minute clock** (this is §5's spine):

| Clock | Block | Minutes |
|---|---|---|
| 0:00–1:30 | Open + the language line | 1.5 |
| 1:30–4:00 | Agenda, hard stop, one qualifying question | 2.5 |
| 4:00–7:00 | Discovery — four questions | 3 |
| 7:00–13:00 | Screen-share the demo | 6 |
| 13:00–15:30 | Price + deposit + what's included | 2.5 |
| 15:30–20:00 | Close — next steps, payment link | 4.5 |

The closing block is ~22% of the call. That ratio is deliberate: successful reps spend **12.7% more time discussing next steps** than unsuccessful ones `[S]`, and the standard advice is to reserve **7–9 minutes of a 30–45 minute call** for next steps `[S]`. Same proportion, smaller call.

**One exception:** if they're engaged and asking real questions at 20:00, keep going. The hard stop is a floor for ending a dead call, not a ceiling on a live one.

### 4.2 When to book it — the timezone problem, solved

Two data points to respect:

- Scheduling at **4pm rather than 8am increases show-up rates by ~30%** `[S]`.
- **Weekend-scheduled calls no-show at roughly 4x** the weekday rate `[S]`. Never offer Saturday or Sunday.

The problem: **you are ~7 hours ahead of US Eastern time.** Their ideal 4pm is your 11pm. Below is the honest trade-off — the table shows *their* local time (US Eastern) against your clock in Cairo.

| Their time (ET) | Your time (Cairo) | Verdict |
|---|---|---|
| 8:00am | 3:00pm | Workable — but the measured worst slot |
| 9:00am | 4:00pm | Good |
| 10:00am | 5:00pm | Good |
| **11:00am** | **6:00pm** | **Best compromise — offer this** |
| **12:00pm** | **7:00pm** | **Best compromise — offer this** |
| 1:00pm | 8:00pm | Good |
| 2:00pm | 9:00pm | Late |
| 3:00pm | 10:00pm | Too late |
| 4:00pm | 11:00pm | Their optimum, but not workable for you |

**My recommendation: offer 11am and 12pm their time — 6pm and 7pm yours.** You give up an unknown slice of the 4pm premium (Gong measured 4pm vs 8am; nobody measured the 11am–1pm band) in exchange for running the call at your best hour, in your strongest state. **This is a judgement call, and I'm flagging it as one:** a fatigued 11pm call with degraded English and a 5% higher show rate is a worse trade than a sharp 6pm call. If you ever test it and the 4pm slot converts materially better, the data wins and you change your mind.

**Time-zone mechanics:** Egypt is UTC+3 in summer and UTC+2 in winter; US Eastern is UTC−4/UTC−5. That's **7 hours for most of the year**, dropping to 6 during the brief late-October/early-November window when Egypt has left daylight saving and the US hasn't. Let the booking tool handle it — but confirm the slot in *their* timezone in every message, never yours.

**Other US timezones:** Central is 1 hour behind Eastern, Mountain 2, Pacific 3. A Pacific prospect's 11am is your 9pm. **Prefer Eastern and Central time zones when sourcing.** This is worth feeding back into the directive's §3B sourcing — a West Coast prospect costs you an hour of your evening for the same $1,200.

**Once `TARGET_COUNTRIES` is widened past the US (§3.5), the table above stops covering you.** The directive now sources only from high-income markets, and your allow-list may include GB/IE, AU/NZ, SG, or the Gulf/EU Tier-2 set — each with its own offset from Cairo (UTC+3 in summer, UTC+2 in winter). The principle is unchanged everywhere — *find their mid-morning-to-early-afternoon band and price what it costs you in the evening* — but the arithmetic is not:

| Market | Offset from Cairo | What it means for you |
|---|---|---|
| **GB / IE** | **~2 hours behind** | A 4pm London call is your 6pm. **The ET problem largely disappears — the single easiest non-US market to run.** |
| **Gulf (AE / QA / SA)** | **≈ your own clock** (Dubai +1; Riyadh/Doha same) | Their business day *is* your business day. Trivially easy on time — but cold English outreach converts worse there than in an English-first market. |
| **Singapore** | 5–6 hours ahead | Their afternoon is your late afternoon/evening. Workable. |
| **AU / NZ** | **7–9 hours ahead** (Sydney; NZ up to ~11) | Their business hours land in your **early morning** — it inverts the problem rather than solving it. Only worth it if the market pays enough to justify the alarm clock. |

Among equally-payable markets, prefer the ones whose working day overlaps your evening — that ordering, not convenience, is what §3.5 is for: **every market on the list can pay; they are not equally pleasant to sell into.**

### 4.3 The booking ask

Two specific times, never an open question — a specific ask converts at 2–3x an open-ended one `[S]`.

```
Easier if I walk you through it live? I have Thursday at 6pm or Friday at 7pm
your time — either works for me. Here's my calendar if neither does: <link>
```

Then, when they pick one: **send the invite while you're still in the conversation.** Every minute between "yes" and the invite is a minute for it to die.

### 4.4 The agenda — send it 24 hours before


Share an agenda **24 hours ahead** `[S]`. It raises show rate and it lowers your language risk, because it makes the call a walkthrough of a known list instead of an open field.

```
Subject: Tomorrow, 6pm — what we'll cover

Hi <First Name> — 20 minutes tomorrow, here's the plan so you know what
you're getting:

1. Quick look at the demo homepage I built for <Business>
2. What it would take to make it live (and what it costs)
3. Anything you want to change

Worth thinking about beforehand: how do most of your customers find you
today? That's the part the site is built to improve.

I'll keep it to 20 minutes. If anything comes up, reschedule here: <link>
```

### 4.5 The confirmation sequence — the highest-ROI 20 minutes of work in this file

**20–40% of booked sales meetings no-show** `[S]`. For cold outbound, a **65% show rate is acceptable** and **70–80% is good**; anything below 60% is a systems problem, not a market problem `[S]`.

A **three-touch confirmation sequence — instant, T-24h, T-1h — moves show rates from the 55–65% range into the 80s** `[S]`, worth **+12–20 points** on its own `[S]`. It is described as the single highest-ROI fix available `[S]`.

| Touch | When | What it says |
|---|---|---|
| 1 — Instant | Within 60 seconds of booking | Calendar invite **plus** a plain-text email from your real address. Three-bullet agenda, one line on what to think about. |
| 2 — Value re-frame | T-24h | **Not** "just confirming." Send one specific, relevant thing — the demo link, a chapter timestamp, or a fact about their listing. This is the touch that turns a polite yes into a real yes `[S]`. |
| 3 — Friction removal | T-1h | One line, mobile-readable, one-tap join link **and** one-tap reschedule link. |

**Supporting rules:**

- **Cap the booking window at 5 business days** `[S]`. Meetings booked 8+ days out no-show at roughly **double** the rate of those booked within 48 hours `[S]`.
- **Verify the email at the moment of booking** `[S]` — not in a quarterly cleanup. Ask for a mobile number in the confirmation questions as a backstop.
- Every touch from a human name, never `no-reply@` `[S]`.
- Vary the channel where you legitimately can — email for touches 1–2, a different surface for 3–4 `[S]`.

### 4.6 When they don't show

1. **T+5 minutes — message while the block is still hot** `[S]`. A message sent within five minutes of the missed slot recovers a meaningful share on the spot `[S]`.

```
<First Name> — looks like we missed each other. No problem. Want to try
again now, or should I send the walkthrough instead? <reschedule link>
```

2. **T+24 hours — the graceful out.** Two specific alternative slots plus explicit permission to decline `[S]`.

```
No worries if now isn't the time — I'll leave it here. If you want to pick
it up, Thursday 6pm or Friday 7pm your time. And if it's a no, just say so
and I'll stop emailing.
```

3. **One-click reschedule in every message.** It converts **~30% of would-be no-shows** `[S]`.

**What I would not do here:** charge a deposit or a paid consult to force attendance. It lifts show rates 25–40 points but "slashes booking volume" `[S]` — correct for high-ticket consulting, wrong for a $1,200 build you're trying to get in front of people.

---

## 5. Stage 4 — Running the 20 minutes

### 5.1 The clock, again — with the exit criteria

| Clock | Block | Exit criterion — do not leave the block without it |
|---|---|---|
| 0:00–1:30 | Open + language line | They know the plan and that it's 20 minutes |
| 1:30–4:00 | Agenda + hard stop + qualifying question | You know how customers find them today |
| 4:00–7:00 | Discovery — four questions | You know what "success" means to them |
| 7:00–13:00 | Demo screen-share | They've said something positive out loud |
| 13:00–15:30 | Price + deposit | The number has been said, once, and not apologised for |
| 15:30–20:00 | Close | Payment link sent, or a specific next step with a date |

### 5.2 The open (0:00–1:30)

**Say the language line once, early, confidently, and then never again.** Framing it as a courtesy rather than a confession is the whole trick:

> "Before we start — English isn't my first language, so if anything I say isn't clear, just stop me and I'll say it again. I'd rather be clear than fast."

Then move on immediately. **Never apologise twice** — the research is blunt about this: what buyers do not adjust to is hesitation, uncertainty in tone, and indirect language, because those signal lack of conviction in the product rather than difficulty with English `[S]`. One acknowledgement is professionalism. Two is a warning sign.

Then hand them the shape of the call:

> "I've got 20 minutes. My plan: show you the demo, tell you exactly what it costs, and answer anything you want. If you've got a hard stop, tell me now and I'll fit it."

**Asking about the hard stop is not politeness** — it prevents the call being cut off at the exact moment you're asking for money.

### 5.3 The qualifying question (1:30–4:00)

One question, and it does a lot of work:

> "Quick one before I show you — how do most of your customers find you today?"

Their answer is your entire pitch frame for the next 15 minutes. "Word of mouth" → the demo is about being findable. "Facebook" → the demo is about owning something instead of renting reach. "Referrals" → the demo is about what happens when a referral googles them and finds nothing.

### 5.4 Discovery — four questions, three minutes (4:00–7:00)

Do not interrogate. Ask these four, in this order, and listen more than you talk. Don't ask anything you could have researched — asking an owner to explain what you could have read on their Maps listing is the fastest way to lose them `[S]`.

1. **"How do most customers find you today — and roughly how many enquiries a week is that?"** *(volume — makes the money math concrete later)*
2. **"When someone gets your name from a friend, what do they find if they search for you?"** *(the absence, in their own words — this is the one that lands)*
3. **"What's the average job worth to you?"** *(needed for §6.1's payback line; ask it casually, as curiosity, not qualification)*
4. **"If this works, what does that look like in six months?"** *(makes them say the outcome aloud — they will hold themselves to it)*

**What not to do:** don't feature-dump, don't over-sell, and don't close here. Discovery is not the time to close, and over-selling early creates resistance `[S]`.

### 5.5 The demo (7:00–13:00) — six minutes, in this order

Share the tab. **Point at things rather than narrating them** — pointing does the work your English would otherwise have to do.

| Order | Show | Say |
|---|---|---|
| 1 | Hero | "<Business>, <trade>, <city>. Clean and simple — first thing a customer sees." |
| 2 | Services | "<service one>, <service two> — the things people actually call you about." |
| 3 | Reviews | "Your <rating> stars are right here. That's what closes the decision." |
| 4 | Click-to-call + booking | "One tap and their phone dials you. No form, no thinking." |
| 5 | **Phone view** | "And this is the phone version — that's where almost all your customers will see it." |
| 6 | Search / AI visibility | "This structure is what lets Google and AI assistants actually read your business — right now there's nothing for them to read." |

**Talk ratio: aim for 43% you, 57% them** `[S]`. The practical way to hit it in a second language: **after every three sentences you say, ask one question.** Pause after questions instead of filling the silence. If they're quiet, ask "does that look about right?" — it's one word of English and it hands them the floor.

**If they go quiet or look unimpressed:** stop showing and ask. "What would you change about it?" An owner who criticises the design is an owner who's already imagining owning it. That's a buying signal, not an objection.

### 5.6 Price and deposit (13:00–15:30)

Say the number **once**, clearly, and then stop talking. Do not soften it, do not apologise, do not stack justifications. Script in §6.1.

### 5.7 The close (15:30–20:00)

Reserve this block and protect it. Scripts in §6.2–§6.5.

### 5.8 The language playbook

Your preparation, from §1.7, cashed in. The eight phrase categories are your working vocabulary when the conversation goes off-script `[S]`:

| Situation | Say this |
|---|---|
| Buying time to think | "That's a fair question — let me make sure I answer it properly." |
| They raise an objection | "I hear you. Before I respond, can I ask you something?" |
| Need to park something | "Let me set that aside for a second and come back to it." |
| Confirming you understood | "So if I'm hearing you right, the main concern is..." |
| Moving to next steps | "Here's what I'd suggest we do..." |
| Checking alignment | "Does that make sense so far?" |
| Asking for the decision | "What would need to be true for this to be a clear yes?" |
| Handling silence | "Take your time — I want to make sure I've given you a complete picture." |

**When you genuinely don't catch something — the recovery line:**

> "Say that once more for me?"

Then **repeat back the part you did catch**: *"You're asking whether it works on phones — yes, and let me show you."* This is the single most important habit in the whole playbook. It proves you were listening even when you missed a word, and it converts a comprehension gap into evidence of attention. What kills credibility is not "say that again" — it's a long hesitant pause filled with filler `[S]`.

**Match their energy** `[S]`: if they're fast and clipped, shorten your sentences and cut the hedging. If they're slow and deliberate, slow down and let silences sit. What to strip out entirely: "I think maybe", "perhaps we could", "I'm not sure but", and filler words `[S]`.

### 5.9 Interruptions and variants

| Situation | What to do |
|---|---|
| They join from a truck or a noisy site | "Sounds like you're out on a job — want me to send the walkthrough and we do 20 minutes when you're back?" Do not push through; a distracted prospect doesn't buy |
| They're 5+ minutes late | Run it, but skip discovery and go straight to the demo. Or reschedule to a specific new slot |
| A partner/spouse joins unannounced | Welcome them, re-do the 40-second absence pitch, then continue. Do **not** restart from zero — and read `client-objections.md` **U3** before the call so you're ready |
| "Just email me the price" | "I'll send it right after this — let me show you the demo first so the number makes sense." Then actually email it **within the hour** |
| They ask something you can't answer | "I don't want to guess — let me confirm and email you today." Never improvise a fact. Then do it within the hour |
| They start negotiating | §6 + `client-objections.md` **U1** (price) and **U11** (cheaper competitor) |
| Tech failure on your side | "That's my fault, not yours — I'll send the walkthrough now and we'll talk <specific day>." Send it within 5 minutes |
| They say "I need to think about it" | §6.4. Isolate the real concern and leave with a date |


### 5.10 After the call — the summary email, within one hour

Send it while the conversation is still warm. It does three jobs: it restates the value without you having to speak it, it puts the price and the payment link in writing, and it creates a written record of the next step.

```
Subject: <Business> — recap + next step

Hi <First Name>,

Thanks for the time. Quick recap:

What we looked at: your homepage demo — hero, services, your 4.8★ reviews,
one-tap calling, and the phone version.

What it would take: the full site (homepage + services page + booking page
+ Google setup), live in about a week — $1,200, half to start.

Next step: <the specific thing agreed, with a date>.

Here's the payment link if you want to start now: <link>

— <Your name>
```

**Every call ends with a date.** Not "I'll wait to hear from you" — a specific day and a specific action.

---

## 6. Stage 5 — The close

### 6.1 Presenting the price (13:00 on the clock)

**Say it once, clearly, then stop talking.** The whole script:

> "So here's everything, no surprises. The full site — your homepage plus a services page and a booking page, and the Google setup so you actually get found — is **$1,200**. Half to start, the rest when it's live. It takes about a week."

Then **silence**. Let them speak first. In a second language, silence feels unbearable — sit in it anyway. Count to five in your head. If it becomes genuinely awkward, use the shortest possible hand-off: *"What do you think?"*

**Rules for this moment:**

- **One price, one thing.** No tiers, no "report-only" option, no ranges, no dashes between the offer and the number (directive §12B.4/§12B.7). A menu invites comparison; a single number invites a decision.
- **Do not apologise for the price.** No "I know it's a lot", no "unfortunately", no nervous laugh. The price is the price.
- **Do not stack justifications before they object.** Justifying an unraised objection tells them there's something to object to.
- **If you got their average job value in discovery (§5.4 Q3), use the payback line once:** *"At <$X> a job, this pays for itself with <N> jobs."* An ROI reframe outperforms opening with a discount by more than 2x (the sourced numbers are in `client-objections.md` §3.5 — that's the same research base, not a second claim).
- **Never discount.** A discount on the same scope tells them the original number was invented. If the budget genuinely isn't there, cut the *scope* (homepage only, no booking page) — a smaller thing at a smaller price is a different offer, not a concession. That distinction is a judgement call I'd defend, but it's yours to overrule.

### 6.2 The deposit

**For a project between $500 and $2,500, the standard deposit is 50% upfront** `[S]`. Your $1,200 build → **$600 to start, $600 on launch.**

A deposit is the single most effective protection against non-payment and clients who ghost after you've done the work `[S]`. The clause that matters: *non-refundable, credited against the final invoice, and work does not begin until it has been received* `[S]`.

> "Half now to lock the date — $600 — and the other $600 when it goes live. The deposit covers the build time."

**The four deposit pushbacks, and the answers** `[S]`:

| They say | You say |
|---|---|
| "We don't pay deposits." | "I understand. I ask for it to reserve the time and start the setup. If your policy really doesn't allow it, I can do a milestone schedule — first payment when I show you the first draft." |
| "Can you start while the payment clears?" | "I'll reserve the date, but I begin once it clears — usually a day or two." Hold this line. A client who pushes on payment pushes elsewhere too `[S]` |
| "Can we pay everything at the end?" | "On a small job I would. On this one I ask for half up front to cover the build time, and the rest on delivery." |
| "Can the deposit be refundable?" | "It secures your slot and covers the setup. If you cancel before I start, I refund it minus a small cancellation fee." |

Keep the agreement to **one page**: scope, what's excluded, response time, rollover, billing, cancellation `[S]`. Do not over-engineer this — you are not building a legal fortress for $1,200, you are creating a written record of what was agreed.

### 6.3 Taking the money — on the call, not after

This is the highest-value behaviour in the entire file.

- **20–35% of verbal commitments never convert to payment when collection happens after the call ends** `[S]`. The longer the gap between "yes" and payment, the higher the drop-off `[S]`.
- **Teams that collect payment on-call report 40–60% higher conversion from verbal yes to actual revenue** than teams that invoice afterwards `[S]`.

**The mechanics:**

1. **Send the link in the meeting chat while you're still on the call.** Payoneer payment request (§1.3).
2. **Stay on the call while they pay.** Do not hang up and wait for an email.
3. **Never read card numbers aloud** — use the hosted checkout so card details never touch you or the call `[S]`.
4. **It must work on a phone browser** — many people join from their phone `[S]`.
5. **You tested this flow once already (§1.3).** Do not discover a broken checkout in front of a paying client.

> "I'll drop the link in the chat now — it's a $600 deposit to start. I'll stay on while you do it, and if anything looks odd just tell me."

Payment clears in seconds `[S]`. **The moment it does, say what happens next, with a date:**

> "Got it — you'll have an email from me within the hour with the five things I need from you, and I start tomorrow."

**If they can't pay right then** (card isn't with them, partner holds it) — do not let it drift. Book the specific finish:

> "No problem. When works for you — Thursday at 6? I'll send a fresh link and we'll finish it in two minutes."

Then send the link at that time. A "yes" without a scheduled next step is not a yes.

### 6.4 "I need to think about it" — on the call

Do not argue, do not repeat the pitch, do not offer a discount. **Isolate the real concern**, because this phrase is almost never about thinking (full branch tree in `client-objections.md` **U2**).

> "Of course. Usually when someone says that it's one of three things — the price, the timing, or you want to run it past someone. Which one is it for you?"

Then route:

| Their answer | Route |
|---|---|
| Price | `client-objections.md` **U1** — and use the §6.1 payback line, never a discount |
| Timing / "next year" | **U7**, **N8** |
| "I need to check with my wife/partner" | **U3** — see below |
| "I'm not sure it'll work for my trade" | **U8**, **N6**, **N15** |
| "I've been burned before" | **U13** |

**The partner branch deserves its own script** because it's the most common real reason and the easiest to mishandle:

> "That makes sense — most people I work with check with someone. What would they want to know? … I'll put it in two lines you can forward, and let's talk Thursday at 6 so I can answer whatever they come back with."

Then **actually send the two lines within the hour**, and **actually book Thursday.** The failure mode isn't the partner — it's leaving the call with no date.

**The one rule for this entire section: never end a call with "let me know."** Every call ends with a specific day and a specific action, or it ends with nothing.

### 6.5 When to walk away

- **They refuse any deposit.** Offer the milestone compromise once. If they still refuse, walk — clients who won't put skin in the game are statistically more likely to pay late or not at all `[S]`.
- **The budget genuinely isn't there.** Offer the reduced-scope version once (§6.1). If that's still out of reach, leave it and keep them on the follow-up list — a no today is often a yes in six months, and the demo costs you almost nothing.
- **They want you to start for free to "prove yourself."** No. That's `client-objections.md` **U15**.
- **They're rude, or they've moved the goalposts twice.** Walk. This is a $1,200 deal; the margin doesn't cover a bad client.

### 6.6 When they don't close

Three touches over 14 days, then stop. Same discipline as §2.5.

| Touch | Day | Content |
|---|---|---|
| 1 | Same day | The §5.10 summary — recap, price, next step with a date |
| 2 | 3 | **One new piece of value.** "Noticed <similar businesses> in <city> come up when people ask AI assistants for a <trade>. That's the gap." |
| 3 | 7 | **The graceful out with one last date.** "If it's a no, tell me and I'll stop. If you want it, Thursday at 6 and I'll get started." |
| 4 | 14 | "I'll stop here so I'm not cluttering your inbox. The demo stays up if you ever want it." → mark dead |

Then leave them alone for six months.

---

## 7. Stage 6 — Post-sale: deliver, then sell the care plan

The build is not the business. **The build is the door.** A $1,200 one-off is a small deal; the same client on a care plan is worth roughly **$4,200 in year one** and $3,000 every year after.

### 7.1 Onboarding — the same hour

Send one email with a numbered list. Make it trivial to answer, because the #1 way this project stalls is waiting on content.

```
Subject: <Business> — let's start (5 things I need)

Great to have you on board. To get live this week I need:

1. Your logo (or say "use the one on my van" and I'll sort it)
2. 5-10 photos — phone photos are fine
3. Your services + prices (or tell me to leave prices off)
4. Your hours + the areas you cover
5. The email on your Google Business Profile (or just say yes to me
   updating it)

Send what you have and I'll start today. Anything missing by Wednesday I'll
pull from your Google listing.
```

**The last line is the important one.** It puts a deadline on content collection without nagging, and it gives you permission to proceed rather than waiting forever.

### 7.2 Build and launch — what to send at each milestone

| Day | Milestone | What you send |
|---|---|---|
| 0 | Payment confirmed | The onboarding list + the launch date |
| 1–3 | Content collected | One line confirming what arrived and what you're using from their listing |
| 3–5 | Build | Nothing. Silence is fine — don't send progress updates nobody asked for |
| 5 | Preview | The link, and: "One round of changes included — send everything in one message and I'll do it in one pass" |
| 6–7 | Launch | "It's live: <link>. I've also updated your Google listing so it points to it" |
| 7 | Final invoice | The remaining $600 |


**On the revision round:** "one round, sent as one message" is the single sentence that prevents a five-week death-by-a-thousand-tweaks. Say it at the preview stage, not the start.

### 7.3 The add-on ladder

Pitch **one** add-on per conversation. Never a menu — a menu converts like a menu, which is to say it doesn't.

| Add-on | Price | Pitch it | Notes |
|---|---|---|---|
| **Care plan** | $250/mo entry (see §7.4) | **At handoff** | The main event. This is the one that matters |
| Extra pages | $150–250 per page | At handoff | The natural first yes; services, gallery, about |
| Booking / scheduling setup | $200–400 setup + tool cost | At handoff | High value for any trade with appointments |
| Local SEO setup (one-time) | $300–600 | At handoff | On-page, Google Business Profile, citations |
| Google Business Profile management | $100–200/mo | +30 days | Posts, review replies, photos |
| Blog / content | $150–300 per post | +30–90 days | Only if they'll actually use it — dead blogs hurt them and you |
| **AI receptionist / chat** | $149–299/mo (resold) | +30–90 days | Highest margin, needs call volume — see §7.5 |

### 7.4 The care plan — the real product

**Three tiers exist in the market** `[S]`. Be honest with yourself about which one your clients will actually buy.

| Tier | Price `[S]` | What's in it | Who it's for |
|---|---|---|---|
| **Starter** | **$200–300/mo** | CMS/plugin updates, security scan + malware monitoring, daily backups (30-day), uptime monitoring, monthly performance check, ~30 min content edits, monthly email report | Small sites that need reliability. **This is your tier for a $1,200 build client** |
| Professional | $500–750/mo | + 2 hrs design/content work, quarterly speed optimisation, monthly analytics review with one recommendation, 4 GBP posts/mo, basic on-page SEO, 24h priority | Businesses where the site is a primary lead channel |
| Growth | $1,000–1,500/mo | + 4 hrs work, 1 blog post/mo, CRO/A-B testing, monthly competitor analysis, quarterly strategy call, Search Console monitoring, same-day priority | Genuine marketing partnership |

**The judgement call:** pitch **Starter** to a one-van operator. Pitching a $750/mo Professional tier to someone who just paid $1,200 will lose you the retainer *and* look like a bait-and-switch. Starter at $250/mo is the tier that actually converts at this deal size; move a client up to Professional only after they've asked for work beyond the Starter scope.

**The pitch, at handoff** `[S]` — frame it as protecting the investment, never as "maintenance". Nobody gets excited about maintenance; everyone wants to protect a $1,200 asset:

> "Right now everything's fast, secure and up to date. In six months without anyone touching it, that drifts — plugins go stale, speed drops, things break. I look after it for $250 a month: updates, security, backups, uptime, and small changes whenever you need them. Want me to add that?"

**What the numbers actually look like** `[S]`:

- **~75% of clients take a care plan if you pitch it consistently** — but you have to ask every time `[S]`.
- Churn runs **10–15% per year** `[S]`; replace them with new builds that convert to plans.
- 10 clients at $250/mo = **$2,500/mo of recurring revenue** before you sell anything new. (The published example uses 10 × $500 = $5,000/mo `[S]` — that assumes the Professional tier, which is why §7.4's tier choice is a business-model decision, not a detail.)

### 7.5 The AI receptionist add-on

The strongest second sale for trades, and the one with a real, checkable value story.

**The evidence you can quote to a client:**

- **~1 in 3 inbound calls to local service businesses go unanswered, even during staffed hours** `[S]`
- **~80% of callers who reach voicemail won't leave a message** `[S]`
- Worked math: a business averaging **$450 per job** that misses **20 calls a month** has roughly **$9,000/month** in potential revenue at stake `[S]`

**Pricing:** small-business AI receptionists run **$149–299/mo** at the common tiers, with a wide market spread of **$25–899/mo** `[S]`. Flat monthly with an included minute pool wins once call volume passes **~80–120 calls/month**; below that, per-minute or per-conversation billing is cheaper `[S]`. That crossover is your qualification question: **"Roughly how many calls do you get a week?"** Under ~20/week, don't pitch it.

**Best-fit trades** `[S]`: HVAC, plumbing, electrical, roofing, dental, veterinary, med spas, law firms, property management, landscaping, cleaning, moving, chiropractic. **Skip** businesses where every call needs deep judgement `[S]`.

**Two ways to offer it:** resell an existing vendor at a markup (less work, you inherit their reliability risk — check that the vendor has real reviews before you put your name on it) or build a simple site chatbot (more work, no dependency). Start by reselling.

**Do not pitch this in the first sale.** It's a 30–90 day conversation, and offering it during the build reads as upselling a client who hasn't seen results yet.

### 7.6 Billing mechanics

- **Auto-charge a card on file monthly. Never invoice a retainer manually** `[S]` — the friction of sending and collecting makes you resent the arrangement, and resentment is how you start delivering badly.
- **Unused hours don't roll over** `[S]` — otherwise clients bank hours and ask for a free mini-redesign in month six.
- **30-day cancellation, no long-term contract** `[S]`. If you need a contract to keep them, the value isn't there.
- One-page agreement: scope, what's excluded, response time, rollover, billing, cancellation `[S]`.

### 7.7 The cheapest pipeline you have

At launch + 30 days, ask two things in one message:

> "Two quick things — would you leave a review on Google? It's the main way I get work. And if you know another <trade> owner who'd want the same thing, I'll look after them properly."

The referral ask costs one sentence and converts better than any cold channel in §2. The review compounds. Do it every single time.

---

## 8. Tracking and the weekly review

Columns are defined in §1.6. This section is about what you *do* with them.

### 8.1 Read the funnel in this order

Stop at the first metric that's off — everything downstream is contaminated by it.

| # | Metric | Target | If it's off |
|---|---|---|---|
| 1 | **Bounce rate** | <1% `[S]` | Stop sending. Fix SPF/DKIM/DMARC and list hygiene first. Nothing else you do matters |
| 2 | Reply rate | 3–5% avg, 5–8% good `[S]` | Under 2% with a clean bounce rate = the hook is wrong, not the list |
| 3 | Positive reply rate | 0.8–1.5% avg, 1.5–3% good `[S]` | Positive replies but no bookings = the walkthrough or the ask is wrong (§3) |
| 4 | Meeting-booked rate | 0.5–1% avg, 1–2% good `[S]` | Booked but not showing = §4.5's confirmation sequence, or the booking window |
| 5 | **Show rate** | **80%+** for this funnel (warm reply + walkthrough watched); 70–80% is good for cold outbound generally `[S]` | Below 60% is a systems problem, not a market problem `[S]` |
| 6 | Close rate on meetings held | 10–25% `[E]` at this price point | Shows but doesn't close = price presented before value, or the demo isn't landing (§5.5, §6.1) |
| 7 | **Verbal yes → deposit received** | **80%+** | Below that, you are invoicing after the call. Fix §6.3. This is the most expensive leak in the business |
| 8 | Care plan attach rate | ~75% if pitched consistently `[S]` | Low = you aren't asking (§7.4) |

### 8.2 Change one thing at a time

- **Don't touch the copy until you have ≥100 sends on the current version.** Anything less is noise.
- Change **one** element per test — the hook, or the subject, or the ask. Never two.
- The only exception to "wait for 100" is metric #1: a bad bounce rate is an emergency, not a test.
- Re-run the §0.3 model against your real numbers every 200 sends and replace the `[E]` estimates with your own. After that, this file's benchmarks become your baselines.

---

## 9. Failure modes

| Symptom | Most likely cause | Fix |
|---|---|---|
| No replies at all | Domain cold, or in spam, or a dirty list | §1.1 — check bounce first, then warm-up |
| Replies, but nobody agrees to a meeting | You asked for a call before giving value, or the walkthrough wasn't sent | §3 |
| Meetings booked, high no-show rate | Booking window too long, no confirmation sequence, or weekend slots | §4.5 |
| Meetings held, low close rate | Price presented before the demo landed, or delivered apologetically | §5.5, §6.1 |
| **Verbal yes, payment never arrives** | Invoiced after the call | **§6.3** — the single most common and most expensive failure |
| Call ends with "I'll think about it" and no date | No §6.4 isolation, no next-step block on the calendar | §6.4 — every call ends with a date |
| Project stalls for weeks | Waiting on client photos/content | §7.1 — the Wednesday line |
| Scope creep, endless tweaks | No one-page agreement, no revision limit stated | §6.2, §7.2 |
| Good builds, no recurring revenue | Care plan never pitched, or pitched at the wrong tier | §7.4 |
| You dread the calls | You're improvising in your second language | §1.7, §5.8 — script the first 30 seconds and the phrase bank |

---

## 10. Directive status — what's now applied, and what still isn't

**Updated 2026-09-24.** The operator has since amended `AUDIT_EXECUTION_DIRECTIVE.md` directly, and **two of the six items below are now APPLIED** — plus a phone-policy change that goes further than what I had proposed. Read this section as a status board, not a wish list.

### APPLIED — do not re-propose

**✅ A4 — phone policy (superseded by a bigger change than I proposed).**
I had asked for a narrow carve-out for scheduled video meetings. The operator instead replaced the phone ban with a full **PHONE POLICY** (§3B.3, §18B point 3, top banner): *never call, always capture, never primary.* Phone numbers are now **recorded in the dossier as a secondary channel** with their WhatsApp/Telegram state verified, and channel priority is fixed as **Email > Social DM > Phone-messaging**. **A phone-only business now ships** instead of being skipped. This is a better change than my proposal — it keeps the anti-call logic intact while no longer throwing away reachable contacts.
**Consequence for this file:** §2.6's "just call me" row and §3's channel assumptions are unchanged in substance (still no calls, still email/DM first), but a phone-only business is now a real prospect rather than a dead one — so the §2 follow-up cadence and the §4 booking path must be able to run over WhatsApp.

**✅ A5 — unit N5 now exists (corrected 2026-09-23).**
The operator added `GENERATE_LANDING_PAGE: ON/OFF` (§0 Controls) and a full **§3C Landing-Page Generation** spec, with N5 as the build unit, a conversion architecture, a technical file spec (`demo/index.html`, self-contained, `noindex`), and a §3C.9 quality gate.
**Correction applied 2026-09-23.** The first draft made the design system a repo-level file the agent had to *read* — `skills/landing-page-design-system/SKILL.md` — and made its absence a **session-wide blocker**. That file never existed, so the toggle was dead on arrival. The operator corrected the model: **the agent CREATES the design system, per business, as the first step**, then builds the page from it. §3C.2 is now **step N5a (author `demo/design-system.md`)**, §3C.3–§3C.7 is **step N5b (build `demo/index.html` from it)**, and there is **no external prerequisite that can block a run**. Both artifacts ship in `Deliverables.zip` and are zip-only.
**Consequence for this file:** §1.5 (the demo factory) and §3 (the walkthrough) now have an **agent-side build path** — the demo can arrive pre-built in `Deliverables.zip` instead of you building it.
**Two operational notes from that change:** the demo and its design system are **zip-only** — never pushed to GitHub, because the page carries the business's contact details and is an unsolicited build; and the page is deployed by **you**, not the sandbox, so the dossier records `demo_url: PENDING-OPERATOR-DEPLOY` until you put it live.
**Cost note (honest):** a per-business design system is *more* work per business than one shared house style would be — that is the price of each demo looking bespoke rather than re-skinned. Same-trade businesses will converge on similar systems, but each is authored and recorded separately.

**✅ A7 — the session contact sheet (operator-requested, 2026-09-24).**
The operator asked for full business-info collection in **both** modes, and for a single per-session file holding every target's reachable channels as clickable links. Applied as directive **§3.6** (the contact-hunt is now a **fixed policy in both `with_website` and `no_website`** — every email, every phone, every DM-able social, not just what the site shows) and **§3.7** (`OUTREACH_CONTACTS.md`, the click-to-contact sheet at the zip root, with verified per-platform DM deep links). The agent must **read the sheet back and verify it** (§3.7.3) before the run continues.
**Consequence for this file:** §0.1 and §2.1 now point at the sheet as the starting point for every outreach session — **the sheet is the route, `Outreach.md` is the message.** Privacy also changed: the sheet is the **second PII file** after the per-business dossiers, zip-only and never pushed.

### NOT APPLIED — still open

**A1 — §12B.4 point 4: the price is in message one.**
Current text puts `$WEBSITE_BUILD_FEE_USD` in the first email/DM. That still contradicts the whole funnel above (price is a §5/§6 event; price in message one anchors to cost before value exists `[S]`).
*Proposed:* "**Offer (1 sentence):** name the thing you built, not the price — 'I put together a one-page demo of what your homepage could look like.' The price is presented at the walkthrough, never in the first message."

**A2 — §12B.4 point 5: the CTA. (Partially resolved by the toggle.)**
The directive still defaults to the deferred-mockup wording. **But** it now explicitly permits the stronger CTA when `GENERATE_LANDING_PAGE: ON` — *"Reply and I'll show you the homepage I built for `<Business>`"* — which is the variant §2.2 and §3 assume. So the conflict now only bites when the toggle is **OFF**, and the cleanest fix is to make the toggle-ON wording the default.

**A3 — §12B.7 quality gate and §18B point 4: "single build price" in the outreach.**
Still requires the price to appear in `Outreach.md`.
*Proposed:* change "Offer is SINGLE: new website build at `$WEBSITE_BUILD_FEE_USD`" → "Offer is SINGLE and stated without a price: the demo walkthrough. The single price is presented at the walkthrough, not in the first message."

**A6 — §16B: the boundary is unstated.**
*Proposed addition:* "Everything after `Outreach.md` — sending, replies, booking, the meeting, the close, delivery, and post-sale — is operator work, documented in `SALES_WORKFLOW.md`. It is out of scope for the agent run and does not affect §16B."

### One dependency you still owe yourself

**Resolved 2026-09-23 — there is no dependency.** The earlier note here flagged `skills/landing-page-design-system/SKILL.md` as a missing blocking prerequisite. That framing was wrong and has been removed: the design system is **authored by the agent, per business, in-run** (§3C.2, step N5a), so nothing external has to exist before `GENERATE_LANDING_PAGE` can be turned ON. The toggle stays defaulted to **OFF** only to keep sessions lean until the demo funnel is in use — flip it on whenever you want pages built.

**Note on the other mode:** §4, §5 and §6 apply unchanged to the `with_website` redesign close (§12.4R) — same 20-minute meeting, same 43/57 talk ratio, same on-call payment. Only §2 and §3 differ: you pitch the audit-then-rebuild sequence instead of a demo homepage, and the walkthrough walks through their *existing* site's defects rather than a mockup.

---

## 11. Quick reference card


Keep this open during calls.

**The funnel:** demo built → permission ask (no price, no link) → 3-min walkthrough → **20-minute** meeting → one price → **payment link on the call** → care plan at handoff.

**The 20 minutes:** 1.5 open · 2.5 agenda + qualify · 3 discovery (4 questions) · 6 demo · 2.5 price + deposit · 4.5 close.

**Numbers to hold in your head:**
- 100 sends → 3–7 replies → 1–2.5 meetings → 0.15–0.5 sales `[E]`
- 20–40% of booked meetings no-show; the 3-touch confirmation sequence takes you into the 80s `[S]`
- 20–35% of verbal yeses die if you invoice after the call; on-call payment lifts it 40–60% `[S]`
- $600 deposit now, $600 on launch; $250/mo care plan = $4,200 first-year value
- Never weekend. Never 60 minutes. Never "let me know."

**When it goes wrong on the call:**
- Don't understand → *"Say that once more for me?"* then repeat back what you caught
- Objection → *"I hear you. Before I respond, can I ask you something?"*
- "Think about it" → *"Price, timing, or you want to check with someone — which one?"*
- Then **leave with a date.**

---

## 12. Sources

Fetched and read in full during this session. Everything marked `[S]` traces to one of these.

| # | Source | What it contributed |
|---|---|---|
| 1 | [Prospeo — How Long Should a Sales Call Be? (2026 benchmarks)](https://prospeo.io/s/how-long-should-a-sales-call-be) | Call-length targets by type; the <$15K → 20-minute guidance; Demodesk's 198-meeting demo data (SaaS 45 min/67% vs healthcare 60 min/33%); Gong's 43/57 talk ratio; follow-up and closing call lengths |
| 2 | [Gong Labs — The Optimal Length for Your First Sales Call](https://www.gong.io/blog/how-long-your-first-sales-call-should-be) | 30,000 first calls: no correlation between length and next step; **30-min slot = 12% better show rate than 60-min** |
| 3 | [Tomba — How to Reduce No-Shows in Sales](https://tomba.io/blog/how-to-reduce-no-shows-in-sales) | 20–40% no-show benchmark; show-rate targets by channel; the 3-touch confirmation sequence (+12–20 pts); booking-window and 8+ day findings; one-click reschedule (~30%); T+5min recovery; deposit trade-off |
| 4 | [Prospeo — Loom Video Cold Email Strategy for 2026](https://prospeo.io/s/loom-video-cold-email) | Permission-first workflow; 15–22% vs 3–4% reply rates; video length (60–90s cold, 3–5 min cap, watch-through collapse); clickable thumbnail vs attachment; follow-up cadence; cohort size; deliverability ceilings; warm-up ramp |
| 5 | [Calendly — 11 Sales Demo Best Practices](https://calendly.com/blog/sales-demo-best-practices) | Agenda 24h before; reserve 7–9 minutes for next steps; book the next meeting before the call ends; Gong Labs' 12.7% more time on next steps |
| 6 | [Cynthia Concierge — How to Collect Payment on a Video Call](https://cynthiaconcierge.com/blog/collect-payment-video-call/) | 20–35% of verbal commitments lost post-call; on-call collection = 40–60% higher conversion; never read card numbers; mobile compatibility; test the flow |
| 7 | [Reapify — How Web Designers Build $5K+ Monthly Retainers](https://reapify.io/blog/web-design-retainers-recurring-revenue) | Three retainer tiers with prices; why sites decay; pitch at proposal/handoff and frame as protecting the investment; ~75% attach rate; 10–15% churn; billing and agreement rules |
| 8 | [DojoSales — Confident Sales Calls in Your Second Language](https://dojosales.com/blog/confidence-sales-calls) | Overlearning the first 30 seconds; objection rehearsal; record-and-review checklist; energy matching; the 8-category phrase bank; what buyers don't adjust to |
| 9 | [Causo Hub — Cold Email Benchmark Report H1 2026](https://hub.causo.ai/guides/h1-2026-cold-email-benchmark-report) | Reply / positive-reply / meeting-booked / send-to-customer benchmark tables; 93% of replies by day 10; specific ask = 2–3x; personalization dosage |
| 10 | [XPay — Wise or Payoneer in Egypt](https://xpay.app/blog/wise-or-payoneer-egypt) | Stripe unavailable in Egypt, PayPal cannot pay out to Egyptian banks; Payoneer as primary receive rail; Wise as backup; effective costs; the $1,000-invoice math |
| 11 | [VantaWeb — AI Receptionist for Small Business 2026](https://vantaweb.io/ai-receptionist-for-small-business/) | AI receptionist price ranges; 1-in-3 calls unanswered; 80% of voicemail callers don't leave a message; the $9,000/month missed-call math; the 80–120 calls/month crossover; best-fit trades |
| 12 | [HubSpot — Discovery Call Questions](https://blog.hubspot.com/sales/discovery-call-questions) | The qualifying / disqualifying / next-step question structure; discovery call durations (20–45 min); the anti-patterns (redundant questions, feature-dumping, over-selling early) |
| 13 | [Contracts Kit — Freelance Deposit Clause](https://contractskit.com/blog/freelance-contract-deposit-clause-how-much-upfront) | Deposit percentages by project size ($500–2,500 → 50%); the deposit clause's three required elements; the four client pushbacks and answers; walk-away guidance |
| 14 | [FTC — CAN-SPAM Act Compliance Guide](https://www.ftc.gov/business-guidance/resources/can-spam-act-compliance-guide-business) | B2B email is covered; deceptive subject lines banned; opt-out handling (carried over from the `client-objections.md` research pass) |
| 15 | [Prospeo — Objection Handling Framework](https://prospeo.io/s/objection-handling-framework) | The 67,149-call dataset behind the ROI-reframe-vs-discount-first figures — cited here via `client-objections.md` §3.5 rather than restated |

**What is *not* sourced and should not be quoted to a client:** every `[E]` and `[C]` label. In particular the 35/60/80 staged-conversion ladder, the close-rate-per-meeting estimate in §8.1, and the worked 100-send model in §0.3. Replace them with your own numbers once you have 200 sends of real data.


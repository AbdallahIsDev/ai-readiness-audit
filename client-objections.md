# Client Objections Playbook — v2 (With-Website + No-Website)

> **What this is:** the single conversation-handling file for both target types. Every objection a local business owner can raise — and what to say back, turn by turn.

> **Channel rule:** outreach and follow-up run on **email / FB-DM / IG-DM / X-DM / Reddit-DM**. Never a phone call in `no_website` mode (§3B.3 phone ban — calls, SMS, WhatsApp). In `with_website` mode no rule forbids a call, but the same reasoning applies: cross-border cold calls read as scam. Default = keep the conversation in the channel that opened it. Every reply below is written as copy-paste-ready text.

> **Golden Rule compliance:** every framework, stat, and script pattern here was researched online against 2025–2026 practitioner sources before being written down — nothing is from assumption. Sources listed at the bottom; inline tags point to them.

---

## 0. How to use this file

### 0.1 The eight laws (read once, obey always)

1. **An objection is a buying signal, not a rejection.** A prospect who objects is still in the room. Cognism: objections "are an indicator that the prospect is interested, but doesn't yet have a full understanding." Ghosting is the failure state — objections are the opportunity.
2. **Diagnose before you prescribe.** The single biggest mistake is answering the *stated* objection instead of the *real* one (HubSpot: "The Explore step is where most reps lose deals"). Top reps respond to objections **with a question 54.3% of the time vs 31% for average reps** [S: Gong via Prospeo]. Ask first.
3. **Never answer the first sentence with a pitch.** "Too expensive" usually means *"I don't see the value yet."* "Talk to my partner" usually means *"I don't trust you yet."* Explore one beat, then respond.
4. **Reframe, don't counter.** Reframing wins **42%** of price objections; countering/discounting wins **19%** [S: Gangly, Salesforce/Gong aggregates]. Countering starts a fight you don't need.
5. **Reframe, never discount reflexively.** A reflexive discount teaches the buyer the price was padded (Objeq). Trade *structure* (phasing, 50/50), never price-for-nothing.
6. **Cap it at 2–3 objections per conversation, then move to the next step.** Deals with no scheduled next step die **85%** of the time [S: Prospeo]. You are not trying to win the argument — you are trying to earn the next turn.
7. **Objections raised early are worth 4× those raised late.** The same objection in the first 10 minutes converts at **41%**; in the last 10 minutes, **10%** [S: Gangly]. Volunteer the hard questions early ("What would stop this from being a fit?") instead of letting them surface after the pitch.
8. **Proof beats promise.** A relevant proof point cited within 30 seconds of an objection lifts close probability by **38%** [S: Gangly]. Have the screenshot/example ready before you need it.

### 0.2 The frameworks — and when to use each

| Framework | Steps | Use it when |
|---|---|---|
| **LAER** (Carew International) | **L**isten → **A**cknowledge → **E**xplore → **R**espond | **Default.** Almost every entry below is LAER with options bolted on. |
| **LAARC** | Listen → Acknowledge → **A**ssess → Respond → **C**onfirm | Higher-stakes / multi-stakeholder. The **Confirm** step ("does that fully answer it?") stops premature closes [S: Prospeo]. |
| **Feel-Felt-Found** | "I understand how you **feel** → others **felt** the same → what they **found** was…" | Emotional objections: burned before, scared, embarrassed about tech. Note: practitioners call it "training wheels" — don't use it as your only move [S: Prospeo]. |
| **Validate → Isolate → Reframe** | "Makes sense" → "If X weren't an issue, is this what you'd choose?" → reframe to cost-of-inaction | Price. The isolation question separates *real* price objections from *value* objections [S: Prospeo]. |
| **Boomerang** | Return the objection as a question | Stall/brush-off. "If it worked and it were free, would you do it?" forces the real blocker into the open. |
| **ARC** | Acknowledge → Respond → Close | Fast, low-ticket, single decision-maker — our exact deal size ($500–$1500). |
| **Diagnose–Decide–Document–Close** | Name the risk → pick a lane → confirm in writing → one dated next step | Freelancer-specific [S: gruv.ai]. Lanes: **Educate / Re-scope / Hold firm / Walk away.** |
| **4 P's** | Pause → Probe → Provide → Proceed | When you'd otherwise talk too fast. Pause **5× longer** than feels natural — top reps do [S: Prospeo]. |

**The four lanes (decide which one you're in before typing):**
- **Educate** — they lack context; current terms still work. → give the missing fact.
- **Re-scope** — they want the outcome but not at this size. → shrink the *scope*, not the price per unit.
- **Hold firm** — the request would make the deal unclear/unworkable. → politely decline, restate value.
- **Walk away** — no workable budget, authority, or timeline after honest clarification. → close the file warmly; a clean no beats a fake maybe.

### 0.3 Diagnose first — the four buckets

Every objection is one of four things (Gong/Salesforce/HubSpot all converge). Name the bucket *before* answering:

| Bucket | Sounds like | Really means | Your first move |
|---|---|---|---|
| **Budget / Price** | "too expensive", "no budget" | value not established yet | isolate: "if price weren't the issue, is this what you'd pick?" |
| **Authority** | "talk to my partner", "I'm not the guy" | not the decision-maker / not armed to sell internally | arm the champion with a 5-line summary |
| **Need / Fit** | "don't need it", "we're fine", "tried before" | weak discovery or wrong problem | ask what they'd improve about the status quo |
| **Timing** | "later", "next quarter", "too busy" | no urgency, or a real competing priority | "what changes between now and then?" |

**Frequency reality check** (so you don't over-rotate on price): price/budget is **35%** of objections, budget-timing **22%**, "already have one" **18%**, no authority **14%**, no urgency **11%**, feature gap **9%**, trust **6%** [S: Salesforce 2025 / Gong / HubSpot via Gangly]. The average deal throws **2.4 objections**, and **64%** of deals raise at least two [S: Gong 2024]. Expect a **series**, not a single gate.

**Never ask "why".** "Why do you feel that way?" triggers defensiveness. Use **"What's driving that concern?"** [S: Gong via Prospeo].

### 0.4 Response format & notation

Each objection is laid out as:

```
### <ID>. "<exact owner phrase>"
Frequency / what it really means   → the diagnosis
**Option 1 — <angle> (<personality it fits>)**: script
**Option 2 — <angle>**: script
**Option 3 — <angle>**: script
**Branch tree**  → what happens next, turn by turn
**Never say**    → the specific sentences that kill this deal
**Exit ramp**    → how to end the turn cleanly if it's genuinely dead
```

**Option selection by personality:**
- **Option 1 = direct/logical** — for the numbers-first owner.
- **Option 2 = empathic/story** — for the cautious, burned, or relationship-driven owner.
- **Option 3 = question-flip** — for the confident owner who will sell themselves if you hand them the question.

**Branch notation:**
- `⇒` = your next message. `⇐` = what they said back.
- `≈N%` = rough likelihood of that branch. `[S]` = sourced statistic; `[E]` = my estimate derived from the sourced data. Treat every `[E]` as a prior, not a fact.
- A branch tree goes **two levels deep**. Past that you're in a live conversation — return to §0.1.

### 0.5 Rules of engagement (hard — breaking these costs the deal or the client)

- **Stay short.** The outreach drafts have hard limits (email ≤150 words / DM ≤80, §12B.4). Replies inside a conversation should be shorter still: **2–4 sentences and exactly one question.** Long replies read like a brochure.
- **One ask per message.** One CTA. Never stack two questions.
- **Never send the full findings/fixes before payment** (§12.4 point 5). It makes you redundant — they'll implement the list themselves. Send a **teaser**: one screenshot, one example, one count. Never the whole report.
- **Never guarantee rankings or customer counts** (§12.7). Everyone who promises "#1 on Google" is lying and the owner has heard it before.
- **Never fabricate a number.** The only dollar figure allowed is a researched, conservative left-on-table estimate with visible reasoning and source (§12.6). No invented statistics, no fake case studies, no made-up review counts.
- **Never badmouth** the nephew, the current web guy, the incumbent agency, or a competitor. It makes the owner defensive and it's the fastest way to lose a warm lead (Cognism: "don't badmouth your competitors" — it may get back to them and it offends the buyer who likes them).
- **Never hard-close a live lead.** Even a "no" gets a graceful exit and a future callback — goodwill refers business.
- **Never argue twice about the same thing.** If they repeat an objection you already answered, that's a **firm no** on that point (HubSpot: "if a prospect raises the same objection twice, treat it as real"). Accept it, pivot once, then exit.
- **Ask for the objection early.** "What would stop this from being a fit for you?" surfaces objections **2.7× more often early** and cuts proposal-stage surprises by ~40% [S: Gangly].

### 0.6 Follow-up cadence — the 5-touch sequence (use for every silent lead)

**80% of sales need 5+ touches; 44% of reps give up after one** [S: SendEmAll]. Silence is not a no — it's an unanswered message.

| Touch | Day | Angle | Typical reply rate |
|---|---|---|---|
| Initial | Day 0 | the hook (their specific fact) | 5–7% |
| FU1 | Day 3 | **new angle** (not "just bumping this") | 4–6% (cum. 9–13%) |
| FU2 | Day 7 | social proof / a real data point | 3–4% (cum. 12–17%) |
| FU3 | Day 12 | a different benefit you haven't mentioned | 2–3% (cum. 14–20%) |
| FU4 | Day 21 | **the breakup** ("should I close your file?") | 3–5% (cum. 17–25%) |

[S: SendEmAll, aggregated cold-email benchmarks]

Rules: **change the angle, not the message** — every touch must give a new reason to reply. Wait **>10 days** and there's a **70%** chance they never re-engage [S: Prospeo]. The **breakup email outperforms the middle touches** — it works because it gives permission to say no, and people don't like decisions being made for them. Multi-channel (email + a social touch) lifts response **15–25%** [S: SendEmAll] — but never a call in `no_website` mode.

**Stop immediately if:** they say not interested/remove me · they mark spam · the address hard-bounces.
**Continue carefully if:** they replied "not now" (nurture list, honour the timeframe) · they asked a question but didn't commit (answer + one CTA) · they open every email but never reply (the breakup usually converts these).

### 0.7 The conversation arc (what "done" looks like)

You are not trying to close the deal in the DM thread. You are trying to earn **one of these three outcomes**, in this order of preference:

1. **A yes** → "reply 'let's do it' and I'll start this week."
2. **A dated maybe** → "check back in [month]" — logged, and you honour the date exactly.
3. **A clean no** → file closed, door open, goodwill banked.

Anything else is a stall — and a stall you didn't date is a lost lead (85% die without a scheduled next step [S: Prospeo]). **Every single conversation ends with a question that has an easy answer.**

---

## Section 0 — UNIVERSAL objections (both types)

> These 18 are handled **once**, here. Section 1 and Section 2 point back to them instead of repeating them. Read the diagnosis line before choosing an option.

### U1. "That's too expensive / I don't have the budget right now."

**Frequency & meaning:** the #1 objection in every dataset — **35%** of all B2B objections [S: Salesforce 2025 via Gangly]. Win rate **31%** overall, but **42% when you reframe to ROI and only 19% when you discount first** [S: Gangly]. So: the math beats the discount, every time. "Too expensive" almost never means *no money* — it means *no value established yet*, or they're not the budget holder.

**Option 1 — Per-client math (direct/logical owner):**
> "Totally fair. Quick math: one [job/patient/client] for you is about $X. If this brings even one extra a month, it pays for itself in [N] weeks — you're not buying a website, you're buying the next 10 clients. Does that math hold up for your numbers?"

**Option 2 — Feel-Felt-Found + phased entry (cautious owner):**
> "I understand — most [trade] owners I talk to felt the same until they saw it broken down. What they found is that starting small works: [with-website: the $500 audit first, then decide on the rebuild later] / [no-website: start with the one-page site + call button, expand when it earns]. Want me to show what phase one alone would cover?"

**Option 3 — Cost-of-inaction flip (confident owner):**
> "Can I ask — what does one lost client cost you? If the current [site / no-site] loses even one a month, that's roughly $X/month walking to whoever has a better presence. The price stings once. The leak stings monthly. Want me to show you where the leak actually is?"

**Branch tree**

- ⇐ **"Still too much. I can get it cheaper on Fiverr / my nephew does it for $200."** (≈30% of price follow-ups [E])
  ⇒ "You're right, cheaper exists. The difference: they deliver pages, I deliver leads — [mobile booking path / AI-readable services + reviews / speed]. A $200 page that brings zero clients is the expensive option. Want a two-minute look at what I'd do differently for *your* business specifically?"
  - ⇐ *"Send me that then."* → send ONE screenshot. Not the report. (§0.5)
  - ⇐ *"Still not worth it to me."* → "Fair — then let's not force it. Can I check back after [busy season] with the numbers for your trade?" (date it, then §0.6)

- ⇐ **"I can't pay it all at once."** (≈20% [E])
  ⇒ "Then don't. 50/50 — half to start, half only at launch. No retainer, no monthly hostage. If that works, reply 'let's do it' and I'll send the three things I'd fix/build first."

- ⇐ **"What exactly do I get for $500?"** (≈25% [E] — this is a **buying signal**, not an objection)
  ⇒ answer the scope in one line, then stop talking: "[with-website: full written audit + the priority fixes done, delivered this week] / [no-website: a complete site — services, reviews, click-to-call/booking — live in about a week]."

- ⇐ **Silence** (≈25% [E]) → §0.6 cadence, don't send a second price message.

**Never say:** "I can do it cheaper." · "What's your budget?" (opens an auction you'll lose) · "Everyone else pays this." · any number you haven't sourced (§0.5).

**Exit ramp:** "If it's not the right time for the budget, that's genuinely fine — I'd rather you tell me no than spend on something you don't believe in. Can I check back in [month]?"

---

### U2. "I need to think about it."

**Frequency & meaning:** appears in roughly **9%** of calls [S: Gangly] — but it's not one objection, it's **four wearing a trench coat**: price, stakeholder approval, trust, or timing [S: Prospeo]. **Half** of these come from someone who isn't the decision-maker [S: Prospeo]. Good news: these deals close at healthy rates — often *higher* than average [S: Prospeo]. What kills them is answering with "sure, take your time" and no date.

**Option 1 — "What specifically?" (best first move — surfaces the real objection ~60% of the time [S: Prospeo]):**
> "Totally understand — can I ask what specifically you'd need to think through? Sometimes I can answer it right now and save you the time."

**Option 2 — The three-category force (gives them a menu instead of an interrogation [S: SalesGravy]):**
> "Fair. Usually when someone says that it's one of three things: it's not for you and you want out, you like it but something's blocking you, or you like it and just need to sort something out. Be honest with me — which one is it?"

**Option 3 — Permission to say no (use when they've gone vague/hedgy [S: Sandler]):**
> "Look, if this isn't for you, I'd honestly rather have a no now than chase you for three weeks. Is that where you're leaning?"

**Branch tree**

- ⇐ **"It's the money side."** (≈30% [E]) → go to **U1**.
- ⇐ **"I'd have to talk to my [partner / wife / brother]."** (≈25% [E]) → go to **U3**.
- ⇐ **"I'm just not sure it'll actually bring clients."** (≈20% [E]) → go to **U8**, then offer the free peek (one screenshot, not the report).
- ⇐ **"Honestly, I'm just flat out right now."** (≈15% [E]) → go to **U7**.
- ⇐ **"I can't put my finger on it, just not sure."** (≈10% [E])
  ⇒ "Then let me make it easier: I'll send you one thing to look at — [the single worst thing on your site / a mock of your homepage]. If it doesn't make you go 'oh, that's a problem', tell me and I'll drop it. Fair?"
  - ⇐ *"OK, send it."* → send it, then date the follow-up: "I'll check back Thursday — one line from you is enough."
  - ⇐ *"Just leave it with me."* → "Will do. I'll circle back [specific day] either way — if it's a no by then, just say no." (date it)

**Never say:** "Sure, take your time." (an undated stall is a lost lead — 85% of deals without a scheduled next step die [S: Prospeo]) · "What would it take to get you to decide today?" (pressure → defensiveness).

**Exit ramp:** always leave with a date. Even the exit is a question: "Can I check back Thursday?"

---

### U3. "I need to talk to my partner / my wife / my business partner."

**Frequency & meaning:** the **Authority** bucket — **14%** of objections, win rate **29%** — and it only wins when you act **within 7 days** [S: Gangly]. **75% of high-ticket reps hear "I need to speak to my spouse" at the close** [S: Prospeo]. This is almost never about the other person. It means: *"I'm not convinced, and I don't want to say so to your face."* Do **not** pressure them — **arm them**. They have to sell it internally; give them the ammunition.

**Option 1 — Arm the champion (default):**
> "Of course — smart move. What would help you explain it to them? I can send a five-line summary plus one screenshot of [the biggest issue / the missing presence] so you don't have to pitch it yourself. And what's the one thing *they'd* care about most — the cost, or the new clients?"

**Option 2 — Isolate the real concern (LAER Explore):**
> "Totally get it. So I point you right — is it the price you're weighing, or whether this will actually bring in clients? If I can answer that one thing clearly, would that make the conversation with them easier?"

**Option 3 — Address both of them at once:**
> "Then let's not make you the middleman. I'll send the summary addressed to both of you — one page, zero commitment, you two look at it together. What's the best way to reach you both — same email, or should I send it to them too?"

**Branch tree**

- ⇐ **"I never make money decisions without them, period."** (≈40% [E])
  ⇒ "Respect that — most owners I work with are the same, and honestly it's why they're still in business. So let me do the work for you: I'll send the free peek addressed to both of you. You look together, no pressure, no payment link. Fair?"
  - ⇐ *"Fine, send it."* → send, then date it: "I'll check back [day] — if the two of you aren't feeling it, just say no."
  - ⇐ *"No, I'll get to it."* → "Understood. I'll circle back [day] either way." (never argue)

- ⇐ **"They handle the money, not me."** (≈25% [E])
  ⇒ "Got it — then let me send it straight to them so nothing gets lost in translation. What's the best email for them?" *(Email only. Never ask to call — §3B.3 / §0.5.)*

- ⇐ **"I'll talk to them and let you know."** (≈35% [E])
  ⇒ "Perfect. So I'm not a nag — will you two have had a chance by [day]? If it's a no, I'll close the file and you won't hear from me again."
  - ⇐ *"Sure, Thursday."* → **you message Thursday. Exactly Thursday.** (getmapleads: "call exactly when you said you would — non-negotiable")
  - ⇐ *"I don't know."* → "Then let's say [day]. If it moves, tell me. If not, I'll assume it's a no and stop."

**Never say:** "So you're not the decision-maker?" (insults them) · "Can I speak to them directly?" (in `no_website` this risks a phone-banned ask; in both modes it bypasses the person you need on your side) · "Great, so it's basically a yes then."

**Exit ramp:** "Either way, you'll have the summary — even if it's a no, you'll know what to fix. That's worth the two minutes."

---

### U4. "Who are you? How did you get my info? Is this a scam?"

**Frequency & meaning:** the **Trust** bucket — only **6%** of objections in datasets [S: Gangly], but for cold email/DM it is the **#1 silent killer**: they don't reply, they just delete. The fix is never defensiveness — it's **specificity**. A generic message reads as a scam; a message that proves you looked at *their* business reads as a person.

**Option 1 — Specific proof (skeptical owner):**
> "Fair question. I'm [name] — I found [Business] on [Google Maps / your site] while looking at [trade] businesses in [city]. What caught my eye: [one concrete fact — 63 reviews at 4.8★ but no site link / the mobile menu overlaps / booking is buried]. Scammers send templates. I can send you the actual screenshot of yours. Want it?"

**Option 2 — Risk reversal:**
> "I get it — I'd be skeptical too. That's why I don't ask for anything upfront: [with-website: you see the audit findings first] / [no-website: you see a homepage mock first]. You look, then you decide. No login, no payment link, nothing to sign. Fair?"

**Option 3 — Social-proof bridge:**
> "Other [trade] owners asked me the same thing. What convinced them was seeing *their own* listing in 30 seconds — not a deck, their business. Want the same 30-second look at yours?"

**Branch tree**

- ⇐ **"How did you get my email address?"** (≈35% [E])
  ⇒ "It's public — [on your site's contact page / on your Google Maps listing / on your Facebook page]. I only used what you've published yourself. If you'd rather I stop, say so and I will, no hard feelings."
  - ⇐ *"OK, but don't email again."* → "Understood — closing your file now. Good luck this season." (then actually stop)

- ⇐ **"Still not comfortable. Do you have references?"** (≈30% [E])
  ⇒ "Happy to — [1–2 past builds / before-and-afters], and you pay 50/50 with the second half only at launch, so you hold the leverage the whole way. Want the links?"

- ⇐ **"Are you even a real company? Where are you based?"** (≈25% [E]) → go to **U16**.

- ⇐ **Silence** (≈10% [E]) → §0.6 cadence. Do **not** re-justify yourself — change the angle instead.

**Never say:** anything defensive ("I'm not a scammer!") · invent an office, address, or local phone number you don't have · "I'll add you to my list" · claim a portfolio that isn't yours.

**Exit ramp:** "If you'd rather not, that's completely fine — I'll close the file. If [the leak / the missing presence] ever starts costing you, you have my email."

---

### U5. "Just send me the info / email it over."

**Frequency & meaning:** appears in ~**7%** of calls [S: Gangly] — and it's **not rejection**. It splits roughly **60% polite dismissal / 40% genuine request** [S: GetMapLeads]. Either way the answer is the same: **send a teaser, never the findings.** The trap: if you send the full list, they fix it themselves and you're redundant (§12.4 point 5).

**Option 1 — Teaser + hook:**
> "Happy to. I'll send three screenshots of [the biggest blockers / the mock] — the full [audit / build plan] comes with the project, so you get the *fix*, not just the list. Is the best email the one on your [site / Facebook page]?"

**Option 2 — Question-first (stops the dead-send):**
> "Will do — so I send the right part: are you more worried about [being found on Google] or [turning visitors into calls]? I'll lead with that."

**Option 3 — Trade for a micro-commitment (the strongest version):**
> "Sure. One thing so it's not wasted: if the three screenshots make sense, will you give me ten minutes to walk through them? If not, tell me and I'll close the file — deal?"

**Branch tree**

- ⇐ **"Just tell me what's wrong, I'll fix it myself."** (≈30% [E] — the free-findings trap)
  ⇒ "I'll give you the honest headline: [ONE issue, stated plainly]. The other [N] and how to fix them are what the audit covers — that's the part you're paying for, because the fix is the work. Want the one screenshot that shows the biggest one?"
  - ⇐ *"Fine, send it."* → send ONE. Then: "That's the free one. If you want the rest fixed, reply 'let's do it'."
  - ⇐ *"Then forget it."* → "No problem — I'll close your file. If it starts costing you, you know where I am."

- ⇐ **Ghosts after you send it** (≈40% [E] — the most likely outcome [S: GetMapLeads]) → **Day 4:** "Did the [screenshot / mock] make sense? One line — worth a ten-minute look, or should I close your file?"

- ⇐ **"I'll look when I get a chance."** (≈20% [E])
  ⇒ "Fair. I'll check back [day] — if it's a no by then, just say no and I'll stop."

**Never say:** "I'll email you the full report." · "The full list, just reply 'send it'." · any wording implying the findings ship before payment (§12.4 point 5).

**Exit ramp:** "Either way you'll have the screenshots — even if you never reply, they're useful. Best email?"

---

### U6. "Not interested."

**Frequency & meaning:** a **reflexive block**, not a considered position [S: GetMapLeads: "they are default responses owners use to end the conversation quickly"]. Do **not** debate it and do **not** try one more angle — ask for **micro-permission**. This is the highest-leverage five seconds in the whole playbook, because the "can I check back?" question is almost impossible to say no to.

**Option 1 — Micro-permission:**
> "Totally fair — most owners say that until they see it. Mind if I send you ONE screenshot of [what customers see on a phone / what Maps shows with no site]? Ten seconds to look, then I'll drop it."

**Option 2 — Close-the-loop question:**
> "Got it. Quick close-the-loop so I don't bother you: is it timing, or that you don't believe a [rebuild / site] brings in clients? One word is enough."

**Option 3 — Graceful exit that keeps the lead alive (the money move [S: GetMapLeads]):**
> "No problem at all — thanks for taking the time. Would it be OK if I checked back in a few months? Things change, and I'd rather come back when it actually makes sense for you."

**Branch tree**

- ⇐ **"Yeah, fine, check back."** (≈50% of the time, once you ask like this [S: GetMapLeads]) → log the date, honour it. A "yes" to this keeps the lead live for a future callback.
- ⇐ **"No, don't contact me again."** (≈30% [E])
  ⇒ "Understood — I'll close your file. If anything changes, you're welcome to reach out. Good luck." **Then genuinely stop.** (§0.5)
- ⇐ **"What's the one screenshot?"** (≈20% [E] — the block just cracked)
  ⇒ send it. Do not add a pitch. Let the screenshot work.

**Never say:** "But just let me explain—" · "You'll regret this." · anything that makes them defend their no. A defended no is permanent.

**Exit ramp:** "Closing your file — genuinely good luck this season." *(Warm exit. Goodwill refers business. §0.5.)*

---

### U7. "I don't have time for this right now / get back to me next quarter."

**Frequency & meaning:** the **Timing** bucket. Note the split: *budget-timing* objections have the **highest win rate of all (38%)** when you offer a staged/phased path, while *no-urgency* ones are the **lowest (18%)** and are usually a polite disqualifier [S: Gangly]. The move is to shrink the ask to near zero and put a date on it. **"I'm too busy" is almost always true for a local owner** [S: GetMapLeads] — respect it and it becomes a scheduling problem, not a rejection.

**Option 1 — Shrink the ask (default):**
> "That's exactly why I do it done-for-you — you spend about 30 minutes total (one conversation + approving the design), I do everything else. If I handle it all, is starting next month better, or should I check back after [busy season]?"

**Option 2 — Hold a slot (uses real scarcity, never fake):**
> "Fair — busy means business is good. I only take one [trade] per town so competitors don't end up with twins. Want me to hold [city] with zero deposit, so when you're ready we skip the queue?"

**Option 3 — Season-aware (the strongest for trades):**
> "Makes sense. When's your busy season? I'd rather build in your slow month so the site is live and earning *before* the rush — not sitting half-finished while you're slammed. Which month is worst for you?"

**Branch tree**

- ⇐ **"Next year, maybe."** (≈35% [E])
  ⇒ "Done — I'll check back in [January]. Meanwhile, want me to file the free peek away so you have it when you're budgeting? Costs you nothing and it's ready when you are."
  - ⇐ *"Sure."* → log the date, send nothing more now. Honour the date.
  - ⇐ *"No."* → close the file warmly.

- ⇐ **"I'm too busy to be involved in a project."** (≈30% [E])
  ⇒ "You won't be — that's the point. I write the copy from your [Facebook posts / price list], use your [Maps photos / existing photos], and hand you one five-minute video at the end. Your total involvement is approving the design. Is that doable?"
  - ⇐ *"I still don't have time."* → "Then let's not start now. What month is calmer? I'll come back then." (date it)

- ⇐ **"Get back to me next quarter."** (≈25% [E])
  ⇒ "Will do — [specific month] or [specific month]? I'll message you then, and I won't chase in between." *(In `with_website` mode you may offer a call here if you choose; in `no_website` mode never — §3B.3. Default: stay in-channel.)*

- ⇐ **Vague "later" with no date** (≈10% [E] — the dangerous one)
  ⇒ "So I'm not a nag — if I message you in [month] and it's still a no, is that fine? Or should I close the file?"

**Never say:** "It'll only take a minute" (they've heard it) · "I'll just keep following up" (threat) · fake urgency like "this price expires Friday" (top reps use business-timeline urgency, never artificial discount timers [S: Prospeo]).

**Exit ramp:** "Enjoy the season — I'll come back when you're calmer."

---

### U8. "Can you guarantee I'll get more customers / rank #1 on Google?"

**Frequency & meaning:** everyone who promises this is lying, and the owner has already been burned by one. **Never guarantee rankings or customer counts** (§12.7). Guarantee the **work and the inputs**, then show the **math**. This objection is often really "I don't believe it works" — the fix is proof, not promises.

**Option 1 — Honest + risk reversal:**
> "No honest person guarantees #1 — anyone who does is lying to you. What I do guarantee: a [modern, fast, mobile site with a working booking path / site that Google and AI assistants can actually read], delivered in [N] days. 50/50, second half only at launch, and you own everything. The risk sits with me, not you. Fair?"

**Option 2 — Work-guarantee, spelled out:**
> "I can't guarantee Google's algorithm, and I'd run from anyone who says they can. What I *can* put in writing: every issue the audit found gets fixed, it loads fast on a phone, customers can call or book in one tap, and I don't get paid in full until you see it live. Does that sound like a fair guarantee?"

**Option 3 — Proof stack (when the real issue is trust [S: Prospeo "Proof Stack"]):**
> "Rather than promise, let me show. I'll send [one before-and-after / one real example from your trade], and you can judge. If it doesn't convince you, don't hire me. Want the example?"

**Branch tree**

- ⇐ **"So there's no guarantee at all?"** (≈40% [E])
  ⇒ "There is — just the honest kind. I guarantee the deliverables and the timeline, and I carry the financial risk: you pay half at the end, when it's live. What I won't do is promise Google's ranking, because that would be a lie and you'd find out in three months."
  - ⇐ *"Other companies guarantee it."* → "They mean ads or a paid ranking report. Organic #1 is not something anyone controls. If someone's promising it, ask them to put it in the contract — they won't."

- ⇐ **"I don't believe a website brings clients."** (≈30% [E])
  ⇒ "That's the right thing to be skeptical about. So let's test it on your business instead of arguing: I'll show you what [your customers see now / what comes up when someone searches your name], and you tell me if that looks like it converts. If it does convert, no need for me. Fair?"
  - ⇐ *"Show me."* → send the screenshot. Then go to the offer.

- ⇐ **"How do I know you won't disappear?"** (≈20% [E]) → go to **W7** (with-website) / **U15** (payment terms).

- ⇐ **Silence** (≈10% [E]) → §0.6 cadence.

**Never say:** "I guarantee you'll get X clients." · "We rank everyone on page 1." · "Our secret method." · any invented statistic.

**Exit ramp:** "If proof matters more than promises to you — good, that's the right instinct. Let me show you something real instead."

---

### U9. "Why should I choose you specifically?"

**Frequency & meaning:** this is a **differentiation objection** hiding as a question. Never answer with adjectives ("passionate", "the best") — those are what everyone says. Answer with **a specific gap only you fill** and a **risk reversal**. Generic comparisons lose this objection **4 times out of 5** [S: Gangly on "already have a tool"].

**Option 1 — The specific gap (default):**
> "Honestly? Because I do one narrow thing for [trade] businesses in [city] — not full-service marketing, not ads, just the website that makes you findable and bookable. Most people emailing you do everything for everyone. I'll show you the three things I'd fix on yours and you can judge if I actually understand your business. Want them?"

**Option 2 — Risk reversal + ownership:**
> "Two reasons. One: you pay 50/50, second half only at launch. Two: you own everything — domain, site, content, no monthly hostage, no lock-in. Most agencies rent you your own website. I don't. Does that matter to you?"

**Option 3 — The specificity test (the strongest, because it proves itself):**
> "Don't take my word for it — test me. Ask any of the others emailing you what specifically is wrong with [your mobile menu / your booking path / your Maps listing]. If they can answer, hire them. If they can't, you know who actually looked at your business. Want to see what I found on yours?"

**Branch tree**

- ⇐ **"So what's actually different from the five other emails I got today?"** (≈35% [E])
  ⇒ "The others are templates with your name pasted in. Here's the proof I'm not: [one specific, verifiable detail about their business that a template couldn't know]. That took me looking at your [site / listing] properly. Want the rest of what I found?"
  - ⇐ *"OK, fair enough."* → move to the offer. One ask only.
  - ⇐ *"Everyone says that."* → "Then test it — the question I gave you works on all of them. I'll wait." (confidence wins this branch)

- ⇐ **"I just want the cheapest option."** (≈25% [E])
  ⇒ "Then I'll be straight with you: if price is the only thing that matters, there are cheaper options and I'm not going to pretend otherwise. What I'd ask is what a cheap site that brings no clients actually costs you. Want me to show you the difference in one screenshot, then you decide?"
  - ⇐ *"Show me."* → one screenshot.
  - ⇐ *"No, cheapest."* → "Understood. If it doesn't work out, come back and I'll show you what went wrong — free." (walk away warmly — §0.2 lane 4)

- ⇐ **"Why not just use a big agency?"** (≈20% [E])
  ⇒ "You can — you'll pay $3–10k and talk to an account manager who never touches your site. I build only for local [trade], the price is $[X], and you talk to the person doing the work. Which matters more to you — brand name or the person actually building it?"

- ⇐ **"I need to see examples first."** (≈20% [E]) → send 1–2 real examples, then ask: "Is that the kind of thing you'd want, or different?"

**Never say:** "We're the best in the industry." · "We're passionate about design." · "We have 10 years of experience." (all unfalsifiable filler) · anything you can't prove if challenged.

**Exit ramp:** "If someone else earns it, hire them — I mean that. If not, my door's open."

---

### U10. "I'm not the one who decides — you'd need to talk to [the owner / my boss / head office]."

**Frequency & meaning:** the **Authority** bucket again, but this time it's *true* — you reached the wrong person. Win rate **29%**, and it only wins if you **multi-thread within 7 days** [S: Gangly]. The goal is **not** to argue, and **not** to lose the contact you have. Your ally is now the person in front of you — make it easy for them to hand you over. HubSpot's play: thank them, then ask who owns the decision and whether they'll make the introduction.

**Option 1 — Ask for the introduction (default):**
> "Thanks for telling me straight — that saves us both time. Who handles this on your side? If you point me at them, I'll take it from there and you won't have to be involved at all."

**Option 2 — Recruit them as an ally:**
> "No problem. One thing though — you probably know what would land with them better than I do. What do you think they'd care about most: the cost, or the extra clients? I'll write it for them, not for me."

**Option 3 — Leave something useful behind:**
> "Understood. Would it help if I sent you a one-page summary you can forward? If they're interested, great; if not, no harm. What's the best way to get it to them?"

**Branch tree**

- ⇐ **"It's [name], here's their email."** (≈40% [E] — best case)
  ⇒ "Perfect, thank you. I'll reach out to them directly and mention you pointed me their way. I'll keep you out of the middle."
  - Send within 24h, referencing the referral. That's the whole trick.

- ⇐ **"I can't give out their details."** (≈30% [E])
  ⇒ "Completely fair — I wouldn't expect you to. Then could you forward one thing from me? It's a five-line summary and one screenshot. If it's a no, it's a no and I'll stop."
  - ⇐ *"Fine, send it."* → send it, then follow up once with the referrer, not the boss.

- ⇐ **"We're not looking at this right now."** (≈20% [E])
  ⇒ "No problem. When would be a better time to bring it up with them — after [their busy period / the new year]? I'll check back then and I won't bother you in between."

- ⇐ **"Just tell me and I'll pass it on."** (≈10% [E] — usually a dead end)
  ⇒ "Will do — and to make it easy, I'll write it so you can forward it word for word. If nothing comes back, I'll assume it's a no."

**Never say:** "So who's really in charge?" (insulting) · "I'll just keep emailing until I get the right person." · anything that makes the gatekeeper feel bypassed — they can kill your message with one sentence.

**Exit ramp:** "Thanks for the help — genuinely. If it's a no, no hard feelings."

---

### U11. "Another company quoted me less / I can get it cheaper elsewhere."

**Frequency & meaning:** a **nerve test as much as a price comparison** [S: Objeq]. Two things are true at once: sometimes there's a genuinely cheaper quote, and sometimes they're probing whether your price is real. If you fold instantly, you've taught them the price was padded — and by extension that everything else you said might be. **Verify the comparison before you defend anything.**

**Option 1 — Inspect the comparison (default, straight from Objeq's playbook):**
> "That's a real difference, so let's look at it honestly — is their quote the same scope? Same [booking setup / mobile work / support after launch]? Most of the time the gap lives in what's *not* included. What did their quote cover?"

**Option 2 — Reframe from price to cost of being wrong:**
> "The cheaper option costs less *if it works*. What does it cost if it doesn't — another six months of nothing, and paying twice? I'd rather you got it right once. Want me to show you what's in mine that usually isn't in theirs?"

**Option 3 — Concede structure, never price:**
> "I'm not going to pretend I'm the cheapest — I'm not trying to be. What I can do is move *how* you pay: 50/50, or phase it. But the price reflects the work. Want me to break down exactly what the [N] dollars covers?"

**Branch tree**

- ⇐ **"Honestly, I don't know what their quote covered."** (≈35% [E] — the comparison just collapsed)
  ⇒ "Then let's find out — forward me their quote and I'll show you exactly where the gap is. If theirs genuinely covers the same thing, take theirs, and I'll tell you so. Fair?"
  - ⇐ *"OK."* → do the honest comparison. If theirs is genuinely equivalent, **say so** — that honesty closes more deals than any pitch, and it earns referrals.
  - ⇐ *"Never mind, just send yours."* → send the scope, one page.

- ⇐ **"They said the same thing, they're just cheaper."** (≈30% [E])
  ⇒ "Then here's the only question that matters: what happens if it doesn't work? With mine you pay half at the end, you own everything, and if it's not what you approved you don't pay the second half. Can they match that? If yes, take them."

- ⇐ **"Just match their price."** (≈20% [E])
  ⇒ "I won't do that — if I could drop it that easily, I was overcharging you before, and you'd be right not to trust me. What I *can* do is [phase it / trim the scope]. Want to see what a smaller version looks like?"
  - ⇐ *"No, match it or I walk."* → "Then I'd take their offer — genuinely. If it doesn't work out, come back and I'll tell you honestly what went wrong." (walk away warm — §0.2 lane 4)

- ⇐ **"They're a big agency, you're not."** (≈15% [E])
  ⇒ "Right — and with them you'll pay $3–10k to talk to an account manager who never touches your site. With me you talk to the person building it. Which matters more to you?"

**Never say:** "We're better quality." (unprovable) · "They're amateurs." · a reflexive discount · "OK, I'll match it" (re-prices your whole service retroactively [S: Objeq]).

**Exit ramp:** "If budget is the deciding factor, they may genuinely be the right call right now — and I'd mean that. My door's open if requirements grow."

---

### U12. "I'll just do it myself / AI can build it for free / my nephew will do it."

**Frequency & meaning:** rarely hostile — usually **cost-anxiety plus underestimating the last 20%** [S: Squarespace community / InsideTheSquare: AI builders produce drafts that need heavy human polish]. Don't argue about capability. Agree, then move the conversation to the part that actually decides the outcome: **who finishes it, and whether it brings calls.**

**Option 1 — The time-cost (default):**
> "You absolutely can — AI gets you a draft in an hour, and it's genuinely good for that. The part that kills it is the next 20 hours: copy that sells, the booking setup, being readable by Google and AI assistants, speed on a phone. That's the part I do, in days instead of months of evenings. Want me to list what the AI draft will still be missing for *your* trade?"

**Option 2 — Pages vs. a machine:**
> "AI builds *pages*. I build the thing that turns pages into calls. It won't write a [trade]-specific booking flow, set up your reviews as proof, or structure it so ChatGPT can actually recommend you. I use AI too — then I add the 20% that makes the phone ring. Want a side-by-side for one page?"

**Option 3 — The free grading test (hard to refuse, and it's honest):**
> "Try this: have it build one page, then send it to me. I'll grade it free against what actually makes a [trade] site bring calls. If it passes, you saved $[X] and I'll tell you so — no pitch. If it doesn't, you'll know exactly what's missing. Fair?"

**Branch tree**

- ⇐ **"My nephew does this stuff, he'll do it for free."** (≈35% [E])
  ⇒ "He probably did a solid job getting you online — I'm not knocking him. The difference is that a family site shows information and a lead site brings calls. And he's doing you a favour between his real job, so the boring parts slip. How many extra [jobs/patients] would the upgrade need to bring to pay for itself? For you it's [1–2]."
  - ⇐ *"Free is free."* → "True. Free plus zero new clients versus paid plus [N] new clients — which is actually cheaper? Want the math for your trade?"
  - ⇐ *"OK, show me."* → send one comparison, then stop.

- ⇐ **"AI is free and good enough."** (≈30% [E])
  ⇒ "Good enough for what, though? Free gets you something that looks like a website. It doesn't get you something that shows up when someone asks ChatGPT for a [trade] in [city]. That's the whole difference. Want me to run that exact question now and send you what it says about you?"

- ⇐ **"I'll get around to it myself."** (≈25% [E])
  ⇒ "How long has it been on the list? Honestly — I hear that a lot and it's usually a year. Not a criticism, it's just that running a business eats the evenings. What if I did the whole thing and you approved it in one go?"

- ⇐ **"Send me a checklist and I'll do it."** (≈10% [E])
  ⇒ "I'll do better — I'll show you one thing to fix first. The rest is the part you'd be paying for, because the fixing is the work. Want that one?"

**Never say:** "AI is rubbish." (they'll defend it) · "Your nephew doesn't know what he's doing." (insults family) · "You'll never finish it." (condescending).

**Exit ramp:** "Either way, run the ChatGPT test on yourself — it's free and it'll tell you more than I can."

---

### U13. "I got burned before — I don't trust web people anymore."

**Frequency & meaning:** the emotional core of the Trust bucket. The textbook **Feel-Felt-Found** case: "paid, waited, got silence, site never finished, they held the domain." Do **not** defend your industry. Validate it, then show the **structure that prevents it from happening again** — because they can't trust a stranger, but they *can* trust a mechanism.

**Option 1 — Validate + structural proof (default):**
> "I'm sorry — and honestly, I hear this most weeks. [Trade] owners tell me the same story: paid up front, waited months, got silence. That's exactly why I work the way I do: half now, half *only* at launch, you own the domain and the site from day one, and you get updates in a shared folder. I can't vanish with things you already own. Want me to walk you through the three checkpoints before you pay anything?"

**Option 2 — Diagnose the specific failure:**
> "What went wrong last time — was it the communication, the quality, or did they hold your site hostage? Tell me the one thing and I'll show you exactly how I contract against it."

**Option 3 — Replace trust in the person with trust in the terms:**
> "Don't trust me — trust the structure. You pay half to start and the second half *only* when it's live on *your* domain. You approve the design before anything is built. And I show you something real before I ask for anything. If the free look isn't convincing, block me — no hard feelings. Fair test?"

**Branch tree**

- ⇐ **"They took my money and disappeared."** (≈35% [E])
  ⇒ "That's theft, not a bad experience — and it's why I only take half up front. If I disappeared, you'd have lost half of a small number instead of all of a big one, and you'd still own the domain. Want to see the checkpoints written out before you commit to anything?"
  - ⇐ *"What are the checkpoints?"* → list them: (1) you approve the plan, (2) you see the design, (3) it goes live and you pay the rest. Concrete, short.

- ⇐ **"They held my domain / site hostage."** (≈25% [E])
  ⇒ "That's the worst version. Rule one with me: the domain is registered in *your* name, on *your* account, from day one — before any money changes hands. If we part ways, you keep it. I'll say that in writing. Want that in the first message?"

- ⇐ **"How do I know you're different?"** (≈25% [E])
  ⇒ "You don't, and I'm not going to ask you to take it on faith. That's why the first step is free and the second step is half price — the risk is small and it's on me until you've seen something. What would you need to see to feel safe?"

- ⇐ **"Forget it, I'm done with web people."** (≈15% [E])
  ⇒ "That's fair, and I won't push. If you ever want a second opinion on what you were left with — no charge, no pitch — just reply. Good luck." (leave the door open; burned owners refer)

**Never say:** "Not all web guys are like that!" (defensive) · "You should have used a contract." (blaming them) · "I'd never do that." (a promise, not proof — show the structure instead).

**Exit ramp:** "Even if you never hire me, don't pay anyone 100% up front again. That's the whole lesson."

---

### U14. "Send me a proposal / contract first — what are your terms?"

**Frequency & meaning:** looks like a stall, but it's often a **buying signal in disguise** — they're picturing the deal. It becomes a stall only if you send a document and then wait. Answer the terms **in the message**, short, and attach the document to a **next step**, never as the next step itself [S: gruv.ai: "Update the document the same day and close with one dated next step in writing"].

**Option 1 — Terms in three lines (default):**
> "Happy to. The short version: [with-website: $500 audit + priority fixes, then $1500 if you want the full rebuild] / [no-website: $1200 for the complete site], 50% to start and 50% only at launch, you own the domain and everything on it, no retainer. I'll send the one-pager today. If the terms look right, can you confirm by [day] so I can hold [day] for the start?"

**Option 2 — Document + forcing question:**
> "Sending it now. One question so I know it's the right version: is the blocker going to be the total cost, or the payment timing? I'll build the doc around whichever one matters."

**Option 3 — Pre-empt the objection (use if they've been burned before):**
> "Will do — and I'll include the two things most owners ask about: you own the domain from day one, and the second half is only due when it's live. If either of those doesn't work for you, tell me now and I'll adjust before you read the rest."

**Branch tree**

- ⇐ **"Send it and I'll review it."** (≈45% [E] — the danger branch)
  ⇒ "Sure. So it doesn't sit in your inbox — can you confirm by [specific day]? If it's a no by then, just say no and I'll close the file." *(An undated "I'll review it" is how deals die — 85% [S: Prospeo].)*
  - ⇐ *"Sure, Thursday."* → message Thursday. Exactly.
  - ⇐ *"I'll get to it."* → "Then let me ask differently — is this something you actually want, or is it a no? Either answer is fine, I just don't want to waste your time." (U2 permission-to-say-no)

- ⇐ **"I need to see the contract before anything."** (≈30% [E])
  ⇒ "Of course. I'll send the one-pager and the terms together. Nothing's signed and nothing's paid until you've seen both and said go. Does that remove the worry?"

- ⇐ **"Why 50% up front?"** (≈15% [E])
  ⇒ "Because it's the fair split of risk: half so I can start the work, half held back so you're not exposed if it's not what you approved. If you'd rather pay all at the end, I'd have to say no — but I'd rather tell you that now than surprise you later." *(Never accept vague pay-on-completion terms [S: gruv.ai].)*

- ⇐ **"Can you just start and invoice me after?"** (≈10% [E]) → go to **U15**.

**Never say:** a long legal document with no next step · "I'll send the full proposal when you're ready." · three different price tiers in one message (§12.4: one price, one thing).

**Exit ramp:** "If the terms aren't right, tell me which line and I'll tell you honestly whether it can change."

---

### U15. "Can I pay at the end / pay per result / pay you commission?"

**Frequency & meaning:** a **cash-flow and risk-transfer** request. Freelancer guidance is blunt here: avoid vague pay-on-completion terms, and if the payment trigger can't be defined, **pause and close out** [S: gruv.ai]. A performance-only deal also means they've stopped valuing the work — and it puts you in a position where you can't control the outcome (their sales, their pricing, their season).

**Option 1 — Hold the structure, offer a trigger (default):**
> "I can't work for free and I can't work for commission — if I could control how many people walk through your door, I'd charge ten times more. What I *can* do: 50/50, with the second half due when it goes live, not when you get your first client. That way you're not exposed, and I'm not gambling on your season."

**Option 2 — Reframe what they're actually buying:**
> "You're not buying a result you can't guarantee either — you're buying a proper site that's live and working. Nobody can promise the phone rings. What I can promise is that it's built, it's yours, and it's faster and clearer than what you have now. Half at launch. Fair?"

**Option 3 — Meet them partway with a *defined* trigger (last resort, only if it's a real deal):**
> "Here's the most I can flex: 50% now, and the last 25% held until launch — so you're only 75% in when you see it live. But I can't do 'pay when it brings clients', because neither of us can define that. Want to do it that way?"

**Branch tree**

- ⇐ **"I only pay when I see results."** (≈40% [E])
  ⇒ "Then we're not a fit, and I'd rather say that now. But let me ask — what would 'results' mean for you? If we can define it, maybe there's a version. If it's 'when the phone rings', that's not something either of us controls."
  - ⇐ *"Then no deal."* → "Understood. If you want to revisit it later with a clearer picture of what you need, my door's open." (close it cleanly)
  - ⇐ *"Let's say X."* → only proceed if X is something you actually control (site live, mobile working, booking functioning). Otherwise decline.

- ⇐ **"Every freelancer takes payment at the end."** (≈25% [E])
  ⇒ "Some do, and some get burned. Half up front is standard for custom work — it's also what protects you, because I'm not going to disappear mid-build if I'm invested. If you'd rather pay 100% at the end, I'll have to pass, respectfully."

- ⇐ **"Can we do a revenue share instead?"** (≈20% [E])
  ⇒ "I appreciate the ambition, but no — I'd be betting my rent on your sales, and I don't have control over your pricing or your season. If the site works, you'll get the upside anyway. Shall we do it the simple way?"

- ⇐ **"I can't pay anything up front."** (≈15% [E])
  ⇒ "Then let's not force it. If cash flow is the issue, the honest move is to wait until you can do it properly rather than do it half-way. Can I check back in [month]?" (date it)

**Never say:** "OK, pay me whatever at the end." (you will get paid nothing, and you've also signalled the work is worthless) · "Sure, commission works." · "I'll take a % of your revenue." (undefined, unenforceable, and it puts you in their books)

**Exit ramp:** "I'd rather lose the deal than do it in a way that ends badly for both of us."

---

### U16. "Where are you based? Do you actually work with businesses here?"

**Frequency & meaning:** a real trust objection for anyone reaching across borders, and it deserves a **straight answer, never a dodge**. Faking a local address is the fastest way to lose everything — if they ever check, you've burned the niche permanently. Remote delivery is completely normal now; what matters to them is **who owns what, who answers, and what happens if something goes wrong.**

**Option 1 — Straight answer + what it changes (default):**
> "Straight answer: I'm based in [location] and I work remotely with [trade] businesses in [their country]. That's been normal for years — your web guy is on a screen either way. What matters: you own the domain and the site, we're in the same inbox, and I work your time zone for calls and messages. Anything else you'd want to know?"

**Option 2 — Turn it into an advantage:**
> "I'm in [location] — which is exactly why my price is $[X] and not the $3–10k a local agency charges for the same work. Same output, no office overhead, and you still own everything. Would you rather pay for a city address or for the site?"

**Option 3 — Address the real fear behind the question:**
> "Fair question — I think what you're really asking is 'if something goes wrong, who fixes it?' The answer: me, on the same email thread, with the second half of the money still in your pocket until it's live. And you own the domain from day one, so you're never stuck with me. Does that cover it?"

**Branch tree**

- ⇐ **"I'd rather work with someone local."** (≈35% [E])
  ⇒ "Totally fair, and if a local option at a price you're happy with exists, take it — genuinely. The only thing I'd say is that most of the local quotes you've had were $3–10k. If your local guy is cheaper than mine, hire him. If not, I'm here."
  - ⇐ *"OK, what's your price?"* → give the single number. One ask.

- ⇐ **"How do I know you'll still be around?"** (≈30% [E])
  ⇒ "You don't — which is exactly why you own the domain and everything on it from day one, and why you hold half the money until it's live. If I vanished, you'd have a complete site you own. That's the whole safety design."

- ⇐ **"Are you a real company?"** (≈20% [E]) → go to **U4** (specific proof), then back here for the ownership answer.

- ⇐ **"Do you have clients in my country?"** (≈15% [E])
  ⇒ "Yes — [N] in [trade]. I'll send you one example. If you'd rather see something closer to you, tell me and I'll be honest about what I have and haven't done."

**Never say:** a fake local office or address · "I'm basically local." (a lie waiting to be caught) · "Location doesn't matter" (it does to them, or they wouldn't have asked — answer the fear).

**Exit ramp:** "If local matters more than price, that's a legitimate way to decide. If you change your mind, you know where I am."

---

### U17. The lead went quiet — recovery after silence

**Frequency & meaning:** this isn't an objection, it's the **most common outcome of all**: they were warm and then vanished. Silence is almost never a considered no — it's a message that got buried, or a decision they avoided. **80% of sales need 5+ touches and 44% of reps quit after one** [S: SendEmAll]. Run the §0.6 cadence, and make the **breakup email** your best weapon: it regularly outperforms the middle touches because it gives them permission to say no [S: SendEmAll].

**Message 1 — Day 3, new angle (never "just bumping this"):**
> "One thing I didn't mention: [new, real angle — e.g. what customers see on a phone / what ChatGPT currently says about your business]. Want me to send that part?"

**Message 2 — Day 7, proof:**
> "Quick data point — [a real, sourced figure for their trade or a real example]. Happy to show you the working. Useful?"

**Message 3 — Day 12, different benefit:**
> "Different angle — [the thing you haven't pitched yet: speed, reviews as proof, the booking path]. Is that something you're thinking about at all?"

**Message 4 — Day 21, the breakup (highest reply rate of the follow-ups):**
> "I've reached out a few times about [the site / the missing presence] and haven't heard back, so I don't want to keep cluttering your inbox. Should I close your file, or is this worth revisiting in a few months? Either way, no hard feelings."

**Branch tree**

- ⇐ **"Sorry — buried. Tell me more."** (≈30% of replies [E]) → you're back in a live conversation. Pick up where you left off: one ask, not a re-pitch.
- ⇐ **"Not now, but check back in [month]."** (≈30% [E]) → log the exact month, honour it, don't touch them in between.
- ⇐ **"Actually yes, let's do it."** (≈15% [E]) → send the start message immediately. Don't celebrate, just execute.
- ⇐ **"Please stop emailing me."** (≈15% [E]) → "Understood — closing your file now. Good luck." **Then actually stop.** (§0.5)
- ⇐ **No reply to the breakup** (≈10% [E]) → 90-day re-engagement list, fresh angle, one more attempt. Then stop.

**Never say:** "Just following up!" · "Did you see my last email?" · "Bumping this to the top of your inbox." (all zero-value, all deserve to be ignored [S: SendEmAll]) · any guilt-tripping ("I've emailed you three times…").

**Exit ramp:** the breakup *is* the exit ramp — that's why it works.

---

### U18. "I don't have photos / content / text — this sounds like a lot of work for me."

**Frequency & meaning:** a **capacity objection**, not a price objection. They're picturing themselves writing paragraphs at 9pm. The fix is to show that **you do the work from what already exists** — their Facebook posts, price list, Maps photos, and a 10-minute conversation. Local owners decide fast when the effort is near zero [S: LeadsAgent: "Ready to buy if you make it easy"].

**Option 1 — Everything-from-what-exists (default):**
> "You won't write anything. I build it from what you've already got — your [Facebook posts / price list / photos on Maps] — and one short conversation. Your total involvement is approving the design. If I did all of it, would that change things?"

**Option 2 — The 30-minute maths:**
> "Here's the honest number: about 30 minutes of your time, total. One conversation now, one design approval later. Everything else — copy, photos, layout, the booking setup — I handle. Is 30 minutes over a couple of weeks realistic for you?"

**Option 3 — Reframe the fear:**
> "Most owners think it's a big project. It isn't — the big project is what you're already doing: running the business. My job is to take that off your plate, not add to it. Want me to show you a mock built *only* from your public photos and posts, so you can see what it looks like before you give me anything?"

**Branch tree**

- ⇐ **"I don't have any photos."** (≈35% [E])
  ⇒ "Then we use what's on your [Maps listing / Facebook page], and if we need more, you take four quick phone photos of a job — that's genuinely it. I'll tell you exactly which four. Does that work?"
  - ⇐ *"OK."* → name the four shots. Concrete beats abstract.

- ⇐ **"I'm not good with words."** (≈25% [E])
  ⇒ "That's exactly my job. I'll write it and you'll read it and say 'yes' or 'change this line'. You'll never have to write anything from scratch. Deal?"

- ⇐ **"I don't have time to be involved."** (≈25% [E]) → go to **U7** (shrink the ask).

- ⇐ **"Just build whatever you think."** (≈15% [E] — a *great* branch, but don't run with it blindly)
  ⇒ "I'd love to — one guardrail though: I'll send you a rough version first so you can say 'that's not us' before I finish it. Ten seconds of your time, and you won't get a surprise. Fair?"

**Never say:** "It's really easy, anyone can do it." (dismissive) · "You'll need to write your own content." (kills the deal) · "Send me everything you have." (overwhelming).

**Exit ramp:** "If you'd rather do nothing at all for now, I'll mock it from your public photos and you can look whenever."

---

## Section 1 — WITH-WEBSITE owners only (they already have a site)

> Use **after** §0. Every response here assumes you have actually **looked at their site** — cite at least one concrete, verifiable defect or you sound like a template (§12.4, Prospeo Script rule). The primary pitch is **outdated/broken site → modern rebuild**; AI-readiness is one supporting bucket, never the lead (§12.4R).

### W1. "We already have a website and we're happy with it."

**Frequency & meaning:** the **"already have a tool"** objection — **18%** of all objections, and it has the second-lowest win rate at **22%** because reps answer it with generic "we're better" claims, which fail **4 times out of 5** [S: Gangly]. It only cracks with a **specific gap** they can see for themselves. "We're happy" usually means *"I haven't looked at it on a phone in years."*

**Option 1 — The phone test (the single highest-percentage opener):**
> "Great — that's actually why I wrote. I checked it on my phone and [the menu overlaps / there's no call button / it takes about X seconds to load / booking is buried three taps deep]. Desktop hides it, phones expose it — and most of your customers are on phones. Want the screenshot? Ten seconds to see what they see."

**Option 2 — The AI-visibility angle (supporting bucket, never lead with jargon — §12.5):**
> "Glad it's working. One thing most owners miss: when someone asks ChatGPT or Gemini for a [trade] in [city], the assistants can only recommend sites they can *read*. Yours [hides prices in images / blocks key pages / has no reviews markup]. Want me to show you what ChatGPT says about you right now? It's eye-opening."

**Option 3 — Compliment + wedge:**
> "Your [reviews / services / photos] are genuinely strong — the site undersells them. I found [N] specific things that push visitors away; fixing just [ONE] would lift calls without touching the rest. Want the three-item list?"

**Branch tree**

- ⇐ **"It brings us business already — why touch it?"** (≈40% [E])
  ⇒ "That's the best reason to touch it — you're winning *despite* the leak. If it's bringing X now with [broken mobile / no booking path], imagine X plus 30% with it fixed. I'd start with the $500 audit and the priority fixes — you see the lift before we ever talk about a rebuild. Want the audit scope?"
  - ⇐ *"Send the scope."* → send it. One ask: "Reply 'let's do it' and I'll start this week."
  - ⇐ *"We're fine, honestly."* → "Fair. One question though — when did you last look at it on your phone? If it's fine there too, I'll drop it." (the phone test is the whole objection; most say "a while ago")

- ⇐ **"Our web guy watches it."** (≈25% [E]) → go to **W2** or **W4**.
- ⇐ **"Send me the screenshot."** (≈20% [E] — the block just cracked)
  ⇒ send ONE screenshot. No pitch attached. Then: "Want the other two?"
- ⇐ **"We're happy, thanks."** with no engagement (≈15% [E]) → §0.6 cadence, different angle at Day 3. Never repeat the same pitch.

**Never say:** "Your website is terrible." · "Whoever built this didn't know what they were doing." · anything about their design taste (that's their call, not yours) · "You're losing thousands" without a sourced figure (§12.6).

**Exit ramp:** "If it's genuinely working for you, leave it alone — I mean that. Can I check back after [season] just in case?"

---

### W2. "My nephew / son / friend built it and handles it."

**Frequency & meaning:** a **loyalty + money** objection wearing a family mask. Attacking the relative loses the deal instantly and permanently (Cognism: never badmouth — the owner likes them). The winning frame is **design vs. lead-machine**: a family site *shows information*; a lead site *brings calls*. Those are different jobs and can coexist.

**Option 1 — Honour + differentiate (default):**
> "He probably did a solid job getting you online — I'm not knocking that. The difference is that a family site shows information, and a lead site brings calls: [search structure / mobile booking / reviews as proof / speed]. Worth a two-minute comparison? Even if he implements it, you keep the insight."

**Option 2 — Workload empathy (the humane angle):**
> "That's handy — but he's doing you a favour between his real job, right? So the boring bits slip: [speed / updates / backups / the review setup]. I'd do the maintenance *and* the lead upgrades so neither of you has to think about it. Want me to list what I'd take off his plate?"

**Option 3 — Free grading test (removes the loyalty conflict entirely):**
> "Send me one page he built and I'll grade it free against what makes a [trade] site bring calls. If it passes, you keep everything as is and I'll say so. If it doesn't, you'll know what's missing — and he can even do the fixes."

**Branch tree**

- ⇐ **"He does it for free — you charge."** (≈40% [E])
  ⇒ "Free is hard to beat, genuinely. So here's the only question: how many extra [jobs/patients] would the upgrade need to bring to pay for itself? For you that's [1–2]. Free plus zero new clients, versus paid plus [N] new clients — which is actually cheaper? I'll show you the math for your trade."
  - ⇐ *"Show me."* → the math, one page. Then one ask.
  - ⇐ *"He'd be offended."* → "Then don't replace him — keep him for updates and let me fix the parts that bring clients. He'd probably rather you kept the family site. Want me to send him the list directly so it's not coming from you?"

- ⇐ **"He's a professional, actually."** (≈25% [E])
  ⇒ "Then you're in good hands and I'll say so — but professional designers optimise *looks*. I optimise *calls* and whether AI assistants can read the site. Different job. One test settles it: ask ChatGPT for the best [trade] in [city] and see if you appear. Want me to run it and send both answers?"
  - ⇐ *"OK, run it."* → run it, screenshot it, send it. That screenshot is the entire pitch.

- ⇐ **"It's family, I'm not changing it."** (≈20% [E])
  ⇒ "Completely understood — I'd do the same. If you ever want a second opinion, no charge and no pitch, just reply. Good luck." (exit clean; family loyalty means referrals later)

- ⇐ **"How much would it cost to fix just the bad parts?"** (≈15% [E] — the crack)
  ⇒ "$500 for the audit and the priority fixes. If it turns into a rebuild later, that's a separate conversation and a separate decision. Want the audit scope?"

**Never say:** "Your nephew isn't a professional." · "Family projects always fail." · "He's ripping you off." · anything that forces them to defend a family member.

**Exit ramp:** "Keep him for the updates — I'd just fix what brings clients. Different jobs."

---

### W3. "We just redid it recently / it's brand new."

**Frequency & meaning:** a **status-quo + sunk-cost** objection. They spent money recently and don't want to hear it was wasted. Don't attack the new site — find the **lead layer** a recent build usually still misses (fresh designs often nail looks and skip booking, local pages, review proof, and AI readability).

**Option 1 — Compliment + the leftover list:**
> "Congrats — fresh is genuinely good. I looked anyway, out of habit, and spotted [two leftovers: e.g. no location pages / images without descriptions / booking still three taps in]. New builds often miss the *lead* layer. Want the two-item punch list? Your guy can implement it himself."

**Option 2 — Waste-not framing:**
> "Then you're 90% there — it would be a waste to redo it. My $500 audit is built for exactly this: keep the design, fix the 10% that blocks Google, AI assistants, and calls. Want me to scope just the gaps?"

**Option 3 — The live test:**
> "Then let's check it properly instead of guessing — I'll ask ChatGPT '[best trade] in [city]' and see whether you come up. If you do, you're genuinely sorted and I'll tell you so. Want the answers?"

**Branch tree**

- ⇐ **"The designer said it's fully optimised."** (≈35% [E])
  ⇒ "Designers optimise looks; I optimise calls and whether AI can read the site — different job. One test settles it: ask ChatGPT for the best [trade] in [city] and see if you appear. Want me to run it live and send both replies?"
  - ⇐ *"Do it."* → run it, send the screenshot. Then one ask.
  - ⇐ *"We trust our designer."* → "Good — then send them my two-item list and let them decide. If they fix it, you win either way."

- ⇐ **"I'm not spending more on it right now."** (≈30% [E]) → go to **U1**, then **W5** (patch vs rebuild math).
- ⇐ **"It's brand new, it can't have problems."** (≈20% [E])
  ⇒ "New isn't the same as built for leads — I've seen three-month-old sites with no call button on mobile. Let me show you one thing, and if it's fine, you'll never hear from me again. Fair?"
- ⇐ **"Send the punch list."** (≈15% [E]) → send **two** items, not all of them. The rest is the paid work.

**Never say:** "You wasted your money." · "That was a mistake." · "Your designer ripped you off." (they chose them; you're insulting their judgement)

**Exit ramp:** "You're 90% there — don't rebuild, just close the gap."

---

### W4. "We're locked in with our web company / under contract."

**Frequency & meaning:** a **timing + loyalty + contract** hybrid. Never ask them to break a contract. Give them two paths that work **inside** the constraint: audit now (they implement, or your findings sit ready), or queue the rebuild for renewal. Then — the key move — **get the renewal date**.

**Option 1 — Two paths (default):**
> "Makes sense — don't break a contract over this. Two options: I do the audit now ($500) and *they* implement the fixes, so there's no conflict; or I queue the rebuild for when the contract ends. When does it renew? I'll check back 30 days before."

**Option 2 — Give them a test to run on their current provider (the sharpest version):**
> "Then ask them one question for me: 'show us our mobile conversion path and what AI assistants currently say about us.' If they produce it, you're covered — if they dodge, you have your answer. Want the three questions to ask them?"

**Option 3 — Benchmarked value:**
> "Fair enough. One thing worth checking while you're locked in: what are you actually getting monthly? If it includes [updates, backups, lead tracking], you're in good shape. Most contracts are hosting plus silence. Want me to benchmark what you're paying against what you're getting?"

**Branch tree**

- ⇐ **"They charge monthly, all included."** (≈35% [E])
  ⇒ "Monthly is fine *if* it includes updates, backups and lead tracking. Most don't — they host and vanish. What do you actually get each month? I'll benchmark it in one message, free."
  - ⇐ *"Just hosting, I think."* → "Then you're paying rent on something that isn't growing. Want me to show you what the same money gets you?"
  - ⇐ *"They do everything."* → "Then ask them the three questions — if they pass, stay. Genuinely."

- ⇐ **"It renews in [month]."** (≈30% [E] — the best outcome)
  ⇒ "Perfect — I'll put a reminder 30 days before and message you then. In the meantime, want the audit so you know exactly what to ask for in the renewal? No conflict, no pressure."
  - Log the date. Honour it. This is a **queued deal**, not a lost one.

- ⇐ **"I don't want to upset them."** (≈20% [E])
  ⇒ "Then don't — I'll stay out of the way entirely. The audit is just for you; nobody else sees it. If you never use it, you've lost $500 and learned what your site is missing. Fair?"

- ⇐ **"We're happy with them."** (≈15% [E]) → go to **W1** (specific gap) — the contract is the surface, satisfaction is the real objection.

**Never say:** "You should break that contract." · "You're being ripped off." (unproven and insulting) · "Their work is bad."

**Exit ramp:** "Tell me the renewal date and I'll be useful then — until then, you won't hear from me."

---

### W5. "Why rebuild? Can't you just fix a couple of things?"

**Frequency & meaning:** **the core with-website price objection** and a completely reasonable one. The answer is not "rebuild is better" — it's **patch economics vs. rebuild economics** (§12.4R): patching N scattered issues costs more and leaves the old foundation, and owners who patch usually rebuild within a year anyway — paying twice. But always let them **start with the cheap step** so the decision is only $500, not $1500.

**Option 1 — Patch math (default):**
> "We *can* patch — audit plus priority fixes, $500. Honest take: your site has [N] issues across design, mobile, speed and content. Patching fifteen holes in an old roof costs more than re-roofing, and you still have an old roof. A rebuild fixes all of them at once and adds what the old one can't hold: [booking path / speed / AI-readable structure]. Start with the audit, then decide — you're risking $500, not $1500. Fair?"

**Option 2 — Foundation analogy (cautious owner):**
> "Think of it as a house with good bones versus a bad foundation. Yours has [template-era structure / a slow builder / no mobile base]. I can paint it, or I can rebuild on a base that Google, AI assistants and phones can all read. Want me to show you which camp yours is in — with the actual evidence, not an opinion?"

**Option 3 — Two-step, priced explicitly:**
> "Here's how I'd do it: $500 now for the full written audit and the priority fixes, so you see real improvement this week. If you then want it solved properly, $1500 for the modern rebuild that fixes everything and adds the lead layer. Two separate decisions, no bundling. Want to start with the audit?"

**Branch tree**

- ⇐ **"Just quote me the fixes."** (≈35% [E])
  ⇒ "Will do — but the audit comes first ($500, and it's credited toward the rebuild if you go ahead within 30 days). That way the fixes aren't guesses. Deal?"

- ⇐ **"Why not just do the cheap fixes and stop?"** (≈30% [E])
  ⇒ "You can, and some owners do. The honest caveat: the fixes patch symptoms on a base that's still [slow / not mobile-first / unreadable to AI]. You'll be back in a year — paying twice. But if $500 is what you want to spend now, that's a completely fair place to start."

- ⇐ **"That's a lot for a website."** (≈20% [E]) → go to **U1** (per-client math), then come back to the two-step.
- ⇐ **"Can I see what the rebuild would look like first?"** (≈15% [E])
  ⇒ "Yes — the audit shows what's wrong, and I'll include a short outline of what the rebuild changes. If you like the direction, we go. If not, you still have the fixes."

**Never say:** "Patching is a waste of money." (it isn't, for some) · "You'll regret it." · "Rebuild is the only right answer." (always give them the cheap step)

**Exit ramp:** "Start with the audit — $500, and it's yours either way."

---

### W6. "We get all our business from referrals — the website doesn't bring us clients."

**Frequency & meaning:** a **Need** objection that's often literally true. Never attack referrals — **extend** them. The killer reframe: a referral doesn't end when the phone rings; it ends when the referred person **googles you to check you out**. Your site doesn't replace word-of-mouth — it **closes** it. And there's a second engine now: AI assistants.

**Option 1 — The referral-closer (default):**
> "Referrals are gold — so what does a referred person do first? They Google you. If your site looks dated next to the competitor they *also* got referred to, you lose a referral you already earned. Your site doesn't replace word of mouth — it closes it. Want me to show what a referred customer sees in the first ten seconds?"

**Option 2 — The new referral engine:**
> "There's a new referral engine running in parallel: people ask ChatGPT 'best [trade] in [city]'. No readable site means no recommendation — and the referral goes to whoever the AI *can* read. Want me to run that exact question and send you what it says?"

**Option 3 — The verification step (uses the researched referral-leak logic):**
> "Fair. Here's the part owners don't see: the referral gets you *considered*, then the customer checks you online before calling. Roughly half call anyway; the other half look at the next option — and the one with a proper site gets that call. You never see the ones who didn't call. Want me to show you what that check looks like for your business?"

**Branch tree**

- ⇐ **"We're fully booked anyway."** (≈35% [E])
  ⇒ "That's the best time to fix it — no desperation, you can pick your clients and raise your prices with better positioning. And when the slow season comes, the new site is already earning. Want me to queue the rebuild for [slow month]?"
  - ⇐ *"We're never slow."* → "Then the site's job is different: it lets you charge more and stop taking the jobs you don't want. Want me to show how [a proof-heavy site] does that?"
  - ⇐ *"Maybe after the season."* → date it. Honour it.

- ⇐ **"Show me proof it works in my trade."** (≈30% [E])
  ⇒ "Fair — let's test it on *your* street instead of theory. I'll show you what your listing looks like next to the three competitors who have proper sites, and you tell me which one you'd call. Want the screenshot?"
  - ⇐ *"OK."* → the screenshot. Then one ask.

- ⇐ **"Our customers are old, they don't use the internet."** (≈20% [E]) → go to **W11**.
- ⇐ **"It's not worth it to us."** (≈15% [E]) → "Fair. Then let me ask — what *would* make it worth it? One extra client a month? Two? If I can show you the maths for your numbers, would that change anything?" (U1 math)

**Never say:** "Referrals are dying." (false, and they'll defend them) · "Word of mouth doesn't scale." · "You're leaving money on the table" (vague — show the specific leak instead).

**Exit ramp:** "Your referrals are already working. This just makes sure none of them leak."

---

### W7. "My site is built on Wix / hosted by [X] — I can't move it."

**Frequency & meaning:** a **lock-in + sunk-cost** objection, often believed more strongly than it's true. Never lie about migration difficulty — be honest about what moves, what doesn't, and what they keep. If the platform genuinely can't be improved (no code access, no booking, no speed control), that *is* the argument for a rebuild — stated as a fact, not a criticism of their choice.

**Option 1 — Honest audit of what they'd lose (default):**
> "Fair concern. Here's the honest split: your domain, your content, your photos, and your Google listing all move with you — those are yours. What doesn't move is the template. So the question isn't 'can we move it', it's 'is the template helping you get calls or not'. Want me to check that, and if it's helping, I'll say so?"

**Option 2 — The limitation, stated neutrally:**
> "That's a common setup and there's nothing wrong with it — for a brochure. The limits are [no proper booking path / slow on phones / the platform controls the structure, so AI assistants struggle to read it]. If you're happy with a brochure, keep it. If you want the phone to ring more, the platform is the ceiling. Want the specifics for yours?"

**Option 3 — Keep it, add to it:**
> "Then don't move it — I can build the lead layer alongside it [a landing page with the booking path + the review proof], and your existing site keeps doing what it does. Cheapest path, least disruption. Want to see what that looks like?"

**Branch tree**

- ⇐ **"I paid for that already."** (≈35% [E])
  ⇒ "I know — and I'm not asking you to throw it away. Keep it live while the new one is built, then switch when you're happy. You don't lose anything except the problems. Fair?"
- ⇐ **"Can't you just work inside Wix?"** (≈30% [E])
  ⇒ "Partly — I can improve the words, photos and structure, but I can't fix the speed or the platform's core limitations, because those aren't mine to change. Honest answer: if you want the lead layer, it needs to live on something I control. Want the comparison?"
- ⇐ **"I don't want to lose my Google ranking."** (≈25% [E]) → go to **W9** (the ranking-fear branch).
- ⇐ **"Just tell me what's wrong with Wix."** (≈10% [E]) → "Nothing, for a brochure. Here's the one thing it's costing you: [specific]." (one item, then ask)

**Never say:** "Wix is rubbish." (they chose it, and many businesses run fine on it) · "You have to move." · "I can migrate everything perfectly in a day." (overpromising on a platform you don't control)

**Exit ramp:** "Keep it live — you only switch when you're satisfied. There's no risk in looking."

---

### W8. "We like our design / our brand — we don't want a new look."

**Frequency & meaning:** a **taste + identity** objection, and a legitimate one. Per the operator's own doctrine: a colour or look choice is the owner's call — never argue aesthetics. **Agree with the brand, disagree only about function.** The rebuild pitch is about the *machine under the paint*, and it can keep their look.

**Option 1 — Keep the look, fix the machine (default):**
> "Good — I wouldn't touch the look, that's your brand and it's working. What I'd change is underneath: [speed / mobile layout / the booking path / whether AI can read it]. Same face, better engine. Want me to show you the difference with your current colours and logo?"

**Option 2 — Separate design from function explicitly:**
> "Fair enough — and honestly, your [colours / logo] are recognisable, which is an asset. A redesign doesn't have to mean a new identity; it can mean the same identity built properly. Most of what I'd fix, your customers would never consciously notice — they'd just call more. Want the list?"

**Option 3 — Show, don't tell:**
> "Then let me show you rather than describe it — I'll mock one page using your existing look, and you tell me if it feels like *you*. If it doesn't, we stop there. Fair?"

**Branch tree**

- ⇐ **"We just had it designed, we love it."** (≈35% [E])
  ⇒ "Then keep it. I'm not here to sell you a new logo. The question is whether the site *works* — mobile, speed, booking, AI readability. Want me to check just those four and send you the results? If they're all fine, you'll never hear from me again."
- ⇐ **"Our customers like it too."** (≈30% [E])
  ⇒ "I believe you — and they'd like it *more* if it loaded faster and they could book in one tap. Want me to test those two things on a phone and send you a screenshot? Takes me a minute."
- ⇐ **"So you want to change everything?"** (≈20% [E])
  ⇒ "No — I want to change what's costing you calls. That's usually 4–5 things, and the look isn't one of them. Want me to name them?"
- ⇐ **"Not interested in a new look at all."** (≈15% [E]) → go to **W5** (patch path) — you can still sell the $500 audit.

**Never say:** "Your design looks outdated." (subjective, and it's their call) · "That colour doesn't work." · "You need a rebrand." (bigger, scarier ask than you need)

**Exit ramp:** "Same look, better engine. That's the whole pitch."

---

### W9. "We don't want to lose our Google ranking / our SEO."

**Frequency & meaning:** one of the most **legitimate** objections in this file — and one you must never wave away, because the fear is based on something real: badly executed rebuilds *do* destroy rankings. That's a migration failure, not an inevitability. Answer with the mechanism: **what actually causes the loss** (changed URLs with no redirects, dropped content, broken structure, weeks of downtime) and how you prevent each. Never promise rankings will improve (§12.7).

**Option 1 — Name the real cause, then the prevention (default):**
> "That's the right thing to worry about — and I'll be straight with you: rankings get lost in *bad migrations*, not in rebuilds. The causes are always the same: URLs changed with no redirects, content deleted, or the site down for weeks. I keep the URLs (or redirect them), keep the content that ranks, and build the new one alongside the old one so there's no downtime. Want the migration plan in writing?"

**Option 2 — Audit-first, so nothing is assumed:**
> "Then let's not guess. The $500 audit tells us exactly which pages bring you traffic and which ones are dead weight — so we protect the ones that matter and drop only the ones doing nothing. You'd see the plan before a single thing changes. Fair?"

**Option 3 — Prove it with their own data:**
> "Fair. Let's look at what's actually ranking: if most of your traffic comes from two or three pages, we protect those and rebuild around them — that's a much smaller risk than it feels like. Want me to check which pages are actually bringing people in?"

**Branch tree**

- ⇐ **"Our SEO guy says any change is dangerous."** (≈35% [E])
  ⇒ "He's half right — careless change is dangerous, which is why the plan protects what ranks. Ask him this: 'if we keep the URLs, redirect what changes, and run the new site alongside the old, what breaks?' If he has a real answer, send it to me and I'll work around it. If he doesn't, the fear is bigger than the risk."
  - ⇐ *"OK, I'll ask."* → follow up in 3 days. This is a live deal.
  - ⇐ *"He said no."* → "Then let's do the audit only — it changes nothing on your site, and you'll know exactly where you stand."

- ⇐ **"We rank well already, why risk it?"** (≈30% [E]) → go to **W10**.
- ⇐ **"Can you guarantee we won't drop?"** (≈20% [E])
  ⇒ "No — and anyone who guarantees it is lying. What I *can* do: keep the URLs, redirect the rest, keep the content that ranks, and never take the old site down until the new one is live and checked. If I can't promise the mechanism, I shouldn't be doing the job."
- ⇐ **"Then forget the rebuild, just fix things."** (≈15% [E]) → go to **W5** (patch path — a perfectly good outcome).

**Never say:** "SEO doesn't matter." · "You'll rank higher with me." (unpromised and unprovable) · "Trust me." (they have a professional telling them the opposite — trust isn't the currency here, mechanism is).

**Exit ramp:** "Nothing changes until you approve the plan. That's the safety."

---

### W10. "We already rank on page one / Google works fine for us."

**Frequency & meaning:** a **status-quo** objection with a real basis. Don't argue with their ranking — **separate ranking from conversion**. You can rank and still lose the click, or win the click and lose the call. Also worth checking honestly: they may rank for their own name (which means almost nothing) rather than for the service searches that bring new customers.

**Option 1 — Rank ≠ calls (default):**
> "Good — that's genuinely an asset. The question is what happens *after* they click. If they land and can't find [prices / the booking button / proof], the ranking is doing half a job. Want me to look at the click-to-call path on a phone? That's where the ranking either pays off or leaks."

**Option 2 — Test what actually ranks:**
> "Let's be specific about it — you might rank for your own name, which people only search if they already know you. The searches that bring *new* customers are '[service] [city]'. Want me to run those on a phone and send you what comes up? If you're first on all of them, I'll say so and go away."

**Option 3 — The AI layer (the genuinely new risk):**
> "One thing that's changed: a growing share of people don't scroll Google any more — they ask ChatGPT or Gemini. Those assistants recommend sites they can *read*. Want me to ask them about your business and send you the answer? It's the fastest reality check there is."

**Branch tree**

- ⇐ **"We're number one, we don't need this."** (≈35% [E])
  ⇒ "Then you're in a great position and I'm not going to pretend otherwise. One thing worth checking: does the AI answer include you? If it does, you're genuinely covered and I'll say so. If it doesn't, that's a new gap and it's cheap to close. Want the answer?"
  - ⇐ *"Check it."* → run it, send the screenshot. This is the whole conversation.
- ⇐ **"Rankings change all the time, we're fine."** (≈30% [E])
  ⇒ "They do — and that's exactly why owning a site you control matters more than renting a position. One competitor with a faster, clearer site can take it. Want me to show you who's climbing behind you?"
- ⇐ **"So what would you actually change?"** (≈20% [E] — they're engaging)
  ⇒ name **two** things, concretely, from their site. Then one ask.
- ⇐ **"Not interested."** (≈15% [E]) → go to **U6** (micro-permission), then §0.6.

**Never say:** "You're not really ranking." (unless you've verified it — then say it with the evidence) · "Page one means nothing." (dismissive of a real achievement) · "Rankings will drop if you don't act." (fear-selling without evidence)

**Exit ramp:** "If you're covered on Google and by the AI assistants, leave it alone — genuinely."

---

### W11. "Our industry is different / our customers are older / they don't buy online."

**Frequency & meaning:** a **Need/fit** objection built on a real observation — older customers *do* prefer to phone. But the conclusion ("so I don't need a site") doesn't follow. The data says otherwise: **81% of consumers research a business online before deciding** [S: Google Consumer Research 2025] and **91% read online reviews before visiting a local business** [S: marketingltb 2026]. Older customers still call — but someone researches *for* them first, usually a family member.

**Option 1 — The family-member truth (default):**
> "That's true — older customers call, they don't fill in forms. But here's what actually happens: their son or daughter researches for them. 'Find a roofer for mum' — and whoever looks trustworthy gets the call. A simple site with big reviews and a clear phone number serves both. Who usually calls you — the homeowner, or their family?"

**Option 2 — Reviews are the real product:**
> "Fair. Quick question though: when someone's deciding between you and another [trade], where do they look? Reviews. And reviews live online. Your site is where you get to *show* them properly, instead of hoping they scroll far enough. Want me to show what a customer sees when they check you out?"

**Option 3 — The category test:**
> "Let's not argue about it — let's test it. I'll search '[your service] [your city]' the way a customer would and send you what comes up. If nothing about your business appears, that's the gap. If it does, you're right and I'll drop it. Fair?"

**Branch tree**

- ⇐ **"All my customers come from referrals anyway."** (≈35% [E]) → go to **W6** (referral-closer) or **N1** if they have no site.
- ⇐ **"My trade doesn't work online."** (≈30% [E])
  ⇒ "Then let's find out instead of guessing — what does someone see if they search for [service] in [city] right now? I'll send you the screenshot. If the whole category is offline, I'll tell you. Want it?"
- ⇐ **"I've been fine for 30 years without it."** (≈20% [E])
  ⇒ "And you'll be fine for another 30 — this isn't survival, it's growth. The question is whether you want the next ten years to look like the last ten, or a bit better. Want me to show you what's changed in how people choose?"
- ⇐ **"Send me the proof."** (≈15% [E]) → send the sourced statistic *with its source*, plus one screenshot of their own search results. Never a bare number.

**Never say:** "Your customers are wrong." · "Old people use the internet too, you know." (condescending) · any stat without a source (§0.5).

**Exit ramp:** "Test it yourself — search your own service and city. It takes ten seconds and it doesn't cost anything."

---

### W12. "The site is just informational — we don't sell online."

**Frequency & meaning:** they've confused *e-commerce* with *lead generation*. Most local businesses don't need a checkout; they need a **call or a booking**. Reframe from "selling online" to "being found and being contactable" — which every local business needs regardless of what they sell.

**Option 1 — The call is the conversion (default):**
> "Right — and you don't need to sell online. Nobody's buying a [roof/HVAC job] on a website. The site's job is simpler: get found, prove you're good, and make the phone ring. One tap to call, one tap to book. Is your site doing that on a phone today? Want me to check?"

**Option 2 — What "informational" is costing:**
> "Fair — but 'informational' usually means 'nobody has to act'. That's the leak: a visitor reads, then has no obvious next step, then leaves. One button changes that. Want me to show you where a [trade] site usually loses the call?"

**Option 3 — Compare to what they already do:**
> "You're already selling — you just do it on the phone. The site's only job is to start that phone call more often. So the question isn't 'do we sell online', it's 'does the site make it easy to call us'. Want the honest answer for yours?"

**Branch tree**

- ⇐ **"We don't want online orders anyway."** (≈35% [E])
  ⇒ "Then we won't build any — no cart, no checkout. Just services, proof, and a call button. Simple, and it's exactly what your customers want to do anyway. Want to see the layout?"
- ⇐ **"Our customers just want to talk to someone."** (≈30% [E])
  ⇒ "Perfect — that's what the site is *for*: getting them to the point where they call you instead of the next listing. Right now, does anything on the site tell them to call? Let me check and show you."
- ⇐ **"It's just there so people can find our hours."** (≈20% [E])
  ⇒ "Fair — and how many people find it versus your Google listing? If the listing does that job, the site can do the bigger one: convincing them to choose you. Want me to show the difference?"
- ⇐ **"We're happy with it as is."** (≈15% [E]) → go to **W1**.

**Never say:** "You need e-commerce." (they don't) · "Your site is useless." · "Everyone needs a website." (unprovable and it sounds like a pitch)

**Exit ramp:** "No checkout, no cart — just more calls. That's the offer."

---

### W13. "Our marketing person / our staff / an agency handles all that."

**Frequency & meaning:** an **Authority** objection, but a different flavour: there's a professional in the way. Two rules: **never undermine them** (they chose them, and you'll look like a poacher) and **never let the conversation end with "speak to them"**. Get either the introduction, or a reason to be useful *to them*.

**Option 1 — Be useful to their person, not a rival (default):**
> "Then they'll want this — I've found [N] specific things on the site, and I'm not asking to replace anybody. Send them the list and let them implement it. If they'd rather I did it, that's their call. Want me to write it up so it's easy to forward?"

**Option 2 — Ask what the arrangement actually delivers:**
> "Got it. So I'm not wasting your time — what are they actually responsible for: the site, the ads, or just social? I ask because most of what I find is nobody's job. Want me to check whether your site's covered or whether it's falling between the cracks?"

**Option 3 — Position as the specialist:**
> "Makes sense — and a general marketing person doing the site on the side is normal. I only do [trade] websites, which is why I spot things a generalist doesn't. Want to test that? I'll send two things they missed; if they didn't miss them, I'll shut up."

**Branch tree**

- ⇐ **"They handle everything, we're covered."** (≈35% [E])
  ⇒ "Then you're in a good spot. One question that settles it: ask them what ChatGPT currently says about your business. If they know, you're genuinely covered. If they don't, that's the gap — and it's a new one, not their fault. Want me to check it first so you have the answer?"
- ⇐ **"I'd have to ask them."** (≈30% [E]) → go to **U10** (get the introduction), then **W4** (working alongside).
- ⇐ **"It's my wife / my son who does it."** (≈20% [E]) → go to **W2** (honour the relative, differentiate).
- ⇐ **"We don't have anyone."** (≈15% [E] — the crack)
  ⇒ "Then that's exactly why you're hearing from me. Nothing gets updated because nobody owns it. Want me to take it off the pile — one price, and you never think about it again?"

**Never say:** "They're doing a bad job." · "You should fire them." · "Agencies overcharge." (their judgement is being questioned and you'll lose the room)

**Exit ramp:** "Even if they keep it, the list is useful to them. That's a win for you either way."

---

### W14. "We tried a redesign before and it made things worse."

**Frequency & meaning:** a **trust objection with evidence** — the worst kind, because they're right about something that actually happened. Almost always the same cause: a bad migration (rankings lost, mobile made worse, the old content deleted, or the site abandoned half-built). Diagnose the specific failure, then show how you prevent *that exact one*.

**Option 1 — Diagnose first (default):**
> "That's frustrating, and more common than you'd think. What actually got worse — did you lose your Google position, did it get slower on phones, or did it just never get finished? Tell me the one thing, and I'll show you exactly how I'd stop that happening."

**Option 2 — Name the usual causes:**
> "Almost every redesign that goes wrong does it one of three ways: the old pages were deleted instead of redirected, it was built without checking on a phone, or it was launched before it was finished. All three are avoidable. Want me to check your old site against those three and tell you which one hit you?"

**Option 3 — Risk-reversed process:**
> "Then we do it differently this time: the new site gets built *alongside* the old one, nothing goes live until you've approved it on your own phone, and the old one stays up until the new one's working. If it's not better, you don't switch. Want the plan?"

**Branch tree**

- ⇐ **"We lost our Google ranking."** (≈35% [E]) → go to **W9** (migration mechanism).
- ⇐ **"It cost a fortune and never got finished."** (≈30% [E]) → go to **U13** (structure: 50/50, ownership, checkpoints).
- ⇐ **"It looked worse."** (≈20% [E])
  ⇒ "Then that's a design-process failure — they didn't show you before they built. I show you a rough version first, so you can say 'that's not us' at the cheap stage. Want to see how that works?"
- ⇐ **"I'm not doing it again."** (≈15% [E])
  ⇒ "That's fair, and I won't push. If you ever want a free second opinion on what you were left with — no charge, no pitch — just reply. Good luck." (clean exit; burned owners remember who didn't push)

**Never say:** "They did it wrong." (even if true — you're insulting their decision) · "It'll be different this time, I promise." (a promise, not a mechanism) · "You should have used a contract."

**Exit ramp:** "Built alongside, approved on your phone, old site stays live. That's the fix for what happened last time."

---

### W15. "How do I know you won't break my site / take it down / disappear mid-project?"

**Frequency & meaning:** the **risk** objection, usually raised by an owner who's already been burned once. The answer is never reassurance — it's **structure**: staging, approval, backups, ownership, and a payment split. Name the four boundaries in writing (scope, ownership, liability, acceptance) [S: gruv.ai].

**Option 1 — The structure list (default):**
> "Fair question. Four things: the new site is built separately and your live one stays up until the new one's checked; you approve it on your own phone before anything switches; you own the domain and the files from day one; and you hold half the money until it's live. I can't break something I don't control. Want that written out?"

**Option 2 — Name their specific fear:**
> "Which part worries you most — the site going down, or me not finishing? Because they're different problems with different fixes, and I'd rather answer the one that's actually bothering you."

**Option 3 — Give them the exit before they ask:**
> "Here's the honest deal: if at any point you're not happy, you keep everything built so far, you keep the domain, and you don't pay the second half. The worst case for you is a half-finished site you own and half a payment. Is that an acceptable risk? If it isn't, I'd rather know now."

**Branch tree**

- ⇐ **"What if you disappear?"** (≈35% [E]) → go to **U13** (the burned-before structure).
- ⇐ **"What if it breaks after launch?"** (≈30% [E])
  ⇒ "Then you message me and I fix it — that's included for the first [30 days]. After that it's small stuff you'd text me about. And you own the files, so any other developer can pick it up. You're never locked to me."
- ⇐ **"I don't understand any of this, that's the problem."** (≈20% [E])
  ⇒ "Then you shouldn't have to. That's my job: I do the technical side and hand you one short video at the end so you can change your phone number yourself if you want. You'll never need to know what a redirect is. Fair?"
- ⇐ **"I need to think about the risk."** (≈15% [E]) → go to **U2**, then offer the smallest possible first step (the $500 audit changes nothing on their site).

**Never say:** "Nothing can go wrong." · "Trust me, I've done this a hundred times." · "It's really simple." (dismissive when they've told you they're nervous)

**Exit ramp:** "Start with the audit — it changes nothing on your live site, and you'll see how I work before you risk anything."

---

## Section 2 — NO-WEBSITE owners only (they have no site at all)

> Use **after** §0. These owners live on Google Maps and social. Every hook must cite **their own listing fact** — rating, review count, trade, city, the empty website field — or you're a template (§12B.3). Channel is **email or FB/IG/X/Reddit DM**; in this mode **phones are banned entirely** — no calls, no SMS, no WhatsApp, never a phone as the contact channel (§3B.3). DM replies should be **≤80 words**.
>
> **Context worth knowing:** **27%** of small businesses still have no website [S: Smart Soft Solutions 2025], and in trades it's much higher — plumbing and cleaning **40–65%**, landscaping **35–55%**, HVAC and electrical **35–50%**, auto repair **30–45%** [S: LeadsAgent estimates]. They're not failing businesses; they're referral-driven ones that **don't see the losses**, because the customer who didn't call is invisible. Their sales cycle is short — most decide in **1–2 contacts over 3–10 days** [S: LeadsAgent], which is why a clear, low-friction DM beats a polished pitch.

### N1. "I don't need a website — word of mouth keeps me busy."

**Frequency & meaning:** the **#1 reason** no-website owners give [S: LeadsAgent], and it's usually **true and honest, not hostile** [S: GetMapLeads: "it is not a considered position — it is a reflex… the objection is not hostile, it is honest"]. Never attack referrals. Show the **invisible leak**: the referral gets you *considered*, then the customer verifies you online — and roughly **half call anyway, half look at the competitor with a site** [S: LeadsAgent observed 50/50 rule]. The owner never sees the half that didn't call.

**Option 1 — The Google check (direct/logical):**
> "That's great — it means your work is good. Quick question: when a referred customer Googles '[Business] [city]', what do they find? Right now it's [your Maps listing with no website link]. Half of them will call anyway. The other half look at the competitor with photos, prices and a Book button. Your referrals earn the lead — the missing site loses half of them. Want the screenshot of what they see?"

**Option 2 — The young-customer angle (story/cautious):**
> "Other [trade] owners told me the same — until their own kids said 'Dad, nobody calls without checking online first.' Under-40 customers don't call blind, they compare. A simple site with your reviews, photos and a call button catches the ones your referrals already sent you. Want a mock of your homepage — no charge?"

**Option 3 — Extend, don't contradict (the highest-trust framing [S: GetMapLeads]):**
> "That's brilliant — and a website wouldn't replace that at all. It just means when those referrals Google you before calling to check you out, they actually find you instead of nothing. Do you know what comes up when someone searches your business name right now?"

**Branch tree**

- ⇐ **"I'm fully booked, go away."** (≈30% [E])
  ⇒ "Best problem to have! Two options: raise your prices with better positioning (a proper site is premium proof), or bank a waitlist for the slow season. I can queue the build for [slow month] — want me to check back then with the mock ready?"
  - ⇐ *"We're never slow."* → "Then the site's job is different — it lets you stop taking the jobs you don't want and charge more for the ones you do. Want me to show how?"
  - ⇐ *"Maybe after the season."* → date it, honour it.

- ⇐ **"Show me proof websites bring clients in my trade."** (≈30% [E])
  ⇒ "Fair — so let's use your street, not theory. **[81% of consumers research a business online before deciding** [S: Google Consumer Research 2025], and **91% read reviews before visiting a local business** [S: marketingltb 2026].] Right now you're invisible at that exact moment. I'll send you a screenshot of your listing next to the [trade] who has a site — you tell me which one you'd call."
  - ⇐ *"OK."* → the screenshot. Then one ask. No more statistics than this.

- ⇐ **"My customers are all older, they don't go online."** (≈25% [E]) → go to **N6**.
- ⇐ **"It's working fine as it is."** (≈15% [E])
  ⇒ "Then let me ask the one question that settles it: what comes up when someone searches your name? If it's a full picture of your business, you're right and I'll go away. If it's an empty listing, that's the gap. Want me to check?"

**Never say:** "Word of mouth is dying." (false, and they'll defend it) · "You're losing money" without a sourced, reasoned figure (§12.6) · "Everyone needs a website."

**Exit ramp:** "Your referrals already work — this just stops half of them leaking."

---

### N2. "My Facebook / Instagram / Google Maps page is enough."

**Frequency & meaning:** a **Need** objection from an owner who's built a real audience — and they're **not wrong that it works**. The three wedges are: you don't own it (the algorithm decides who sees you), it can't be searched properly (customers who want prices/menu/booking have to scroll), and **AI assistants can't recommend a Facebook page** [S: LeadsAgent: the journey is Google → website → call; Facebook is a different lane]. Never trash their page — position the site as the **amplifier**.

**Option 1 — You don't own it (direct/logical):**
> "Your page is strong — keep it. The risk is that Facebook decides who sees your posts, and Maps shows your competitors right next to you. A website is the one place you own: every post and listing points *there* to book. Facebook brings attention; the site catches it. Want me to show how your best post would convert with a Book button behind it?"

**Option 2 — Customer behaviour (story):**
> "Fair — but where does a customer go on your Facebook page when they want prices, or before-and-afters, or to book? They scroll through fifty posts. On a site it's one tap. And ChatGPT can't recommend a Facebook page properly — it recommends sites with readable services. Want me to run that test for '[trade] [city]' and send you what it says?"

**Option 3 — Amplify, don't replace (highest-trust):**
> "Then the site makes your Facebook *more* profitable: 'link in bio' goes to your own booking page instead of Messenger chaos. Less back-and-forth, more booked jobs. What do you sell most over Messenger? I'll mock that one page so you can see it."

**Branch tree**

- ⇐ **"My customers are all on Facebook anyway."** (≈35% [E])
  ⇒ "Then you're exactly who this works for. Right now every enquiry comes through Messenger, which means you're answering the same five questions all day. A one-page site answers them for you and takes bookings while you're on a job. Want to see the one page I'd build for you?"
  - ⇐ *"Show me."* → the mock. Then one ask.

- ⇐ **"A website costs money, Facebook is free."** (≈30% [E])
  ⇒ "Facebook is free *until* it isn't — one algorithm change and your reach halves. And it's rented: you don't own your followers. The site is the only asset you own outright. Want me to show what the same effort gets you on a site you control?"
  - ⇐ *"Still free though."* → "True. Free plus rented versus $[X] once and owned. Which one do you want to be building on for the next five years?"

- ⇐ **"I don't have time to run a website too."** (≈20% [E]) → go to **N4** (done-for-you) or **U7**.
- ⇐ **"I tried a site before and Facebook did better."** (≈15% [E]) → go to **N5** (diagnose the dead site).

**Never say:** "Facebook is a waste of time." · "Your page is bad." · "Social media doesn't work for business." (it demonstrably does — for attention)

**Exit ramp:** "Keep the page — the site just makes it pay."

---

### N3. "A website is too expensive / I was quoted thousands once."

**Frequency & meaning:** the same **price** objection as **U1** (35% of all objections [S: Salesforce 2025]) but with a specific history: no-website owners have often been quoted **$3,000–$10,000** by agencies [S: LeadsAgent]. So the anchor in their head is enormous and your price looks like either a bargain or a scam. **Use U1 for the handling logic** — this entry only covers what's different: the agency anchor and the starter slice.

**Option 1 — Agency vs. local (direct/logical):**
> "Agencies charge $3–10k because they're selling to companies with marketing departments. I build only for local [trade] — one focused site with services, reviews, click-to-call and booking for $[X], 50/50. No $10k machine, no retainer. Want the exact list of pages you'd get?"

**Option 2 — Starter slice (cautious):**
> "We can start below that: a one-page site with your services, reviews and a call button, live in days. Most owners add pages later out of profit, not savings. Want the starter scope?"

**Option 3 — Anchor to what they already spend:**
> "Fair — but compare it to what you already spend: one month of [van ads / a truck payment / insurance] is about the same as the whole site, once. The site doesn't expire. Want me to show what the same money gets you here?"

**Branch tree**

- ⇐ **"Still a lot for something I've lived without."** (≈35% [E]) → **U1 Option 1** (per-client math), then: "…and you've lived without it while losing roughly [one client a month]. The site costs once; the gap costs monthly."
- ⇐ **"Can you do it for less?"** (≈30% [E])
  ⇒ "I can do *less* for less — a smaller version, not a discount on the same thing. Want to see what the one-page version covers?"
  - ⇐ *"Yes."* → scope it. Never discount the full build to match the reduced scope's price.
- ⇐ **"I need to think about it."** (≈20% [E]) → go to **U2**.
- ⇐ **"My nephew will do it cheaper."** (≈15% [E]) → go to **U12**.

**Never say:** "It's only $[X]." (diminishing their money) · "You can't afford not to." (pushy) · a reflexive discount (§0.1 law 5).

**Exit ramp:** "Start small — one page, live in days, expand when it earns."

---

### N4. "I'm not technical — who updates it? It'll break or get hacked."

**Frequency & meaning:** a **capacity + risk** objection. They're picturing themselves maintaining a machine they don't understand. The fix is **done-for-you** plus **ownership clarity** — they own it, you maintain it, updates are a message away. Hacking fear is real but easily addressed: a simple, fast, static-style build with backups is far *less* attractive to attackers than a bloated CMS.

**Option 1 — Done-for-you (default):**
> "You never touch it. I write everything from your [Facebook posts / price list], set up the call button and the reviews, and hand you one five-minute video — how to change your phone number, that's it. Updates: you message me and I do them. Hacked? There's nothing to hack on a simple site, and I keep backups — I can restore it in an hour. Want the video sample?"

**Option 2 — Proof by example (cautious):**
> "Look at [a past client's site] — the owner's a [55-year-old plumber] and he hasn't logged in once in a year. That's the point: you run the jobs, I run the site. Fair split?"

**Option 3 — Turn "not technical" into an advantage:**
> "Honestly, that's better for me — owners who 'know a bit' break things. You tell me what you want changed, I do it properly. You never see a control panel. Does that sound like less hassle than what you're imagining?"

**Branch tree**

- ⇐ **"What if you disappear like the last guy?"** (≈30% [E]) → go to **U13** (structure: 50/50, they own everything, checkpoints).
- ⇐ **"I don't want a monthly bill."** (≈25% [E]) → go to **N16**.
- ⇐ **"I've heard sites get hacked all the time."** (≈25% [E])
  ⇒ "Big WordPress sites do — they're targets. A simple fast site with no plugins is boring to hackers. And it's backed up, so even in the worst case it's restored in an hour. Is that the worry, or is it something else?"
- ⇐ **"I don't have time to learn it."** (≈20% [E])
  ⇒ "You won't learn anything — that's the deal. Thirty minutes total, and you'll never open a dashboard. Want me to show you the five-minute video so you can see how little there is to know?"

**Never say:** "It's easy, you'll pick it up." (they told you they don't want to) · "You'll have full control of the backend." (that's the fear, not the selling point) · "Hacking is impossible."

**Exit ramp:** "You never touch it. That's the whole offer."

---

### N5. "I tried a website before — it was a waste of money, it brought nothing."

**Frequency & meaning:** a **Need + trust** objection backed by real experience. This is actually a **gift**: they've thought about it, tried it, and been disappointed — which means the problem is **diagnosable**, and diagnosis is exactly what you're good at [S: GetMapLeads: "this is actually a valuable opening"]. The three usual causes: never found on Google, no call button on mobile, or launched and abandoned.

**Option 1 — Diagnose (default, LAER Explore):**
> "I'm sorry — that's money gone. What did it actually do? Most dead sites fail the same three ways: nobody could find them on Google, there was no call button on a phone, or it was launched and then abandoned. Which one was yours? Tell me one and I'll show you how mine avoids exactly that."

**Option 2 — Before/after (story):**
> "A pretty page with no booking path *is* a waste — I'd have been annoyed too. Mine is built backwards from the call: every page ends in 'call' or 'book'. Want me to tear down your old one (if it's still up) next to my layout — three screenshots?"

**Option 3 — Free diagnostic on the old site (the strongest, because it's concrete):**
> "If you still have the old address, send it to me. I'll check it the way a customer would — search it, open it on a phone, try to book — and tell you honestly what was wrong. Free, no pitch. If it turns out it was fine and just never got traffic, I'll tell you that too."

**Branch tree**

- ⇐ **"It was Wix and I paid monthly for years."** (≈30% [E])
  ⇒ "Then you paid for the *tool* and nobody built the machine. Hosting isn't marketing. I build the machine once — $[X], and you own it. Want the cost breakdown?"
- ⇐ **"Nobody ever found it."** (≈30% [E])
  ⇒ "That's the most common one, and it's fixable — a site with no location pages and no review proof is invisible. Want me to show you what 'findable' looks like for a [trade] in [city]?"
- ⇐ **"I paid a lot and got nothing."** (≈25% [E]) → go to **U13** (structure) — the real objection is trust in providers, not the website.
- ⇐ **"I'm not trying again."** (≈15% [E])
  ⇒ "That's fair and I won't push. If you ever want the free diagnosis on the old one, just reply. Good luck." (exit clean)

**Never say:** "You were scammed." (even if true — it makes them feel foolish) · "That site was terrible." · "Things are different now." (a claim, not a diagnosis)

**Exit ramp:** "Send me the old address and I'll tell you what went wrong — free."

---

### N6. "It won't work for my trade / my town is small / my customers are old."

**Frequency & meaning:** a **fit** objection built from genuine local knowledge. Three sub-cases, three different answers: **small town** (fewer competitors with sites = *easier* to own the search), **old customers** (their family researches for them), **"my trade is different"** (test it instead of debating it). Always offer the **test** — it converts a belief into evidence.

**Option 1 — Small town (direct/logical):**
> "Small town is actually the *easier* case — fewer competitors with proper sites, so owning the search is quicker. Let's test it: search '[trade] [city]' right now. See the three with sites taking the calls? And your Maps listing sits next to them with no link. Want the screenshot of your own search street?"

**Option 2 — Older customers (story):**
> "Older customers call — but their kids research for them. 'Find a plumber for mum' — and whoever looks trustworthy gets that call. One page with big reviews and a clear phone number serves both. Who usually calls you, the homeowner or their family?"

**Option 3 — Test, don't argue (confident):**
> "Let's settle it with evidence rather than opinions. I'll search the way a customer would, in your town, for your service — and send you exactly what comes up. If your competitors are all invisible too, I'll say so. Want it?"

**Branch tree**

- ⇐ **"Everyone in my town knows me."** (≈35% [E])
  ⇒ "Then the site is your 24/7 shop window on the main street — which is Google. Newcomers, tourists, and your neighbours' kids don't know you yet. They search. Want the mock with your town name on it?"
- ⇐ **"My customers are older, they call."** (≈30% [E]) → **Option 2** above, then: "So the site's job is to get you *chosen* before they dial. Want me to show what that looks like?"
- ⇐ **"My trade is different, we don't get found online."** (≈20% [E])
  ⇒ "Then let's check rather than assume — what do you get if you search your own service in your town? I'll send the results. If the whole category is offline, you're right and I'll drop it."
- ⇐ **"I don't want strangers calling."** (≈15% [E]) → go to **N10**.

**Never say:** "Everyone's online now." (they know their customers better than you) · "You're wrong about your own town." · "Just trust me."

**Exit ramp:** "Search it yourself — ten seconds, no cost. Then decide."

---

### N7. "I'm too small / it's just me / I'm retiring soon / it's a side job."

**Frequency & meaning:** a **fit + timing** hybrid, and one of the few where the honest answer can be **"then don't"**. Three sub-cases: **solo operator** (being small is a selling point — "the owner does every job"), **side job** (a one-pager is enough), **retiring** (a site adds sale value — the buyer gets lead flow, not just tools). Never sell a dying business a project; that burns goodwill and referrals.

**Option 1 — Solo is the premium (direct):**
> "Solo is a *selling* point — 'the owner does every job' beats a faceless company. A one-pager with your face, your reviews and a call button lets you charge more and pick the jobs you want. Want the solo-owner layout?"

**Option 2 — Exit value (for the retiring owner):**
> "If you're thinking of selling in the next few years, this matters: businesses with a site and a Google presence sell for more, because the buyer is paying for lead flow, not just tools. $[X] now can add real value at the sale. When are you thinking of selling?"

**Option 3 — Honest disqualification (the trust builder):**
> "Straight answer — if you're winding down within a year, don't build it. It won't pay back. I'd rather tell you that than take your money. Can I check back in [month] in case plans change?"

**Branch tree**

- ⇐ **"I'm closing in a few months."** (≈30% [E])
  ⇒ "Then don't build — genuinely. I'll close your file. If plans change, or if the person taking over wants it, send them my way. Good luck." (never hard-close a dying lead — they refer [§0.5])
- ⇐ **"I'm too small for a website."** (≈30% [E])
  ⇒ "You're too small for a *complicated* one — you're not too small for a one-pager. It's one page, your services, your reviews, a call button. Small businesses are exactly who I build for. Want to see what it looks like?"
- ⇐ **"It's just a side thing right now."** (≈25% [E])
  ⇒ "Then the one-pager is right, and we grow it if the side thing takes off. Want me to scope the smallest version that still looks professional?"
- ⇐ **"I'll do it when I'm bigger."** (≈15% [E]) → go to **N8** (timing).

**Never say:** "You're too small to compete." · "You need to think bigger." · anything that makes their scale feel like a failing.

**Exit ramp:** "If it's not going to pay back for you, I'd rather say so."

---

### N8. "Maybe later / next year / it's not a priority right now."

**Frequency & meaning:** the **timing** bucket — and in no-website mode, note the nuance from the data: these owners decide **fast** (1–2 contacts, 3–10 days) *when* they decide [S: LeadsAgent], so a "later" usually means **the value hasn't landed yet**, not that they're genuinely planning for next year. Shrink the ask and **put a date on it**. One in this category is actually a buying signal: *"I've been meaning to get a website but haven't gotten around to it"* — that's the most qualified lead you'll ever get [S: LeadsAgent]; they just need it made easy.

**Option 1 — Seasonal queue (default):**
> "Fair — when's your busy season? I'd rather build in your slow month so it's live and earning *before* the rush, instead of half-finished while you're slammed. Which month is worst for you?"

**Option 2 — Zero-effort starter (cautious):**
> "No project needed now. Give me ten minutes — or nothing at all, I'll build the mock from your Facebook page — and you look whenever you're ready. No expiry, no pressure. Want me to start the mock?"

**Option 3 — Catch the "been meaning to" signal:**
> "Sounds like it's been on the list a while. Here's the thing — I can have something ready for you to look at in about a week, and you'd only need to say yes or no. If you've been meaning to do it, this is the cheapest version of meaning to. Want me to start?"

**Branch tree**

- ⇐ **"After [season]."** (≈35% [E]) → log the exact month, honour it, **don't touch them before**.
- ⇐ **"AI / my kid will do it later."** (≈25% [E]) → go to **U12**, adapt: "Have them build one page and send it — I'll grade it free against what makes a [trade] site bring calls. If it passes, you saved $[X]."
- ⇐ **"I just don't have the money right now."** (≈25% [E]) → go to **U1** (per-client math) or **N3** (starter slice).
- ⇐ **"It's not a priority."** (≈15% [E])
  ⇒ "Fair enough. One question then — is it not a priority because it wouldn't help, or because nothing's forcing it? If it's the second one, can I check back in [month]?" (U2 permission-to-say-no)

**Never say:** "You're losing money every day you wait." (unproven, and it's fear-selling) · "This price is only good this week." (fake urgency) · "I'll keep following up until you're ready." (threat)

**Exit ramp:** "I'll come back in [month] — and if it's still a no then, just say no."

---

### N9. "I only need Facebook ads / TikTok — not a website."

**Frequency & meaning:** a **channel** objection from an owner who's already spending on ads (or thinking about it). The argument isn't "ads are bad" — it's the **leaky bucket**: ads without a site send paid clicks nowhere, so the same spend converts worse. Also worth checking: **88% of visitors leave after a poor mobile experience** [S: Google 2025], which is exactly what a Facebook page or a weak link does to an ad click.

**Option 1 — The leaky bucket (direct/logical):**
> "Ads without a site is paying to send people nowhere — a Facebook page with Messenger chaos. Ads *with* a one-pager: every click can book. Same ad spend, more bookings. Where do your ad clicks land today? I'll show you the leak in one screenshot."

**Option 2 — Rent vs. own (story):**
> "One month of ads is about $[X] and then it's gone. A site is $[X] once and it keeps working — and it makes every *future* ad cheaper, because a fast landing page is cheaper to send traffic to. Ads rent attention; a site owns it. Want the maths for your spend?"

**Option 3 — Ad-to-page match (the practical version):**
> "Fair — keep running ads. Just give the clicks somewhere to land that's built to convert: one page, your service, your reviews, a Book button. That's the difference between paying per click and paying per customer. Want me to mock the page your current ad should point at?"

**Branch tree**

- ⇐ **"I don't run ads, I just post on Facebook."** (≈35% [E]) → go to **N2** (the page-as-home objection).
- ⇐ **"Ads bring me enough work."** (≈30% [E])
  ⇒ "Then they'd bring more with somewhere better to land. One question: what happens to a click that *doesn't* book immediately? On Facebook they're gone forever. On a site you can bring them back. Want me to show you what that's worth?"
- ⇐ **"I don't want to pay for both."** (≈20% [E])
  ⇒ "Then start with the site — it makes the ads work better, so you spend less on them. And you don't have to run ads at all. Want the version that works without ads?"
- ⇐ **"TikTok brings me younger customers."** (≈15% [E])
  ⇒ "Then the site is what catches them after the video — a link in bio that books instead of a Messenger thread. Want the one page your TikTok should point at?"

**Never say:** "Ads don't work." · "Social media is a waste." · any invented conversion number.

**Exit ramp:** "Keep the ads — just give them somewhere to land."

---

### N10. "I'm fully booked / I don't want more customers / I don't want tyre-kickers."

**Frequency & meaning:** a **genuine no-need objection** — and one of the few where the right answer isn't more volume. Three legitimate paths: **charge more** (a proper site is premium proof), **filter better** (a site that shows services and prices screens out the tyre-kickers), and **bank the overflow** (a waitlist for the slow season). Never sell them "more leads" — that's not their problem.

**Option 1 — Position, not volume (default):**
> "Then this isn't about more customers — it's about *better* ones. A proper site with your prices and services up front filters out the tyre-kickers and lets you charge more for the jobs you actually want. Want me to show what that looks like?"

**Option 2 — The season bank (story):**
> "That's the best position to be in. Two things worth doing: raise your prices (a solid site is the proof you need to justify it), and have somewhere to send the overflow so the slow season isn't a cliff. Want me to show how a waitlist page does that?"

**Option 3 — Tyre-kicker filter (practical):**
> "Tyre-kickers come from *not* saying what you do and what you charge. A page that lists your services, your area, and a starting price scares off the time-wasters before they message. Want me to mock the page that does exactly that?"

**Branch tree**

- ⇐ **"I'm booked solid for months."** (≈40% [E])
  ⇒ "Then you can raise your prices and let the market tell you. The site is what makes a higher price look justified instead of cheeky. Want to see what I mean?"
- ⇐ **"I really don't want more work."** (≈30% [E])
  ⇒ "Understood — then don't build it for more work. Build it so the work you take is better paid and less annoying. That's a different job and it's the one I'd do. Still not interested?"
  - ⇐ *"Not really."* → go to **U6** (micro-permission + graceful exit).
- ⇐ **"If I got more calls I couldn't handle them."** (≈20% [E])
  ⇒ "Then that's a pricing problem, not a website problem — you're undercharging. Want to see what the same jobs at a higher price look like? It's cheaper than hiring."
- ⇐ **"Let's talk next year."** (≈10% [E]) → go to **N8** (date it).

**Never say:** "You'll lose customers if you don't." (they're turning work away) · "You're leaving money on the table." (vague) · anything implying they're being irrational.

**Exit ramp:** "If you're full, you don't need leads — you need better-paying ones. That's a different offer."

---

### N11. "I don't use email — just call me." (channel objection)

**Frequency & meaning:** very common with no-website owners, who are phone-first. **Handle with care — this is the one objection where the "obvious" answer is forbidden.** In `no_website` mode, phones are **never** a contact channel: no calls, no SMS, no WhatsApp, and a phone can never appear as the contact route (§3B.3). The move is to **redirect to a channel they already use** — Facebook or Instagram DM — and make it feel like *their* convenience, not your limitation.

**Option 1 — Redirect to the DM they already use (default):**
> "No problem at all — I'll message you on Facebook instead, same as your customers do. Saves us both a phone call and I can send you the actual screenshots so you can see what I mean. Is your Facebook page the best place to reach you?"

**Option 2 — Frame messaging as the better medium (practical):**
> "Fair — but let me send it over message instead of calling, because half of what I'd tell you is screenshots of your own listing. Easier to see than to describe. Which do you check more — Facebook or Instagram?"

**Option 3 — The honest boundary (if they insist on a call):**
> "I get it — honestly I'd rather keep it in messages so you have everything in writing and can look whenever suits you. If it's easier, send me a message here whenever you're free and I'll reply the same day. Does that work?"

**Branch tree**

- ⇐ **"I never check Facebook messages."** (≈30% [E])
  ⇒ "Then which one do you actually check — Instagram, or your Google listing messages? I'll use whichever you already look at. I just want it somewhere you'll actually see it."
- ⇐ **"Just call me, it's faster."** (≈30% [E])
  ⇒ "I work over messages so you've got everything written down — no pressure, no sales call, and you can reply at 9pm when the jobs are done. Send me a message whenever and I'll take it from there." *(Do not call. Do not offer to call. §3B.3.)*
- ⇐ **"Why won't you just call?"** (≈25% [E])
  ⇒ "Honest answer: I work across time zones and messages keep everything in one place — you get the screenshots, you reply when it suits you. Nothing gets lost. Fair?"
- ⇐ **They give an email anyway** (≈15% [E]) → use it. Email is a valid channel.

**Never say:** "I can't call." (sounds like something's wrong with you) · "Let me get your number." · any offer to call, text, or WhatsApp — **in `no_website` mode this is a critical failure** (§3B.3). Never log a phone as the contact channel.

**Exit ramp:** "Message me here whenever — I'll reply the same day."

---

### N12. "Who owns it? What happens if I stop paying?"

**Frequency & meaning:** a **rental/ownership fear** — and a smart one, usually learned from a bad experience or from watching someone else lose a site. This is where you win by **giving away control**: the domain is registered in *their* name from day one, the files are theirs, and there is no monthly hostage. The stronger your ownership terms, the faster this objection dies.

**Option 1 — Ownership up front (default):**
> "Yours, from day one. The domain is registered in *your* name, the site files are yours, and there's no monthly fee to keep it alive — you just pay for hosting, which is a few dollars a month paid directly to the host. If you stopped working with me tomorrow, everything still works. Want that in writing before we start?"

**Option 2 — Contrast with the alternative (story):**
> "Fair question — and it's the difference between me and the platforms. On Wix or a rent-a-site, you stop paying and it's gone. With me you own the thing. I'd rather you owned it, because then you're never stuck with me. Does that matter to you?"

**Option 3 — Kill the retainer fear directly (practical):**
> "Let me be clear about the money: $[X] once, then hosting which is a few dollars a month paid to the host, not to me. No retainer, no lock-in, no monthly fee to *me*. If you want me to make updates later, that's a separate thing you ask for. Fair?"

**Branch tree**

- ⇐ **"So there's no ongoing fee?"** (≈35% [E])
  ⇒ "Only hosting — a few dollars a month, paid straight to the host, and you keep the receipt. I don't take a cut of your own website. If you want me on call for changes, that's optional and separate."
- ⇐ **"What if I want to leave?"** (≈30% [E])
  ⇒ "Then you leave with everything — domain, files, the lot. I'll hand over the logins and that's it. No exit fee, no hostage situation. That's the deal from the start."
- ⇐ **"Can I own the domain myself?"** (≈20% [E])
  ⇒ "You *should*. Register it in your own name and give me access — that way you're never dependent on me for the most important piece. I'll walk you through it if you haven't done it before."
- ⇐ **"This sounds too good."** (≈15% [E])
  ⇒ "It's just normal — most people in my position rent you your own site because it's easier for them. I'd rather you owned it. Want me to send the terms so you can check them properly?"

**Never say:** "I keep the domain for security." (red flag, and it's exactly what burned them) · "There's a small monthly management fee." (unless it's genuinely optional) · "You'll have full access after final payment." (hostage framing)

**Exit ramp:** "Domain in your name, files yours, no retainer. That's the whole arrangement."

---

### N13. "What do you need from me? How long does it take?"

**Frequency & meaning:** **not really an objection** — it's a buying signal wearing a logistics question. They're picturing the project. Answer with a **small number** (time) and a **short list** (inputs), because the fear is that this will become a second job. Local owners decide fast when the effort is near zero [S: LeadsAgent].

**Option 1 — Small numbers (default):**
> "About thirty minutes of your time, total: one conversation now and one design approval later. Everything else I build from your [Facebook posts / photos / price list]. Live in about [N] days. Does that work for you?"

**Option 2 — Nothing-needed version (cautious):**
> "Nothing to start — I'll build the first version from what's already public: your photos on Maps, your services, your reviews. Then you tell me what to change. You literally don't have to prepare anything. Want me to start with that?"

**Option 3 — Milestone clarity (practical):**
> "Three steps: (1) I build a rough version, you say 'that's us' or 'change this'; (2) I finish it and you check it on your own phone; (3) it goes live on your domain. You're involved twice, briefly. Fair?"

**Branch tree**

- ⇐ **"I don't have any photos."** (≈35% [E]) → go to **U18** (four phone photos, that's it).
- ⇐ **"I don't have time."** (≈30% [E]) → go to **U7** (shrink the ask) or **N4** (done-for-you).
- ⇐ **"How long exactly?"** (≈25% [E])
  ⇒ give a **realistic, modest** number and then under-promise slightly: "[N] days for the first version; call it [N+2] to be safe." Never promise a timeline you can't hold — §12.7.
- ⇐ **"Send me the list."** (≈10% [E]) → send three bullets, not a form. Then one ask.

**Never say:** "It's a big project, but…" (kills it) · "I'll need all your content first." (that's the fear) · an aggressive timeline you'll miss.

**Exit ramp:** "Thirty minutes of you, a week of me. That's the trade."

---

### N14. "Will it be in my language? My customers don't all speak English."

**Frequency & meaning:** a **service-fit** question that is often a **hidden opportunity**: in many markets the local competition is English-only, so a bilingual site reaches a whole customer segment nobody else is serving. Answer honestly about what you can actually write — **never promise a language you can't produce professionally** (§12.7).

**Option 1 — Opportunity framing (default):**
> "Good question — and honestly it's an advantage. Most of your competitors' sites are English-only, so a version in [language] reaches customers they're missing entirely. Yes, I can do [language]. Want me to show you what the bilingual version would look like?"

**Option 2 — Straight capability answer (if you can't write that language):**
> "Straight answer: I can build the site so it handles [language] properly — the structure, the buttons, the booking — but I'd want you or someone on your side to check the wording so it sounds like you, not like a translation. Fair?"

**Option 3 — Test the market first (practical):**
> "Let's check whether it's worth it before we build it: search '[service] in [language]' in your city. If the results are thin, that's your gap. Want me to run it and send you what comes up?"

**Branch tree**

- ⇐ **"My customers mostly speak [language]."** (≈40% [E])
  ⇒ "Then it should lead with [language], not be an afterthought. I'll build the main version in [language] and add the English version alongside. Want the mock?"
- ⇐ **"I only need English."** (≈30% [E])
  ⇒ "Then English only — simpler and cheaper. One thing worth knowing though: [X]% of your city speaks [language], and none of your competitors serve them. Want me to check how big that gap is before you decide?"
- ⇐ **"Can you write in [language]?"** (≈20% [E]) → answer honestly, per **Option 2**. Never fake fluency.
- ⇐ **"I'll just use Google Translate."** (≈10% [E])
  ⇒ "That's how you get a site that reads like a machine wrote it — which is exactly what makes customers distrust it. Better to do it properly or not at all. Want to see the difference?"

**Never say:** "Yes, I speak every language." · "Google Translate is fine." (it isn't, for business copy) · "Nobody cares about the language." (they do — that's why they asked)

**Exit ramp:** "If most of your customers speak [language], that's where the site should start."

---

### N15. "Do you know my trade? Have you done a [trade] site before?"

**Frequency & meaning:** a **credibility** objection, and the fastest way to lose it is to fake experience. Be honest about what you have, then **substitute proof with demonstration**: build a mock from their public photos. A specific mock of *their* business beats a generic portfolio every time — and it's something you can actually do.

**Option 1 — Honest + demonstrate (default):**
> "Straight answer: I've built [what you've actually built]. What I can do right now is show you rather than tell you — I'll mock up your homepage from your own photos and reviews, free, so you can judge the work instead of the CV. Want me to do that?"

**Option 2 — The relevance flip (story):**
> "Fair — but here's the thing: a [trade] owner doesn't care if I've built for other [trades]; they care whether the site brings *their* customers in. That's why I'd rather show you a version of *your* site than a gallery of someone else's. Want it?"

**Option 3 — Specificity proof (practical):**
> "Let's test it: I'll tell you the three things that decide whether a [trade] site brings calls — [e.g. reviews up front, one-tap call, service + area pages]. If those sound like the right three for your business, you know I understand it. If they don't, tell me what I'm missing."

**Branch tree**

- ⇐ **"I want to see a [trade] site you've built."** (≈40% [E])
  ⇒ if you have one, send it. If not: "I don't have one in [trade] I can show you honestly. What I'll do instead is build you a free mock — same effort, and it's about *your* business, not someone else's. Want me to start?"
  - ⇐ *"No, I want to see your work first."* → send whatever real work you have, labelled honestly. Never invent.
- ⇐ **"I've been burned by someone who didn't know my trade."** (≈25% [E]) → go to **U13** (structure) and **N5** (diagnose the failure).
- ⇐ **"So you're new at this?"** (≈20% [E])
  ⇒ "I'm new to *you* — here's what I've actually done: [honest list]. And you can test the work for free before you spend anything. That's a better test than a portfolio. Fair?"
- ⇐ **"Send me examples."** (≈15% [E]) → send 1–2 real examples, then one ask. Never pad with work you didn't do.

**Never say:** a portfolio you didn't build · "I've done hundreds" (if untrue — and it's checkable) · "Trade doesn't matter." (it does — that's the whole question)

**Exit ramp:** "Let me mock yours — that's the real test."

---

### N16. "I don't want another monthly bill."

**Frequency & meaning:** **subscription fatigue** — they're already paying for a phone, insurance, a van, a Facebook boost, and probably a tool they forgot about. The winning frame is **own vs. rent**: a one-time build plus a few dollars of hosting, versus a monthly fee forever. Make the distinction between **your fee (once)** and **hosting (small, paid to the host, not you)** crystal clear.

**Option 1 — One-time vs. monthly (default):**
> "You won't have one from me. It's $[X] once, then hosting which is a few dollars a month paid straight to the host — not to me. Compare that to $[X]/month forever on a platform. Which do you prefer?"

**Option 2 — Contrast with what they already pay (story):**
> "Fair — you've got enough bills. Think of it like the difference between buying a van and renting one every month: same van, but one of them is yours at the end. This is the buy version."

**Option 3 — Kill the recurring fear outright (practical):**
> "Let me be explicit: no retainer, no monthly fee to me, nothing auto-charged. One payment for the build, hosting you pay yourself, and updates only if you ask. Does that remove the worry?"

**Branch tree**

- ⇐ **"What's hosting, and why do I pay it?"** (≈35% [E])
  ⇒ "Hosting is just the rent for the space where the site lives — like electricity for a shop. It's a few dollars a month, you pay the host directly, and you keep the account. I don't take a cut."
- ⇐ **"I've been paying monthly for years on something I don't use."** (≈30% [E]) → go to **N5** (the dead-site diagnosis) — that's the real wound.
- ⇐ **"Can you just include everything in one price?"** (≈20% [E])
  ⇒ "I can build it so hosting is the only recurring cost, and it's tiny. I won't bundle a monthly fee into it, because then you're back to renting. Fair?"
- ⇐ **"What if I don't pay hosting?"** (≈15% [E])
  ⇒ "Then the site goes offline — but you still own it, and you can host it anywhere else. It's never lost. Want me to show you how to move it if you ever need to?"

**Never say:** "$X/month, all included." (that's the objection) · "There's a small management fee." (unexplained recurring = distrust) · "You won't even notice it." (patronising)

**Exit ramp:** "One payment, you own it, hosting is a few dollars to the host. That's it."

---

## Section 3 — Conversation maps, worked examples, and index

### 3.1 The master decision tree (use this when the objection is vague)

```
Owner raises something
        │
        ▼
Is it clear which bucket it is? ──── NO ──► Ask ONE open question
        │                                   ("What's driving that?")
        │                                              │
       YES ◄────────────────────────────────────────────┘
        │
        ├── PRICE ──────► Isolate: "if price weren't the issue, is this what you'd pick?"
        │                    ├─ yes ──► ROI reframe (U1) → phasing if needed
        │                    └─ hesitate ──► it was never price → go to NEED or TRUST
        │
        ├── AUTHORITY ──► Arm the champion (U3) / get the intro (U10)
        │                    └─ always date the next touch
        │
        ├── NEED ───────► Diagnose the status quo (W1/W6/N1/N2/N5)
        │                    └─ show THEIR specific gap (screenshot > argument)
        │
        └── TIMING ─────► "What changes between now and then?"
                             └─ shrink the ask + date it (U7/N8)

After ANY branch: one ask, one question, or a dated next step. Never two.
If the same objection returns twice → it's real → stop, pivot, exit warmly.
```

**Lane check before you reply** (gruv.ai): **Educate** (missing context) · **Re-scope** (wants it, wrong size) · **Hold firm** (terms would break) · **Walk away** (no workable budget/authority/timeline). Knowing the lane stops you improvising.

### 3.2 Three worked transcripts (the branches in action)

**Transcript A — with-website, price → cheaper competitor → phased close.**
*(turns: 6 · branches taken: U1 → U11 → U1-Option 2)*

> **Owner:** "Honestly, that's a lot of money for a website. I've had a quote for half that."
> **You (U11, inspect first):** "That's a real difference — so let's look at it honestly. Is their quote the same scope: the mobile work, the booking setup, and support after launch?"
> **Owner:** "I don't know, they just said $750 for a site."
> **You (comparison collapsed):** "Then I'd want to see what's inside it before you decide. Forward me their quote and I'll show you exactly where the gap is — if theirs genuinely covers the same thing, take theirs and I'll tell you so."
> **Owner:** "…Alright. But I still don't want to spend $1,500."
> **You (U1-Option 2, phase it):** "Then don't — start with the $500 audit and the priority fixes, and you decide on the rebuild later once you've seen it. Two separate decisions. Want the audit scope?"

**Why it works:** you never defended the price. You made *them* inspect the comparison, then handed them a smaller door. If they'd said "they're cheaper, same scope, I'm going with them" — you'd have said "then take it, genuinely" and walked (§0.2 lane 4).

---

**Transcript B — the partner scenario, with the double pushback.**
*(turns: 7 · branches taken: U2 → U3 → U3 pushback → date)*

> **Owner:** "I like it, but I need to think about it."
> **You (U2-Option 1):** "Totally understand — can I ask what specifically you'd need to think through? Sometimes I can answer it right now and save you the time."
> **Owner:** "I'd have to talk to my business partner."
> **You (U3-Option 1):** "Of course — that's smart. What would help you explain it to them? I can send a five-line summary and one screenshot so you don't have to pitch it yourself. What would *they* care about most — the cost, or the new clients?"
> **Owner:** "Look, I never make any financial decisions without consulting them first. That's just how we work."
> **You (U3 pushback branch — agree, don't fight):** "Respect that — most owners I work with are the same, and honestly it's why they're still in business. So let me do the work for you: I'll send the summary addressed to both of you. You look at it together, no commitment, no payment link. Fair?"
> **Owner:** "…Fine, send it."
> **You (date it immediately — never leave an undated stall):** "Will do — and so I'm not a nag, will you two have had a chance to look by Thursday? If it's a no, I'll close the file and you won't hear from me again."

**Why it works:** the second pushback isn't resistance, it's a boundary. You agreed with it, then removed their effort. The dated follow-up is what stops this becoming one of the **85%** of deals that die without a scheduled next step [S: Prospeo].

---

**Transcript C — no-website, word of mouth → "show me proof" → fully booked.**
*(turns: 6 · branches taken: N1 → N1 proof → N10 → N8)*

> **Owner:** "I don't need a website — all my work comes from word of mouth."
> **You (N1-Option 3, extend don't contradict):** "That's brilliant — and a website wouldn't replace that at all. It just means when a referral Googles you before calling to check you out, they actually find you instead of nothing. Do you know what comes up when someone searches your business name right now?"
> **Owner:** "Probably just the Google listing. But show me proof websites bring clients in my trade."
> **You (N1 proof branch):** "Fair — let's use your street instead of theory. 81% of consumers research a business online before deciding [Google Consumer Research 2025], and 91% read reviews before visiting [marketingltb 2026]. I'll send you a screenshot of your listing next to the [trade] who has a site — you tell me which one you'd call."
> **Owner:** "…OK, but honestly I'm fully booked. I don't need more work."
> **You (N10 — switch from volume to position):** "Then this isn't about more customers — it's about *better* ones. A site with your prices and services up front filters out the tyre-kickers and lets you charge more for the jobs you actually want. Want to see what that looks like?"
> **Owner:** "Maybe after the season."
> **You (N8 — date it):** "Perfect — when does it calm down? I'll message you in [month] with the mock ready, and I won't chase you in between."

**Why it works:** three different objections, three different buckets (Need → Need → Timing), and the whole thing ends in a **dated maybe** — which is a win. Note there's no phone call anywhere: it's all DM/email, per §3B.3.

### 3.3 Quick index — owner phrase → where to answer

| Owner says | Go to |
|---|---|
| "Too expensive" / "no budget" | **U1** (+W5 rebuild math / +N3 starter slice) |
| "I need to think about it" | **U2** |
| "I need to talk to my partner / wife" | **U3** |
| "Who are you?" / "is this a scam?" / "how'd you get my info?" | **U4** |
| "Just send me the info" / "tell me what's wrong for free" | **U5** |
| "Not interested" | **U6** |
| "No time" / "next quarter" / "after the season" | **U7** (+N8) |
| "Can you guarantee more clients / #1 on Google?" | **U8** |
| "Why should I choose you?" | **U9** |
| "I'm not the one who decides" | **U10** |
| "Someone quoted me less" / "cheaper elsewhere" | **U11** |
| "I'll do it myself" / "AI can build it free" / "my nephew" | **U12** (+W2) |
| "I got burned before" / "I don't trust web people" | **U13** (+W14) |
| "Send me a proposal / contract first" | **U14** |
| "Can I pay at the end / per result?" | **U15** |
| "Where are you based?" / "do you work here?" | **U16** |
| They went silent after showing interest | **U17** (+§0.6) |
| "I have no photos / content / time for this" | **U18** (+N13) |
| "We already have a site, we're happy" | **W1** |
| "My nephew built it" | **W2** (+U12) |
| "We just redid it" | **W3** |
| "We're locked into a contract" | **W4** |
| "Why rebuild? Just patch it" | **W5** |
| "Referrals are enough" (has a site) | **W6** |
| "It's on Wix, I can't move it" | **W7** |
| "We like our design / our brand" | **W8** |
| "We don't want to lose our Google ranking" | **W9** |
| "We already rank page one" | **W10** |
| "Our customers are old / our industry is different" | **W11** |
| "The site is just informational" | **W12** |
| "Our marketing person handles it" | **W13** |
| "We tried a redesign, it got worse" | **W14** |
| "How do I know you won't break it?" | **W15** |
| "Word of mouth is enough" (no site) | **N1** |
| "Facebook / Instagram / Maps is enough" | **N2** |
| "A website is too expensive" (never had one) | **N3** (+U1) |
| "I'm not technical / it'll get hacked" | **N4** |
| "I tried a site before, it failed" | **N5** |
| "Won't work in my trade / town" | **N6** |
| "I'm too small / retiring" | **N7** |
| "Later / next year" (no site) | **N8** |
| "I only need ads / TikTok" | **N9** |
| "I'm fully booked / don't want tyre-kickers" | **N10** |
| "I don't use email — call me" | **N11** |
| "Who owns it? What if I stop paying?" | **N12** |
| "What do you need from me? How long?" | **N13** |
| "Will it be in my language?" | **N14** |
| "Do you know my trade?" | **N15** |
| "I don't want another monthly bill" | **N16** |

### 3.4 Mode cheat sheet — what changes between the two modes

| | `with_website` | `no_website` |
|---|---|---|
| **Core pain** | decay — the site is outdated/broken and leaking | absence — they're invisible where customers look |
| **Primary pitch** | audit ($500) → **redesign ($1500)** (§12.4R) | **build ($1200)**, one offer (§12B.4) |
| **Proof that lands** | a defect on **their own site** (screenshot) + the AI transcript | their **Maps/social facts** (rating, review count, empty website field) |
| **Best first wedge** | "I checked your site on my phone…" | "You have [N] reviews and no website — where do ready-to-buy customers go?" |
| **The killer reframe** | patch vs. rebuild economics (W5) | the invisible referral leak (N1) + AI can't recommend you (N2) |
| **Objections that don't apply** | "I don't have a site" ones | audit/redesign/patch ones (nothing to audit) |
| **Channel** | email (DM optional) | email or FB/IG/X/Reddit DM |
| **Phones** | avoid by default (cross-border calls read as scam) | **absolutely banned** — no calls, SMS, WhatsApp (§3B.3) |
| **Word limits** | outreach ≤150 words; replies 2–4 sentences | outreach email ≤150 / **DM ≤80**; replies ≤40 |

### 3.5 Sources (Golden Rule — everything above was researched, not assumed)

**Fetched and read in full for this version:**
1. **Prospeo — "Objection Handling Framework: 7 Proven Methods (2026)"** (prospeo.io/s/objection-handling-framework) → the 7 frameworks (ARC, LAARC, LAIR, LACE, FFF, SOLVE, ARR), Validate-Isolate-Reframe, "at least four attempts", the 60%/48%/80% follow-up figures, "compared to what?", the "never ask why" rule.
2. **Prospeo — "I Need to Think About It: 7 Sales Responses That Work (2026)"** (prospeo.io/s/i-need-to-think-about-it) → the four hidden meanings, "what specifically?" (~60%), Gong's 54.3%-vs-31% question stat, deals without a next step die 85%, the 10-day/70% rule, 75% spouse stat, 50% non-decision-maker stat, the Day 0/2/5/10 cadence.
3. **Gangly — "Sales Objection Statistics" (Apr 2026)** (getgangly.com/blog/sales-objection-statistics) → the frequency table (price 35%, timing 22%, already-have 18%, authority 14%, urgency 11%, feature 9%, trust 6%), win rates by type, 2.4 objections/call, 64% with 2+, the 4.1× early/late multiplier, 42%-vs-19% reframe/discount, +38% for proof within 30s, top-vs-bottom quartile 2.4×.
4. **HubSpot — "44 common sales objections & how to respond" (Aug 2026)** (blog.hubspot.com/sales/handling-common-sales-objections) → the 5-step framework (LAER + Anticipate), the 44-objection catalogue, "if they raise it twice, it's real", never disparage competitors, the champion-arming scripts.
5. **GetMapLeads — "Cold Calling Script for Web Design Agencies" (Apr 2026)** (getmapleads.io/blog/cold-calling-script-web-design-agencies) → the eight no-website objections with their "why they say it" analysis, the 60%/40% split on "just send me an email", callback discipline, the "is now a bad time?" technique, 90-day/6-month callback windows. *Adapted here from phone to email/DM, since §3B.3 bans calls.*
6. **LeadsAgent — "27% of Small Businesses Have No Website in 2026" (Mar 2026)** (leadsagent.io/blog/businesses-without-website-statistics) → 27% no-website figure, 81% research-before-buying, 94% first-impression stat, 88% mobile-abandonment, trade-level no-website percentages, the 50/50 referral-leak rule, the four reasons owners say no, 1–2 contacts / 3–10 day cycle, the "been meaning to" buying signal.
7. **Objeq — "I Can Get It Cheaper Elsewhere" (Sep 2026)** (objeq.io/blog/handle-can-get-it-cheaper-elsewhere) → inspect-the-comparison, concede structure not price, "what does the cheaper option cost if it doesn't work", know your walk-away.
8. **SendEmAll — "Cold Email Follow-Up Sequence" (Aug 2026)** (sendemall.com/blog/cold-email-follow-up-sequence) → the 5-touch Day 0/3/7/12/21 sequence with per-touch reply rates, "change the angle not the message", why the breakup email works, multi-channel +15–25%, the stop rules.
9. **gruv.ai — "How to Handle Sales Objections as a Freelancer" (Aug 2026)** (gruv.ai/blog/how-to-handle-sales-objections-as-a-freelancer) → objections as risk signals, the four lanes (Educate / Re-scope / Hold firm / Walk away), payment-trigger discipline, naming the four boundaries in writing.
10. **Cognism — "Objection Handling for 2026" (Sep 2025)** (cognism.com/blog/objection-handling) → the 5-step process (Listen → ask open questions → Solve → Confirm → Move on), the 70/30 rule, "never badmouth your competitors" + the 1–10 rating technique, "never go back to an objection once addressed".
11. **marketingltb — "Local Marketing Statistics 2026"** (marketingltb.com/blog/statistics/local-marketing-statistics/) → 91% read reviews before visiting a local business; 73% trust businesses with 4+ stars.
12. **Pitchbase — "Objection Handling: 5 Frameworks + 10 Scripts" (Apr 2026)** (pitchbase.app/en/blog/objection-handling-complete-guide) → LAER/CRAC/Feel-Felt-Found/Boomerang reference set; cap at 2–3 objections per conversation.

**Cited secondarily (via the sources above — not independently re-verified this session):** Gong's call dataset, Salesforce State of Sales 2025, Chorus.ai, Outreach's Sales Performance Report, Sandler's "permission to say no", SalesGravy's three-category force, Squarespace-forum / InsideTheSquare evidence on AI-builder drafts needing human polish. Treat their numbers as indicative until re-verified.

**Constraint source:** `AUDIT_EXECUTION_DIRECTIVE.md` §0 (controls and prices), §3B.3 (phone ban), §12 / §12B (outreach protocol, word limits, banned vocabulary, single-offer rule), §12.4R (audit → redesign sequence), §12.6 (left-on-table estimate must be researched, never invented), §12.7 (truthfulness).

### 3.6 Maintenance

- **Prices change →** update the three anchors at the top and search the file for `$500`, `$1500`, `$1200`.
- **A new objection keeps appearing →** add it to the right section, give it three options and a two-level tree, and add it to the §3.3 index. If it's shared by both audiences, it belongs in Section 0 and gets referenced, not duplicated.
- **An option stops working →** replace the *option*, don't delete the entry — the branch tree below it is usually still valid.
- **Probability labels are priors, not facts.** `[S]` means sourced; `[E]` means my estimate. When real reply data accumulates from your own sends, replace the `[E]` figures with your own numbers — that's the only way this file gets sharper than the research it came from.


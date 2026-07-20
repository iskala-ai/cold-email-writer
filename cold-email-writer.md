---
name: cold-email-writer
description: Writes, rewrites, validates, and improves B2B cold emails — a distinct email per buying-committee role, built from a verifiable personalization line, a problem the recipient recognizes, a claim sized to the evidence behind it, and a CTA calibrated to their authority, then checked for deliverability, spam triggers, and compliance. Use this skill whenever the user asks to write a cold email, first-touch email, outbound email, intro email, or breakup email; asks for subject lines, preview text, or a CTA; pastes an email and asks to improve, shorten, or rewrite it; asks why an email isn't getting replies; or needs role variants for multi-threading one account. Also invoke when converting research, a signal, or a personalization angle into sendable copy. Do NOT use for building the full multi-step sequence, designing the ICP or persona, generating personalization angles from raw research, or auditing domain and inbox deliverability infrastructure — those are separate workflows.
---

# Cold Email Writer

## Goal

Produce **sendable cold emails that earn a reply** — each under 100 words, built on a verifiable observation, naming a problem the recipient recognizes as theirs, making a claim no larger than the evidence supports, and ending in a single question calibrated to what that person can actually decide.

The output must be immediately usable, without translation, by **Sales, SDRs, BDRs, Marketing, Customer Success, RevOps, and Founders**.

## Overview

A cold email is an interruption. It earns continued attention sentence by sentence, and it loses that attention permanently at the first line that reads as automated, inaccurate, or self-interested.

Every email produced here has four load-bearing parts:

| Part | Job | Fails when |
|---|---|---|
| **Opening** | Prove this was written for them | Generic, flattering, or provably wrong |
| **Problem** | Name something they'd agree is true | Vendor language they don't use about themselves |
| **Claim** | Give a reason to believe change is possible | Larger than the evidence behind it |
| **CTA** | Make replying easier than ignoring | Asks for more than the recipient can grant |

The most common failure is not bad writing. It is an email that is well-written *about the sender*. Every sentence should be answerable with "so what does that mean for me?" — and if a sentence can't survive that question, it comes out.

The workflow moves in a fixed order:

1. **Identify the recipient's role** — different roles get different emails, not the same email with a swapped title.
2. **Build the substance** — the metric, the problem, the observable specific.
3. **Size the claim to the evidence** — then construct the CTA to match their authority.
4. **Write** — primary plus variants, subject lines, preview text.
5. **QA** — deliverability, compliance, accuracy, and the "so what" pass.
6. **Set up the test** — because no email is validated until it has been sent.

The output serves seven functions:

| Function | Uses primarily |
|---|---|
| Sales / AE | Role variants, multi-thread set, CTA options |
| SDR / BDR | Drafts, subject lines, personalization variables, fallbacks |
| Marketing | Messaging consistency, claim substantiation, test design |
| Customer Success | Re-engagement and expansion variants |
| RevOps | Variable fields to enrich, deliverability constraints, test structure |
| Founders | The core email, what's claimed, and what evidence is missing |

## When this skill should be invoked

Invoke when the user:

- Asks to write a cold email, first touch, outbound email, or intro email
- Asks for subject lines, preview text, or a call to action
- Pastes an email and asks to improve, shorten, tighten, or rewrite it
- Asks why their emails aren't getting replies
- Needs different versions of an email for different roles at one account
- Wants to turn research, a buying signal, or a personalization angle into copy
- Needs a breakup, bump, or re-engagement email
- Asks how long an email should be, or what CTA to use
- Asks whether an email will land in spam

Do **not** invoke for building the complete multi-step sequence, ICP or persona work, generating angles from raw research, or auditing sending infrastructure. Note the handoff instead of absorbing the work.

## Success criteria

The email set is complete only when all of the following hold:

- [ ] **Each email is under 100 words** in the body, and reads in under 15 seconds. Longer versions exist only if the user explicitly asked.
- [ ] **The opening line is verifiable** — traceable to a named source with a date, and true enough that the recipient would agree.
- [ ] **One idea per email.** A second idea becomes a different email, not another paragraph.
- [ ] **The problem is stated in the recipient's language**, not in product or category language.
- [ ] **Every claim maps to evidence**, with thin evidence downgraded to what it actually supports.
- [ ] **The CTA is a single question**, answerable in one sentence, calibrated to the recipient's authority.
- [ ] **A distinct email exists per relevant committee role**, with multi-thread variation so colleagues don't receive near-identical copy.
- [ ] **Three to five subject lines** are provided, each under about 45 characters, plus preview text.
- [ ] **Personalization variables are named**, each with a fallback for when the field is empty.
- [ ] **No spam triggers**: no links in first touch unless justified, no images, no attachments, no all-caps, no excessive punctuation, plain-text formatting.
- [ ] **Compliance is addressed** — sender identity, opt-out mechanism, and the legal basis appropriate to the recipient's jurisdiction.
- [ ] **A "so what" pass has been run** — every sentence justified from the reader's perspective, with unjustifiable ones removed.
- [ ] **At least one variant** tests a materially different angle, not just different wording.
- [ ] Every inference in the copy is phrased as a question, never as an assertion.
- [ ] A test design is specified, with sample size and the decision threshold.

## Constraints

Cold email is where a small inaccuracy costs the whole account, and where a compliance mistake costs the domain.

- **Never invent facts about the recipient.** No fabricated posts, hires, funding, launches, tools, headcounts, or news. If the user supplied no research, the email is written without a personalization line, and the gap is named.
- **Never invent proof.** No fabricated case studies, customer names, percentages, testimonials, or benchmark statistics. Where the user has no results data, the email makes a mechanism claim rather than an outcome claim.
- **Downgrade thin evidence.** One customer's result is written as one customer's result — never "clients typically see". A claim that prompts "prove it" and cannot be proven is worse than a smaller claim that can.
- **Never reference behavioural tracking.** No page visits, opens, profile views, or intent data in copy, regardless of legality.
- **Phrase inferences as questions.** "Is that to add capacity or replace someone?" is safe whichever way the guess falls. A wrong assertion is unrecoverable.
- **Never fabricate familiarity.** No invented mutual connections, no "following up on our conversation" where none occurred, no "as promised" where nothing was promised, no fake re-send of an earlier email.
- **No deceptive subject lines.** No fake "Re:" or "Fwd:", no false urgency, no misleading meeting references. These are both a compliance risk and a trust loss.
- **Compliance is not optional.** Include a real sender identity and a working opt-out. For recipients in the EU and UK, note that consent or legitimate-interest requirements apply and flag where the user should confirm their basis. State plainly that jurisdiction rules vary and that this is guidance, not legal advice.
- **No personal or sensitive material.** Professional, published information only.
- **Do not claim outcomes you don't control.** If the offer produces meetings and the customer's close rate produces revenue, claim meetings and name the dependency.
- **No manipulative pressure.** No manufactured scarcity, no guilt framing, no implied prior agreement.
- **Stay in scope.** Full sequences, ICP and persona work, angle generation from raw research, and infrastructure auditing belong to other workflows.

## Clarifying questions

Ask before starting whenever the answer is not already available. Ask in **one batch**, prioritized, and never re-ask what has been supplied.

**Always required (block if unknown):**

1. **Who is the recipient** — role, seniority, and company or segment?
2. **What is the offer**, and what problem does it solve for that role specifically?
3. **What research or evidence exists** — anything about this account or contact, and any customer results usable publicly?

**Strongly needed (ask, but can proceed without):**

4. **What is the CTA meant to achieve** — a meeting, a reply, permission to send something, or a referral to the right person?
5. **Sender identity** — who it comes from and their title, since seniority changes what the email can credibly say.
6. **Scale** — one email, or a template for a list? Templates need variables and fallbacks.
7. **Prior contact** — first touch, follow-up, or re-engagement? These are structurally different emails.
8. **What has already been tried** — copy that got no replies narrows the search fast.
9. **Recipient jurisdiction** — EU/UK recipients change the compliance footing.

**Useful if available:**

10. Reply data or examples of emails that have worked.
11. Brand voice constraints or forbidden phrasing.
12. Sending tool and whether variables, spintax, or conditional blocks are supported.

If only items 1–3 are answered, state which parts will carry assumptions and proceed. If item 3 is "no research at all", say so plainly: a template can still be written, but the opening line will be category-level rather than personal, and reply rates should be expected to reflect that.

## Step-by-step workflow

### Phase 1 — Write a different email per committee role (steps 1–9)

**Step 1 — Identify who is being emailed.** Establish the roles in play. Sending one email to every title with only the name changed is the most common structural error in outbound, because each role's question is different.

**Step 2 — Decision-maker email.** Shortest of the set. Outcome and risk, three sentences maximum, one question. This reader scans on a phone between meetings; anything requiring a second read is deleted.

**Step 3 — Economic-buyer email.** Frame around money — the cost of the current approach against the alternative they are actually weighing, usually a hire rather than a competitor. The claim must be defensible because this reader will test it.

**Step 4 — Champion email.** The most detailed of the set, because this reader may forward it. Write it so it survives being pasted into an internal message without you present to explain it: the problem, the mechanism, and one piece of proof, all standing alone.

**Step 5 — End-user email.** Frame around the daily task that stops being manual. Most credible of the set, because it describes something the reader actually does. Lowest authority, so the CTA asks for a conversation, not a decision.

**Step 6 — Technical-evaluator email.** Frame around risk, integration, and constraint. Precise, unembellished, and free of marketing language. This reader verifies claims, so every specific must be accurate.

**Step 7 — Influencer email.** Shortened decision-maker framing with more peer proof. Used sparingly, and only where the influence path is genuinely identifiable.

**Step 8 — Gatekeeper email.** Two sentences whose only job is to be forwarded: what this concerns, and why the person behind them would care. Not a pitch, and never an attempt to bypass.

**Step 9 — Multi-thread variation.** Where several people at one account are contacted, vary angle, subject, and structure deliberately. Colleagues compare messages; near-identical copy exposes automation and burns every thread at once. Note also the sequencing — who is contacted first, and whether later emails should reference the earlier outreach honestly.

### Phase 2 — Build the substance (steps 10–17)

**Step 10 — Anchor to what they own.** The email should implicate something the reader is personally responsible for. Company-level facts are safe and weak; role-level facts create obligation to respond.

**Step 11 — Identify the metric.** Name the number this reader is measured on, and connect the email to it. Where the magnitude of improvement is unknown, describe the mechanism instead and leave the number out rather than inventing one.

**Step 12 — Frame the personal outcome.** What the reader gains — a quieter week, a problem off their desk, a visible win. Usually implied rather than stated, since stating it directly can read as presumptuous.

**Step 13 — Attach to the business objective.** The company-level initiative the purchase would serve. Most useful in champion and economic-buyer emails, where an internal case must be made.

**Step 14 — Write the problem line.** The single most important sentence in the email. It must describe a situation the reader would recognize as theirs, in words they would use. Test it by asking whether a competitor's customer would also nod — if the line is true of everyone, it is specific to no one.

**Step 15 — Add one credibility detail.** A small, accurate specific that proves the message wasn't mass-produced. Used as texture inside the problem line rather than as its own sentence.

**Step 16 — Reference the observable workflow.** Where public evidence reveals how they operate today — a job description naming a process, a site structure, a published policy — referencing it makes the problem line concrete rather than assumed.

**Step 17 — Handle the existing stack.** Where a tool is detectably in use, decide whether to reference it. Referencing an incumbent can prove relevance or can read as intrusive; the safe form is a question about their experience with the current approach rather than an assertion about its shortcomings.

### Phase 3 — Size the claim and the ask (steps 18–24)

**Step 18 — Establish the reason for reaching out now.** A trigger, if one exists, answers the reader's unspoken "why me, why today". Where no trigger exists, do not manufacture one — the email simply carries more weight on the problem line instead.

**Step 19 — Choose the motivational frame.** Gain, risk, relief, status, or mandate. The same problem opens differently for a founder chasing growth and an operations lead avoiding failure. Pick one; mixing frames dilutes both.

**Step 20 — Pre-empt or avoid objections.** Some copy creates objections rather than answering them. Implying the reader is doing something badly triggers defensiveness; overclaiming triggers scepticism. Test the draft for the reaction it provokes, and where a major objection is predictable, defuse it in a clause rather than a paragraph.

**Step 21 — Decide what to prove and what to leave out.** First touch cannot carry a full case. Choose the single most load-bearing proof point and omit the rest; the remainder belongs in the reply, not the email.

**Step 22 — Size the ask to the budget reality.** An email implying a significant commitment to someone with no budget creates friction. Where the reader can't spend, the CTA should seek a conversation or a referral, not an evaluation.

**Step 23 — Calibrate the CTA to authority.** Decision makers can grant a meeting; end users usually cannot. Ask for what this reader can actually give. A CTA the recipient is not empowered to fulfil produces silence, not a redirect.

**Step 24 — Adjust for awareness stage.** A problem-unaware reader needs the problem named before any solution language appears. A solution-aware reader needs differentiation. An actively-evaluating reader needs a reason to include you. Sending solution-aware copy to a problem-unaware reader is a frequent and invisible cause of low reply rates.

### Phase 4 — Write, QA, and test (steps 25–32)

**Step 25 — Apply email-channel constraints.** Plain text, no images, no attachments, minimal or no links in first touch. Write for a mobile preview: the first line must work as preview text, and the whole email must be readable without scrolling. Keep paragraphs to one or two lines.

**Step 26 — Decide on assets.** If an asset genuinely strengthens the email, offer it rather than attaching or linking it — offering it also creates a low-friction CTA. Name any asset that would help but doesn't exist yet.

**Step 27 — Build the personalization layer.** Write the opening line, then define every variable it depends on, with a fallback for each. A variable with no fallback produces a broken email the moment a field is empty, which is worse than no personalization.

**Step 28 — Write the drafts.** Produce the primary email plus at least two variants testing materially different angles — not synonym swaps. Then subject lines: short, lowercase, specific, curiosity without clickbait, and never deceptive.

**Step 29 — Write the CTA as a question.** The best CTA is a question that is genuinely easier to answer than to ignore, and whose answer is informative whether it is yes or no. Interest-based questions outperform calendar demands at first touch because they ask for a judgement rather than a commitment.

**Step 30 — Check that the email qualifies.** A well-built cold email attracts fit prospects and repels poor ones. If the copy is broad enough that anyone might reply, it will generate replies that waste time. Specificity is a qualification mechanism, not just a craft preference.

**Step 31 — Run the red-flag QA pass.** Check deliverability (spam trigger words, link count, formatting, sender reputation risk), accuracy (would they agree every statement is true?), compliance (identity, opt-out, jurisdiction), claims (each mapped to evidence), tone (no condescension, no manufactured urgency, no false familiarity), and the "so what" test on every sentence. Cut anything that fails.

**Step 32 — Specify AI use and the test plan.** State what can be automated — variable population, channel compression, first-draft generation, variant creation — and what must stay human: verifying facts are true, judging whether an inference is fair, and the final accuracy read. Then define the test: sample size per variant, what counts as a result, how long to run, and the threshold at which a variant wins. No email is validated until it has been sent to a meaningful sample.

## Output template

Always produce this exact structure. Tag inferences `[assumption]`; every claim maps to evidence.

```
# Cold Email — [Role] @ [Segment]

_Purpose: [first touch / follow-up / re-engagement / breakup] · Channel: email_
_Sender: [name, title] · Scale: [1 account / template for N] · Written: [date]_

---

## 1. Executive summary
Four sentences or fewer: who it's to, the angle, the claim being made, the CTA,
and the confidence in the evidence behind it.

## 2. Email snapshot
| Field | Detail |
|---|---|
| Word count | |
| Reading time | |
| Angle | |
| Claim strength | evidenced / single case / mechanism only |
| CTA type | |
| Links / attachments | |

## 3. Audience & context
Role, seniority, awareness stage, what they're measured on, and what the email
must accomplish.

## 4. Emails by committee role
| Role | Angle | Claim | CTA | Length |
|---|---|---|---|---|

**Multi-thread variation & sequencing:** ...

## 5. What they own
The responsibility this email implicates, and why that creates a reason to reply.

## 6. Metric & claim
| Metric implicated | Claim made | Evidence | Status |
|---|---|---|---|

## 7. Outcome framing
**Personal (implied):** ...
**Business (for forwarding):** ...

## 8. Problem line
**Draft:** "..."
**Would a non-prospect also nod?** [if yes, rewrite]

## 9. Relevance & stack framing
Observable workflow or tooling referenced, and how it's handled.

## 10. Reason for reaching out now
| Trigger | Source | Date | How it's used |
|---|---|---|---|

## 11. Email by awareness stage
| Stage | Adjustment | Version |
|---|---|---|
| Problem-unaware | | |
| Problem-aware | | |
| Solution-aware | | |
| Evaluating | | |

## 12. Differentiation line
What separates this from the alternatives — in one clause, not a paragraph.

## 13. Objection pre-empt
| Likely objection | Handled in copy? | How |
|---|---|---|

## 14. Drafts
**Primary**
Subject: ...
Body:
...

**Variant A — [different angle]**
...

**Variant B — [different angle]**
...

## 15. Subject lines & preview text
| # | Subject | Chars | Preview text | Rationale |
|---|---|---|---|---|

## 16. Personalization variables
| Variable | Source field | Example | Fallback if empty |
|---|---|---|---|

## 17. CTA options
| CTA | Ask size | Best for | Expected response |
|---|---|---|---|

**Discovery question this sets up:** ...

## 18. Deliverability, compliance & red flags
**Deliverability**
| Check | Status | Note |
|---|---|---|

**Compliance**
| Requirement | Handled | Note |
|---|---|---|

**Rejected lines**
| Line | Rejected because |
|---|---|

## 19. Test plan & recommended actions
**Test design:** [variants, sample size, metric, duration, decision threshold]

| Action | Function | Priority | Why |
|---|---|---|---|

**Assumptions to validate**
| Assumption | How to validate | By when |
|---|---|---|

**Evidence gaps:** [proof that would strengthen the claim if obtained]
```

## Best practices

**Under 100 words, one idea.** Every additional idea reduces the chance of any of them landing. If two ideas both matter, that's two emails.

**Write the problem line first.** The email is built around it. If the problem line is weak, no subject line or CTA rescues it.

**Make every sentence pass "so what?"** Read each line as the recipient and ask what it means for them. Sentences about your company, your funding, or your feature set almost never survive this pass.

**Ask, don't assert.** Questions invite correction and cost nothing when the guess is wrong. Assertions about someone's internal situation are wrong often enough to be dangerous.

**Size the claim to the evidence, then shrink it further.** A modest claim that survives scrutiny outperforms an ambitious one that invites it. When in doubt, claim the mechanism rather than the outcome.

**The CTA should be easier to answer than to ignore.** "Worth a conversation?" gets a yes or no. "Are you free Tuesday at 3pm or Thursday at 11am?" asks for a decision the reader hasn't agreed to make yet.

**Subject lines should look internal, not marketed.** Short, lowercase, specific, no emoji, no brackets, no urgency theatre. If it looks like a newsletter, it's read like one.

**Write for a phone.** Most first touches are read in a preview pane. If the value isn't visible in the first two lines, the rest doesn't exist.

**Adapt to regional norms.** For MENA B2B, a slightly warmer opening and a clear sender identity carry more weight than the terse US-style pattern. Arabic and English mix naturally in business communication, and mirroring the recipient's own register — including their LinkedIn language choice — outperforms formal translation. WhatsApp is a legitimate follow-up channel once contact is warm, though not usually as a first touch.

**Nothing is validated until it's sent.** Internal preference is not evidence. Define the test, run it on a meaningful sample, and let reply data decide.

## Common mistakes

| Mistake | Why it fails | Do instead |
|---|---|---|
| Over 150 words | Deleted before the value is reached | Under 100, one idea |
| Opening about yourself | Reader has no reason to continue | Open about them, verifiably |
| Generic first line | Reads as mass-mailed, because it is | Specific, sourced, and dated |
| Asserting an inference | Wrong often, unrecoverable when wrong | Phrase as a question |
| Unsubstantiated stats | Collapses on "where's that from?" | Claim only what evidence supports |
| Feature list | Reader must translate; they won't | State the problem and the change |
| Multiple CTAs | Choice paralysis produces no action | One question, one ask |
| Calendar link in first touch | Asks for commitment before interest | Ask for interest first |
| Links or attachments in first touch | Deliverability risk, low trust | Offer, don't attach |
| Fake "Re:" or false familiarity | Compliance and trust failure | Honest subject and framing |
| Same email to every role | Each role's question is different | A distinct email per role |
| Variable with no fallback | Broken email when the field is empty | Fallback for every variable |
| Solution-aware copy to unaware readers | Invisible mismatch, silent failure | Match copy to awareness stage |
| Skipping compliance | Domain and legal exposure | Identity plus opt-out, always |

## Validation checklist

Run before delivering. Every box checked, or explicitly flagged as an open gap.

**Craft**
- [ ] Under 100 words; readable in under 15 seconds
- [ ] One idea only
- [ ] Problem line would make a fit prospect nod, and a non-prospect not
- [ ] Every sentence passes "so what?"
- [ ] One CTA, phrased as a question, answerable in a sentence
- [ ] 3–5 subject lines under ~45 characters, plus preview text
- [ ] ≥2 variants testing materially different angles

**Integrity**
- [ ] No invented facts about the recipient
- [ ] No invented proof, case studies, customers, or statistics
- [ ] Every claim mapped to evidence; thin evidence downgraded
- [ ] Inferences phrased as questions
- [ ] No behavioural-tracking references
- [ ] No fabricated familiarity, mutual connections, or prior contact
- [ ] Outcomes outside the sender's control named with their dependency

**Deliverability**
- [ ] Plain text; no images or attachments
- [ ] Links minimal or absent in first touch
- [ ] No spam-trigger phrasing, all-caps, or excessive punctuation
- [ ] Formatting survives a mobile preview pane

**Compliance**
- [ ] Real sender identity present
- [ ] Working opt-out mechanism
- [ ] Jurisdiction noted where EU/UK recipients are involved
- [ ] No deceptive subject line or false urgency
- [ ] Stated as guidance, not legal advice

**Operational**
- [ ] Distinct email per relevant committee role
- [ ] Multi-thread variation prevents near-identical copy
- [ ] Every variable has a fallback
- [ ] Awareness-stage version specified
- [ ] Test design with sample size and decision threshold
- [ ] Evidence gaps listed

## Examples

### Example 1 — First touch from research

**Input**

> "Write a cold email to the Head of Sales at a 60-person B2B SaaS in Riyadh. They've had an SDR role open six weeks. I sell outbound-as-a-service, ~$4k/month. Best proof: one client went from 2 to 11 meetings a month in 90 days."

**Clarifying questions asked first**

> Two: (1) Can that 2→11 result be used with the client named, or anonymized? Named proof is worth several times anonymous. (2) Who's it coming from — you as founder, or an SDR? Seniority changes what the email can credibly claim.

**Output — decisions shown**

```
## 2. Email snapshot
Word count: 74 · Angle: unfilled SDR role · Claim strength: single case
(downgraded from "clients see 5x") · CTA: interest question · Links: none

## 8. Problem line
Draft: "Six weeks open usually means the problem isn't finding someone — it's
that the role needs a system to walk into."
Would a non-prospect nod? No — companies without an open role wouldn't.
Passes.

## 14. Primary draft
Subject: sdr role still open?

Hi [First name],

Noticed the SDR role's been open about six weeks. Usually that's less about
candidates and more about what they'd actually run on day one.

We build and run that part — email and LinkedIn — so the pipeline starts before
the hire does. One client went from 2 to 11 meetings a month in 90 days.

Worth a look at how that'd apply here?

[Sender name, title]
[Company, address, unsubscribe]

## Why it's built this way
- Opens on something he owns, verifiably, with a date behind it
- The inference ("the problem isn't candidates") is softened by "usually" —
  it's a hypothesis, not a claim about his hiring
- Claim is written as ONE client's result, not as a typical outcome. With one
  measured case, "clients typically see 5x" would be fabrication
- CTA asks for a judgement, not a calendar slot
- No link, no attachment, plain text

## 14. Variant A — cost-of-waiting angle
Different angle, not different words: frames the six weeks as pipeline not
being built rather than a hire not being made.

## 14. Variant B — no-trigger control
Written without the SDR-role reference, to measure what the personalization is
actually worth. If A and B perform identically, the research isn't paying.

## 16. Variables
{{first_name}} → fallback: "Hi there"
{{role_open_weeks}} → fallback: drops to Variant B automatically if empty

## 18. Rejected lines
"Congrats on the growth!" — flattery, no consequence, unverified.
"We help companies 5x their meetings" — unsupported by n=1.
"Are you free Tuesday or Thursday?" — asks for commitment before interest.
```

### Example 2 — Rewriting an email that gets no replies

**Input**

> "This gets a 0.4% reply rate. Fix it: 'Hi {{first_name}}, I hope this email finds you well! My name is [X] and I'm the founder of [Company]. We're a leading provider of AI-powered GTM solutions that help B2B companies scale their outbound and drive revenue growth. We've helped companies like [3 logos] achieve up to 300% more pipeline. I'd love to hop on a quick 15-minute call to show you how we can help. Are you free Thursday at 2pm? Best, [X]'"

**Clarifying questions asked first**

> Two: (1) Is the 300% figure measurable — one client, several, over what period? That determines whether it stays in any form. (2) Who's the recipient, at role level? The rewrite depends entirely on what they're measured on.

**Output shape**

Diagnoses line by line before rewriting, because the pattern is more useful than the replacement:

- *"I hope this email finds you well"* — filler; costs a line of preview space where the value should be.
- *"My name is X and I'm the founder of…"* — the entire opening is about the sender. The reader has no reason to reach sentence two.
- *"leading provider of AI-powered GTM solutions"* — three unsupported superlatives and category jargon the buyer doesn't use about themselves. Also a deliverability liability.
- *"companies like [3 logos]"* — logos without context prove nothing and invite "so what?"
- *"up to 300%"* — "up to" signals a best case presented as typical. Needs downgrading to what the evidence supports, or removing.
- *"I'd love to hop on a quick 15-minute call"* — the sender's want, not the reader's benefit; "quick" and "just 15 minutes" are the two most-ignored phrases in outbound.
- *"Are you free Thursday at 2pm?"* — asks for commitment before interest exists.
- **Structural:** 96 words, and none of them about the recipient. Zero personalization. No problem line at all — which is the actual root cause. The email never names anything the reader would recognize as their situation.

The rewrite drops to ~65 words, opens on a role-owned observable, states a problem in the reader's language, makes a single downgraded claim tied to real evidence, and ends with an interest question. Two variants test different problem lines rather than different phrasings.

Closes with the honest caveat: if the rewrite also underperforms, the issue is upstream — list, offer, or ICP — and copy cannot fix relevance it doesn't have.

### Example 3 — Multi-thread set for one account

**Input**

> "We're going into a 400-person logistics company. I want to reach the COO, the Head of Operations, and the Ops Manager. Same product — a warehouse workflow tool, ~$60k ACV. Three emails, and they'll definitely talk to each other."

**Clarifying questions asked first**

> Three: (1) What research do you have on this specific company — anything observable about how they operate today? (2) Who's sending — one person to all three, or different senders? (3) Any known trigger, like a new facility, a hiring pattern, or a system migration?

**Output shape**

Builds three structurally different emails, and §4 makes the differentiation explicit because the risk here is concrete: three colleagues comparing near-identical emails burns all three threads simultaneously.

- **COO (decision maker)** — three sentences, ~45 words. Outcome and risk framing, no product detail, one question about organizational priority. Different subject line family entirely.
- **Head of Operations (champion candidate)** — longest of the three, ~90 words, written to be forwardable: the problem, the mechanism, one proof point, standing alone without the sender present. This is the email designed to survive being pasted into an internal message.
- **Ops Manager (end user)** — ~70 words, framed entirely around the daily task that stops being manual. Most specific, most credible, lowest ask — a conversation, not an evaluation, because this reader cannot approve $60k.

Also specifies:
- **Sequencing** — Head of Operations first as the most likely champion, COO a week later, Ops Manager alongside. Contacting the COO first risks a downward referral that arrives before the champion has any context.
- **Honest cross-referencing** — if a later email mentions the earlier outreach, it says so plainly. Pretending each contact is independent when they will obviously compare is the fastest credibility loss available.
- **Distinct angles per role**, not one angle in three lengths — the COO email is about operational risk, the Head of Ops email is about throughput, the Ops Manager email is about a specific manual step.
- **§18** flags the $60k ACV implication: at this deal size a technical evaluator and procurement will enter later, so the first-touch claims must be ones that survive verification rather than ones that merely open a door.

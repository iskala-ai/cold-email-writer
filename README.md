# cold-email-writer

A Claude Skill that writes, rewrites, validates, and improves B2B cold emails — a distinct email per buying-committee role, built on a verifiable observation, sized to the evidence behind it, and QA'd for deliverability and compliance before it's sendable.

Part of a 20-skill GTM suite. Single self-contained `SKILL.md`, no dependencies.

---

## What it does

Produces cold emails **under 100 words** that earn a reply, plus the reasoning behind every choice — so the output is a copy decision, not just copy.

Each email has four load-bearing parts:

| Part | Job | Fails when |
|---|---|---|
| **Opening** | Prove this was written for them | Generic, flattering, or provably wrong |
| **Problem** | Name something they'd agree is true | Vendor language they don't use about themselves |
| **Claim** | Give a reason to believe change is possible | Larger than the evidence behind it |
| **CTA** | Make replying easier than ignoring | Asks for more than the recipient can grant |

The most common failure it's built to prevent isn't bad writing — it's an email that's well-written **about the sender**.

---

## Install

Single file. Drop it wherever your Claude surface loads skills from:

```
skills/
└── cold-email-writer/
    └── SKILL.md
```

No `references/`, `assets/`, `scripts/`, or bundled files. Everything is inside `SKILL.md`.

---

## When it triggers

**Use it for:**
- Writing a cold email, first-touch, intro, or breakup email
- Subject lines, preview text, or CTA options
- Rewriting an email that isn't getting replies
- Role variants for multi-threading one account
- Turning research, a signal, or a personalization angle into sendable copy

**Don't use it for** — these hand off to sibling skills:

| Task | Skill |
|---|---|
| Full multi-step sequence architecture | `cold-email-sequence-builder` |
| Defining the ICP or persona | `icp-builder` / `buyer-persona-builder` |
| Generating angles from raw research | `personalization-angle-generator` |
| Domain, inbox, and DNS auditing | `deliverability-auditor` |
| LinkedIn or WhatsApp copy | `linkedin-outreach-writer` / `whatsapp-follow-up-writer` |

---

## What you get

A 19-section output document. The drafts are §14; everything else is the reasoning that makes them defensible.

| § | Section | Why it's there |
|---|---|---|
| 1 | Executive summary | The decision in four sentences |
| 2 | Email snapshot | Word count, angle, claim strength, CTA type, links |
| 3 | Audience & context | Who, what's known, what's assumed |
| 4 | Emails by committee role | Different email per role — not one email with a swapped title |
| 5 | What they own | The email anchors to their remit |
| 6 | Metric & claim | Claim mapped to evidence, downgraded where thin |
| 7 | Outcome framing | Personal vs business outcome |
| 8 | Problem line | **The "would a non-prospect nod?" test** |
| 9 | Relevance & stack framing | How it connects to what they already run |
| 10 | Reason for reaching out now | The trigger, or an honest absence of one |
| 11 | Email by awareness stage | Problem-aware vs solution-aware readers differ |
| 12 | Differentiation line | One clause, if it's needed at all |
| 13 | Objection pre-empt | Handle it before they raise it |
| 14 | **Drafts** | Primary + variants, in full |
| 15 | Subject lines & preview text | Preview space treated as real estate |
| 16 | Personalization variables | With fallbacks that don't break grammar |
| 17 | CTA options | Sized to the recipient's authority |
| 18 | Deliverability, compliance & red flags | Spam triggers, links, identity, opt-out |
| 19 | Test plan & recommended actions | No email is validated until it's sent |

---

## The rules it won't break

- **Never invents proof.** No fabricated case studies, customer names, percentages, or logos.
- **Claims are sized to evidence.** One measured client result stays "one client did X" — it never becomes "clients typically see X."
- **Never invents the trigger.** No "I saw you're hiring" if that wasn't verified. Inferences are softened into hypotheses ("usually that means…") or dropped.
- **CTA never exceeds authority.** An end user who can't approve $60k doesn't get asked to evaluate a $60k purchase.
- **The "so what?" pass.** Every sentence must survive *"so what does that mean for me?"* — if it can't, it comes out.
- **Compliance is part of the copy**, not a footer afterthought: sender identity, opt-out, and jurisdiction handling are checked in §18.

---

## Regional handling

Built for MENA B2B by default:

- **Sunday–Thursday** working week across the Gulf; Friday avoided
- **Ramadan and Eid** shift response rates and appropriate tone materially
- **Bilingual register** — mirrors how the recipient writes rather than defaulting to formal Arabic or English
- Founder- and GM-led decisions are the norm in mid-market EG / KSA / UAE, which changes who the primary email is written for

---

## Quick start

Give Claude the recipient, what you sell, and your best real proof point:

> Write a cold email to the Head of Sales at a 60-person B2B SaaS in Riyadh. They've had an SDR role open six weeks. I sell outbound-as-a-service, ~$4k/month. Best proof: one client went from 2 to 11 meetings a month in 90 days.

It will ask **1–3 clarifying questions first** — usually whether proof can be named or must be anonymized, and who the email comes from, since seniority changes what the email can credibly claim.

See `cold-email-example.md` for a full worked run.

---

## Sibling skills

**Targeting** — icp-builder · buyer-persona-builder · account-researcher · lead-scoring · buying-signal-analyzer
**Messaging** — value-proposition-builder · personalization-angle-generator · **cold-email-writer** · cold-email-sequence-builder · linkedin-outreach-writer · whatsapp-follow-up-writer
**Execution** — campaign-launch-planner · ab-test-generator · deliverability-auditor · campaign-analyzer
**Sales cycle** — discovery-call-prep · objection-handler · meeting-follow-up-writer · proposal-builder · crm-note-formatter

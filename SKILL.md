# Cold Email Writer — Claude Skill

A standalone Claude Skill that writes, rewrites, validates, and improves B2B cold emails.

It creates a distinct email for each buying-committee role using verifiable personalization, a problem the recipient recognizes, claims supported by real evidence, and a CTA matched to the recipient’s authority.

The Skill also reviews each email for clarity, deliverability, spam triggers, and compliance before it is ready to send.

The core Skill is fully contained in a single `SKILL.md` file with no external dependencies.

---

## What it does

Produces cold emails **under 100 words** designed to earn replies, plus the reasoning behind every copy decision.

Each email has four load-bearing parts:

| Part | Job | Fails when |
|---|---|---|
| **Opening** | Prove this was written for the recipient | Generic, flattering, or inaccurate |
| **Problem** | Name something the recipient recognizes as true | Uses vendor language instead of the recipient’s language |
| **Claim** | Give a credible reason to believe change is possible | Makes a claim larger than the available evidence |
| **CTA** | Make replying easier than ignoring | Asks for more than the recipient can approve |

The most common failure it is designed to prevent is not bad writing. It is an email that is well-written **about the sender**.

Every sentence must survive this question:

> “So what does that mean for me?”

---

## Installation

The core Skill is contained in one file.

Place it wherever your Claude environment loads Skills from:

```text
skills/
└── cold-email-writer/
    └── SKILL.md
```

No scripts, external tools, or additional dependencies are required.

The downloadable package includes:

```text
cold-email-writer/
├── SKILL.md
├── README.md
└── cold-email-example.md
```

---

## When to use it

Use Cold Email Writer for:

- Writing first-touch cold emails
- Writing outbound, intro, breakup, or re-engagement emails
- Generating subject lines and preview text
- Creating CTA options
- Rewriting emails that are not receiving replies
- Creating distinct email variants for different buying-committee roles
- Turning verified research or a buying signal into sendable copy
- Reviewing email length, clarity, deliverability, and compliance
- Creating personalization variables with safe fallbacks

---

## What it does not cover

Cold Email Writer is focused specifically on writing and improving individual B2B cold emails.

It does not cover:

- Full multi-step email sequence architecture
- ICP or buyer persona development
- Generating personalization angles from raw research
- Domain, inbox, DNS, or sending-infrastructure audits
- LinkedIn or WhatsApp outreach copy

---

## How it works

The Skill follows a 32-step workflow across four phases:

| Phase | Steps | What happens |
|---|---:|---|
| **1** | 1–9 | Writes a different email for each buying-committee role |
| **2** | 10–17 | Builds the substance: the metric, problem, and observable details |
| **3** | 18–24 | Sizes the claim to the evidence and calibrates the CTA |
| **4** | 25–32 | Writes, runs QA, checks deliverability and compliance, and defines the test plan |

---

## What you get

The Skill produces a structured 19-section output.

The final drafts appear in section 14. The other sections explain the copy decisions and make the output easier to review and defend.

| § | Section | Purpose |
|---:|---|---|
| 1 | Executive summary | Summarizes the recipient, angle, claim, and CTA |
| 2 | Email snapshot | Shows word count, angle, claim strength, CTA type, and links |
| 3 | Audience and context | Defines what is known and what is assumed |
| 4 | Emails by committee role | Creates distinct copy for each relevant role |
| 5 | What they own | Connects the email to the recipient’s responsibility |
| 6 | Metric and claim | Maps each claim to available evidence |
| 7 | Outcome framing | Separates personal and business outcomes |
| 8 | Problem line | Tests whether the problem is specific enough |
| 9 | Relevance and stack framing | Connects the message to the current workflow |
| 10 | Reason for reaching out now | Uses a verified trigger or names its absence |
| 11 | Email by awareness stage | Adjusts the message to the recipient’s awareness |
| 12 | Differentiation line | Explains the difference in one clause |
| 13 | Objection pre-emption | Handles likely objections concisely |
| 14 | **Drafts** | Provides the primary email and alternative variants |
| 15 | Subject lines and preview text | Provides short subject lines and supporting preview text |
| 16 | Personalization variables | Defines variables and fallbacks |
| 17 | CTA options | Matches the ask to the recipient’s authority |
| 18 | Deliverability, compliance, and red flags | Reviews spam risks, identity, links, and opt-out requirements |
| 19 | Test plan and recommended actions | Defines how the copy should be tested |

Inferences are tagged `[assumption]`, and every claim is mapped to evidence.

---

## Rules the Skill follows

- **Never invents facts about the recipient.**  
  No fabricated posts, hires, funding, launches, tools, or headcounts.

- **Never invents proof.**  
  No fabricated case studies, customer names, percentages, testimonials, or benchmark statistics.

- **Claims are sized to the evidence.**  
  One customer’s result stays “one customer’s result.” It never becomes “clients typically see.”

- **Uncertain inferences are phrased as questions.**  
  For example: “Is that intended to add capacity or replace someone?”

- **Never fabricates familiarity.**  
  No invented mutual connections, false prior conversations, or misleading `Re:` and `Fwd:` subject lines.

- **Never references behavioural tracking.**  
  No page visits, email opens, profile views, or private intent activity in the copy.

- **The CTA never exceeds the recipient’s authority.**  
  Someone who cannot approve a purchase is not asked to evaluate or approve it.

- **One email carries one main idea.**  
  A second idea becomes a different email or variant.

- **Every email is reviewed from the recipient’s perspective.**  
  Sentences that do not answer “why should I care?” are removed.

- **Compliance is part of the review.**  
  Sender identity, opt-out requirements, and jurisdiction considerations are checked before the email is considered sendable.

Compliance guidance is general information and not legal advice. Requirements vary by jurisdiction.

---

## Regional handling

Cold Email Writer is designed with MENA B2B communication in mind:

- A slightly warmer opening may work better than an overly terse US-style pattern
- Clear sender identity is treated as important
- Arabic and English can be mixed naturally where appropriate
- The Skill mirrors the recipient’s own language and communication style
- Tone can be adapted for Egypt, Saudi Arabia, the UAE, and other MENA markets
- Role-specific copy can account for founder- and General Manager-led buying decisions

---

## Quick start

Give Claude the recipient, offer, problem, verified research, and strongest real proof point.

```text
Use the Cold Email Writer Skill to write a first-touch email.

Recipient:
Head of Sales at a 60-person B2B SaaS company in Riyadh.

Offer:
Outbound-as-a-service at approximately $4,000 per month.

Problem:
The company is hiring an SDR but does not yet have a consistent outbound system.

Verified research:
The SDR role has been open for six weeks.

Evidence:
One similar client increased qualified meetings from 2 to 11 per month in 90 days.

CTA goal:
Get a reply confirming whether building pipeline before completing the hire is currently a priority.

Sender:
Engy, Business Developer at iSkala.

Please provide:
- One primary email under 100 words
- Two materially different variants
- Three subject lines
- Preview text
- One CTA
```

Claude may ask a small batch of clarifying questions before producing the final email.

The most important inputs are:

1. Who the recipient is
2. What the offer solves for that role
3. What verified research or usable evidence exists

Other useful inputs include:

- CTA goal
- Sender identity
- Whether this is one email or a reusable template
- Prior contact
- Recipient jurisdiction
- Tone-of-voice requirements

When some information is unavailable, the Skill identifies which parts of the output rely on assumptions.

---

## Worked examples

The Skill includes three worked scenarios:

- **First touch from research** — turns a verified signal into a full draft and variants
- **Rewriting an email that gets no replies** — diagnoses the original copy before rewriting it
- **Multi-threading one account** — creates distinct emails for different buying-committee roles

The downloadable package also includes:

```text
cold-email-example.md
```

This file contains an additional practical example.

---

## Important notes

- Verify all recipient information before sending.
- Only use customer results that are accurate and approved for public use.
- Add a real sender identity.
- Include an appropriate opt-out mechanism.
- Review the legal requirements that apply to the recipient’s jurisdiction.
- Test the emails on a meaningful sample before selecting a winning version.
- Treat deliverability and compliance guidance as general information, not legal advice.

---

Created by **iSkala Business Solutions**.

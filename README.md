# Inkbound

A new home for global writing challenges. Pre-launch.

**Live:** https://tomgarske.github.io/inkbound/ *(landing-page stencil)*

This is a wireframe of the marketing site. Brand name "Inkbound" is a placeholder until the real name is chosen. The page is intentionally pre-launch — no fabricated history, no testimonials, no winners. Everything points to the inaugural 2026 cycle.

## Companion research

Sister repo: [nycm-2026](https://github.com/TomGarske/nycm-2026) — an analytics dashboard built against the in-flight 500-word challenge from the incumbent. It maps 3,456 real writers, scores group competitive density, and surfaces returning finalists. The findings shaped what's in this stencil.

---

## What it would take to actually run the first competition

Honest checklist. Items are sized roughly **S** (a day or two), **M** (a week), **L** (a month+), **XL** (multi-month / specialist).

### Tier 1 — required before you can take a single dollar from a writer

| Item | Size | Notes |
|---|---|---|
| **Real brand name + domain** | S | "Inkbound" is a placeholder. Check trademark, register `.com`, secure social handles. |
| **Legal entity** | M | LLC (Delaware or home-state) with a business bank account. Talk to a small-business attorney about contest-specific liability. |
| **Official contest rules** | M | The legally binding document. NYC Midnight's [rules page](https://www.nycmidnight.com/rules) is the precedent — eligibility, prize structure, IP, dispute resolution, governing law, void-where-prohibited. Get an attorney to review before publishing. |
| **Terms of service + privacy policy** | S–M | Standard SaaS templates plus GDPR/CCPA compliance language since the audience is international. |
| **Payment processing** | M | Stripe account, terms-of-service signoff, refund flow, dispute handling. Plan for chargebacks. International cards = currency conversion fees built into pricing. |
| **Submission upload infrastructure** | M–L | Two options: (a) use **Submittable** (NYC Midnight does this — saves ~6 months of dev time; fees ~5-10%), or (b) build your own with file upload, anonymization, judge-assignment, scoring rubric, feedback editor. Buy first; build later if scale warrants. |
| **Email infrastructure** | S | Transactional emails (confirmation, kickoff) + newsletter. Resend, Postmark, or Mailchimp. |
| **Initial prize money in the bank** | M | $12K per challenge if matching NYC Midnight's 500-word tier. For inaugural cycle, prizes need to be *funded in advance* before registration opens — writers won't trust a "we'll pay if we hit volume" promise. |
| **Judges panel** | L | Working editors, agents, published authors. 5–15 per challenge depending on entry volume. Compensation: NYC Midnight pays $50–$200 per round per judge. Recruit via personal network first; expand via Poets & Writers / lit-mag editor outreach. |
| **Judging system** | M | Anonymized story → judge assignment → rubric scoring → feedback collection → tally + advance list. Submittable does this; otherwise build it. |
| **Anti-AI policy + enforcement** | M | NYC Midnight bans AI; this is a real differentiator now. Need a stated policy + detection plan. Open question: how do you actually catch it? GPTZero / Originality.ai have known false-positive rates. Consider: judges flag suspect entries → manual review process. |
| **Anti-plagiarism check** | S | Copyscape or similar. Run on all advancing entries before announcing results. |
| **Customer support** | M | One person for the first cycle — refund requests, technical issues, "I didn't get my prompt email" tickets. Expect 5–10% of entrants to email at some point. |
| **Marketing funnel + seed audience** | XL | The hardest part. NYC Midnight has 20+ years of reputation; you have zero. Plausible launch paths: Reddit (r/writing, r/shortstories), Substack writer-friendly newsletters, Poets & Writers calendar listing, paid Google/Meta. Realistic year-one volume: 200–1000 writers for the first challenge if you market hard. |

### Tier 2 — must exist by the time the first competition concludes (~6 months out)

| Item | Size | Notes |
|---|---|---|
| **Forum / community** | M | NYC Midnight's forum is a major retention tool — writers discuss prompts, swap feedback, build cohorts. Use Discourse (self-hosted) or Circle.so. Pre-launch sign-ups should land here, not just an email list. |
| **Anthology print partner** | M | KDP for low-volume / no MOQ, IngramSpark for bookstore distribution. Cover designer + interior layout. Pricing: $14.95 print, $4.99 digital is the common ladder. |
| **Online lit journal CMS** | M | "Inkbound Quarterly" needs a real publishing platform. Substack (free, slow) or Ghost ($9/mo+, faster) work. Editorial staff = 1 part-time editor minimum. |
| **Agent / editor panel partnerships** | L | This is the biggest publishing-pathway promise. Realistically only useful if you can actually get 3–5 named agents to commit to reading top-3 from each round. Cold outreach with the dashboard data as evidence of seriousness. |
| **Charity partner agreements** | S | NYC Midnight lists 7 charities. For Inkbound, start with 3–4 — Doctors Without Borders, World Central Kitchen, NRDC, Room to Read. Sign donation MOUs so partners are prepared to receive funds + receipts. |
| **Analytics + funnel tracking** | S | Plausible / Fathom / GA4 — basic page-view and conversion tracking. Helps measure which marketing channels actually drive registrations. |
| **1099 / W-9 collection for winners** | S | US contest winners over $600 need a 1099-MISC at year-end. International winners need separate treatment. Set up form collection in checkout flow. |

### Tier 3 — when scaling (year 2+, when entry volume > 2,000)

| Item | Size | Notes |
|---|---|---|
| **Liability insurance** | M | General business + contest-specific. ~$1–3K/year for a small contest. |
| **Dedicated submission platform** | L–XL | If Submittable fees become material at scale, building your own pays for itself. |
| **Multi-jurisdiction tax compliance** | L | VAT for EU/UK writers, GST for AU. Stripe Tax handles most of it. |
| **Staff** | XL | Operations manager, marketing, editorial. NYC Midnight runs lean (~5 FTE for ~25K writers/year across all challenges). |
| **Sponsorships** | L | Print magazines, literary presses, MFA programs as sponsors. Real revenue diversifier once you have audience. |

---

## The hardest unsolved problems

1. **Cold start** — Writers compete *to be seen by other writers and editors*. Without an existing audience, the prize money and feedback matter less. NYC Midnight's flywheel is 20 years old; replicating it from zero is a 3–5 year project.

2. **AI policy enforcement** — The "no AI" promise is now a differentiator, but actually detecting it is hard. Need a credible policy that's not just performative.

3. **Judge quality** — Cheap judges = unreliable feedback = writers don't come back. Paying competitive rates ($100+/round/judge) on 1,000 entries = $5–10K judging cost per challenge. The math gets tight fast.

4. **Why would the first writer sign up?** — Need a single sharp answer. Likely candidates: (a) faster feedback than NYC Midnight, (b) a specific publishing pathway (anthology + agent intro) NYC Midnight doesn't offer, (c) a niche format NYC Midnight doesn't run.

---

## Stack

- Static one-page HTML
- Inline CSS + tiny JS for challenge card rendering
- No build step
- Deployed via GitHub Pages

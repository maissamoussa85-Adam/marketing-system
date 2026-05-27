# TinyMCE AI Upsell — Tiered Account Strategy

**Product:** Tiny AI Assistant (AI writing upsell on TinyMCE core licence)
**Prepared by:** Maissa Moussa, Sales Development Operations
**Dataset source:** Dagmara, Sales Development Operations Specialist — Salesforce enrichment, Stitch sync confirmed May 2026
**Campaign reference:** LinkedIn ABM Report, week of 23–29 March 2026

---

## The Problem

- Dagmara's dataset identified **162 AI Upsell accounts**. Only **36–48 are active paying customers** with live ACV. The rest are churned or historical.
- Total LinkedIn budget: **$4,000 (ABM budget)**. Spread equally = ~$25 per account = zero measurable impact.
- Prior Gong cold sequences produced clicks but **zero meeting bookings** — cold outreach without a prior relationship has no conversion trigger.

---

## What the March 2026 Campaign Taught Us

| Metric | Company List | Contact List | Winner |
|---|---|---|---|
| CTR | 0.35% | 0.38% | Contact List |
| Cost per click | $8.46 | $6.80 | Contact List |
| Reach | 3,422 | 907 | Company List (volume only) |
| Risk | Google took 61% of impressions | Scoped to named contacts | Contact List |

**Best-performing title:** Group Product Manager — 0.63% CTR
**Best-performing creative:** Build vs. Buy video (0.77% CTR) and static (0.38% CTR)

---

## Scoring Model (0–100)

Every account scored using Dagmara's Salesforce data across six dimensions:

| Dimension | Weight | What It Measures |
|---|---|---|
| Annual ACV | 30 pts | Is this a paying customer today? |
| Lifetime ACV | 15 pts | Total relationship value over time |
| AI Adjacency | 20 pts | Is their product already AI-adjacent? |
| TinyMCE Centrality | 15 pts | Is TinyMCE core to their product? |
| Reachability | 10 pts | Do we have named contacts (GPM, VP Eng)? |
| Recency | 10 pts | Last activity — are they engaged? |

**Tier thresholds:** Score 81+ = Tier 1 · Score 60–80 = Tier 2 · Below 60 = Tier 3

---

## Tier 1 — Concentrated and Personalised
**6 accounts · $3,200 LinkedIn Contact List · Warm Gong re-engagement**
All six are existing TinyMCE customers with active contracts and named SAE contacts.

| Account | Score | Annual ACV | Lifetime ACV | LinkedIn Budget |
|---|---|---|---|---|
| Collibra Belgium BV | 92 | $129,712 | $1,417,261 | $600 |
| 1&1 Mail & Media GmbH | 91 | $146,430 | $515,004 | $600 |
| Sierra Interactive | 90 | $98,886 | $1,600,184 | $600 |
| UBS Financial Services | 89 | $134,275 | $1,358,795 | $600 |
| Google (Delivery Navigator) | 85 | $87,500 | $612,684 | $400 (hard cap $150/wk) |
| LogicGate Inc. | 81 | $60,786 | $1,058,998 | $400 |

> **Google note:** Contact List ONLY. Company list excluded — drove 61% impression-absorption in March campaign.

---

## Tier 2 — Nurture and CSM-Led
**16 accounts · $800 shared LinkedIn pool · InMail + CSM email reactivation**

| Account | Score | Annual ACV | Primary Channel |
|---|---|---|---|
| aNewSpring | 78 | $83,175 | LinkedIn shared pool + Gong |
| ADP Works | 70 | $69,030 | LinkedIn shared pool + AE outreach |
| Sedna Communications | 70 | $36,416 | LinkedIn shared pool + Gong |
| InContact (NICE) | 69 | $52,817 | LinkedIn nurture + product webinar |
| FranConnect | 68 | $48,160 | LinkedIn nurture + partner content |
| Revenue.io | 67 | $31,955 | LinkedIn nurture + Gong |
| Jenzabar | 62 | $23,445 | LinkedIn nurture + EdTech webinar |
| Dev Apploi | 65 | $45,118 | CSM email reactivation + healthcare content |
| Enate | 64 | $42,374 | CSM email reactivation |
| Erste Digital GmbH | 63 | $41,134 | CSM email reactivation + FinServ webinar |
| IntelliGRC | 61 | $25,001 | CSM email reactivation + compliance webinar |
| DLGL Technologies Corporation | 61 | $24,300 | CSM email reactivation |
| Intrepid — VitalSource | 61 | $23,010 | CSM email reactivation + learning webinar |
| Solve Intelligence | 61 | $19,683 | CSM email reactivation |
| Simplify Healthcare | 60 | $23,232 | CSM email reactivation + healthcare content |
| C2Perform | 60 | $25,972 | CSM email reactivation |

---

## Tier 3 — Awareness Only
**~130 accounts · $0 LinkedIn · Content syndication + product newsletter**

| Channel | Vertical / Account |
|---|---|
| Content syndication | GRC / Compliance |
| Content syndication | LMS / EdTech |
| Content syndication | CRM / Sales Enablement |
| Content syndication | FinTech / Banking |
| Product newsletter | All verticals |
| CSM win-back | Moodle ($3.57M LTV) |
| CSM win-back | Legislative Services Agency ($1.27M LTV) |

---

## Budget Summary

| Tier | Accounts | LinkedIn Budget | Source |
|---|---|---|---|
| Tier 1 | 6 | $3,200 | ABM budget (confirmed) |
| Tier 2 | 16 | $800 | ABM budget (confirmed) |
| Tier 3 | ~130 | $0 LinkedIn | Existing marketing budget |
| **Total** | | **$4,000** | |

> **Open item:** Confirm with Caroline (Paid Media) whether additional budget is available. If yes, Tier 2 CSM-only accounts move to dedicated Contact List campaigns — guaranteed reach vs. shared pool distribution.

---

## Why Gong Works Differently in Tier 1

Cold sequences produced clicks but zero meetings — no existing relationship means no reason to respond.

Tier 1 accounts are existing paying customers with live contracts. Gong re-engagement here is warm outreach about upgrading a product they already use, not cold prospecting. Expected response rate is materially higher.

**Rule:** Gong sequences for Tier 1 and Tier 2 existing customers only. Cold sequences on $0 ACV accounts retired.

---

## Next Steps

- [ ] PMM (Bee Lawless) — confirm content and creative per tier
- [ ] Caroline (Paid Media) — confirm whether additional budget is available beyond $4,000
- [ ] Build LinkedIn Contact List audiences from SAE named contact database
- [ ] Launch Tier 1 campaigns within 2 weeks of alignment
- [ ] 60-day check-in — meetings booked and pipeline opportunities per tier

---

## Reuse Notes for Future Projects

This playbook is designed to be reusable. For a new product or campaign:

1. Replace `account-channel-matrix.csv` with the new scored account list (keep the same column headers)
2. Adjust tier thresholds in the scoring model if the account pool size changes
3. Update the budget figures and LinkedIn allocation per tier
4. The GitHub Actions workflow (`abm-account-tier-validation.yml`) will automatically validate the new CSV and generate a tier summary on push

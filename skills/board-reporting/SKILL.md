---
name: board-reporting
last_reviewed: 2026-09-06
group: Fundraising and board
description: Draft the board pack: executive summary, financial dashboard, and governance agenda. For investor metrics, see saas-metrics. Use when preparing quarterly board decks or KPI packets.
---

# board-reporting

## Core Philosophy
A quarterly board meeting is not a performance theater where the executive team reads 80 slides of vanity metrics to prove they worked hard. A board of directors exists to govern corporate fiduciary duty, challenge strategic assumptions, unblock operational gridlock, and allocate capital. Great board reporting is radical transparency: leading with unvarnished lowlights and strategic risks before celebrating wins, anchoring performance in core SaaS financial metrics, and focusing meeting time on high-stakes strategic debates.

---

## 4-Step Executive Board Pack Architecture

### Step 1: The 1-Page CEO Executive Letter (The Narrative Anchor)
1. **The 3 Mandatory Sections**:
   - *Highlights (Top 3 Wins)*: Hard business milestones delivered (e.g. "Closed $1.2M ARR, shipped v3.0, hired VP of Sales").
   - *Lowlights & Misses (Top 3 Failures)*: Transparent ownership of misses (e.g. "Enterprise churn rose to 3.2% due to SOC 2 delay; missed outbound pipeline target by 18%").
   - *Where the Board Can Help (Explicit Asks)*: Specific introductions (e.g. "Need warm intro to Head of Procurement at TargetCo; seeking advice on European expansion tax structure").

### Step 2: SaaS Financial Dashboard & Runway Telemetry
1. **The Core Financial Grid**:
   - *Ending ARR / Net New ARR*: Actual vs Board Budget vs Previous Quarter.
   - *Net Burn & Cash Runway*: Total cash in bank, monthly burn rate, zero-cash date (runway in months).
   - *Gross Margin*: Must be $\ge 75\%$ for software.
   - *Efficiency Metrics*:
     - **Rule of 40**: $text{ARR Growth Rate (\%)} + text{Free Cash Flow Margin (\%)}$.
     - **Magic Number**: $rac{text{Net New ARR (Current Quarter)}  imes 4}{text{Previous Quarter S&M Spend}}$. (Target $\ge 0.75$).

### Step 3: Operational Departmental Health Scorecard
1. **Sales & Marketing**:
   - Pipeline coverage, win rates, CAC Payback Period (in months), Magic Number.
2. **Product & Engineering**:
   - Feature roadmap delivery status, platform uptime SLA (e.g. 99.98%), mean time to resolve (MTTR) P1 bugs.
3. **Customer Success & Retention**:
   - Logo Churn % vs Net Revenue Retention (NRR). Benchmark: NRR $> 110\%$ for top-quartile enterprise SaaS.

### Step 4: Strategic Deep Dive & Governance Consent Agenda
1. **The Strategic Discussion Topic (45 Minutes)**:
   - Dedicate the bulk of the board meeting to **one** major strategic decision (e.g. "Should we build our own payment rail or white-label Stripe?").
2. **Consent Agenda (Fast Governance)**:
   - Bundle routine legal items (stock option grants, 409A valuation adoption, minutes approval) into a consent agenda voted on in the first 5 minutes.

---

## Deliverable Format: Quarterly Board Memorandum (`BOARD-PACK.md`)

```markdown
# Quarterly Board of Directors Pack: [Quarter / Year]
*Date: [YYYY-MM-DD] | Confidential | Prepared for the Board of Directors*

## 1. CEO Executive Overview
### Highlights
- Net New ARR reached **+$420,000** (105% of board plan).
- Shipped automated compliance scanner on schedule; 45 active enterprise pilots.

### Lowlights & Challenges
- Enterprise logo churn increased from 1.2% to **2.8%** due to legacy database latency.
- S&M CAC payback widened from 12 months to **17 months**; pausing underperforming paid channels.

### Key Asks for Directors
- Warm introductions to CISO leaders at Fortune 500 banks.
- Compensation committee review for new VP of Engineering equity grant.

## 2. Executive Financial Scorecard
| Metric | Q2 Actual | Q2 Budget | Variance | Prior Year Q2 |
|---|---|---|---|---|
| Total Ending ARR | $4,820,000 | $4,600,000 | +4.7% | $2,900,000 |
| Cash in Bank | $6,200,000 | $6,000,000 | +$200k | $4,100,000 |
| Net Monthly Burn | $185,000 | $210,000 | -$25k (Favorable)| $140,000 |
| Cash Runway | **33.5 Months** | 28.5 Months | +5.0 Mos | 29.0 Months |
| Net Revenue Retention (NRR) | **114.2%** | 110.0% | +4.2% | 108.0% |
| Rule of 40 Score | **44.8%** | 40.0% | +4.8% | 38.0% |

## 3. Strategic Deep Dive Topic: International Expansion (EMEA)
- **Problem**: 28% of inbound organic traffic originates from Germany and UK, but conversion lags due to lack of local EU data residency.
- **Proposal**: Allocate $150k to stand up AWS Frankfurt datacenter region in Q3.
```

---

## Worked Example: Turning a Crisis into Board Alignment

- **Situation**: Startup missed quarterly ARR target by 25% due to an unexpected sales cycle lengthening.
- **Board Pack Strategy**: CEO owned the miss on page 1 with zero excuses. Delivered a rigorous root-cause analysis showing deals slipped into the next quarter rather than being lost to competitors.
- **Board Response**: Directors praised the intellectual honesty; helped restructure the enterprise pricing tier during the deep-dive discussion; all 3 slipped deals closed within 30 days.

---

## Verification Checklist

- [ ] CEO letter leads with unvarnished lowlights and explicit asks before highlights.
- [ ] Financial table reports ARR, Net Burn, Cash Runway, NRR, and Rule of 40 against budget.
- [ ] Board pack distributed at least **72 hours (3 business days)** prior to the meeting.
- [ ] Routine governance items (options, minutes) consolidated into a fast Consent Agenda.
- [ ] Meeting agenda reserves at least 50% of time for strategic discussion, not slide reading.

---

## Anti-Patterns

- **Surprising the Board**: Revealing a catastrophic cash shortage or key executive departure for the first time during the live meeting.
- **Vanity Slide Bloat**: Sending a 90-slide PDF where real financial metrics are buried behind marketing screenshots.
- **Defensive Justification**: Spending 40 minutes arguing with board members instead of absorbing feedback and advice.

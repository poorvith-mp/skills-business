---
name: decision-making
last_reviewed: 2026-09-06
group: Strategy
description: >-
  Generate options and choose: divergent methods, RACI, scoring, decision trees, and inversion.
  Use when evaluating high-stakes decisions or trade-offs.
---

# decision-making

## Core Philosophy
High-stakes decision-making in leadership is not relying on intuition, gut feelings, or consensus-seeking committee votes. Bad decisions stem from cognitive biases: confirmation bias, sunk cost fallacies, groupthink, and status-quo inertia. World-class decision-making is a systematic, probabilistic discipline. It requires classifying decision reversibility (Jeff Bezos' Type 1 vs Type 2 framework), applying inversion, running pre-mortems to expose blind spots, and establishing explicit RACI accountability.

---

## 4-Step Strategic Decision-Making Framework

### Step 1: Decision Reversibility Triage (Type 1 vs Type 2)
1. **The Two-Way Door vs One-Way Door Filter**:
   - *Type 1 (One-Way Door - Irreversible / High Impact)*: Selling the company, changing corporate entity structure, signing a 5-year lease, firing a co-founder. Requires exhaustive analysis, divergent exploration, and deliberate slowing down.
   - *Type 2 (Two-Way Door - Reversible / Moderate Impact)*: Launching a marketing campaign, tweaking pricing packaging, redesigning a landing page, testing a new feature. **Execute immediately with high velocity**. If it fails, open the door and walk back.
2. **The Bias for Action Rule**:
   - Most organizational gridlock occurs when teams treat lightweight Type 2 decisions as if they are catastrophic Type 1 decisions.

### Step 2: Divergent Generation & Inversion (Charlie Munger)
1. **The Rule of 3 Options**:
   - Never make a binary decision ("Should we build Feature X or not?"). Always generate at least 3 fundamentally distinct viable alternatives.
2. **Inversion Analysis ("Invert, Always Invert")**:
   - Instead of asking: *"How do we make this launch a massive success?"*
   - Ask: *"How could we guarantee this launch turns into a complete disaster?"*
   - List every failure catalyst (e.g. database locks, confusing pricing, broken signup, missed SLA) and systematically engineer preventative safeguards against each.

### Step 3: The Pre-Mortem Protocol & Probabilistic Expected Value
1. **The Gary Klein Pre-Mortem**:
   - Gather key stakeholders 48 hours before signing off on the decision.
   - Prompt: *"Imagine we are 12 months in the future, and this initiative has completely failed. Our budget is blown, customers are furious, and our servers are dead. In the next 10 minutes, write down the exact story of why we failed."*
   - Surfaces hidden political anxieties and unvoiced engineering concerns.
2. **Expected Monetary Value (EMV) Decision Trees**:
   - When facing financial trade-offs:
     $$text{EMV} = \sum (P_i  imes text{Outcome}_i)$$
   - Calculate expected value across optimistic, realistic, and pessimistic probability scenarios.

### Step 4: Governance & The RACI Matrix
1. **Single Accountable Decision Maker**:
   - Consensus breeds mediocrity. Every decision must have exactly **one Accountable (A)** individual who has the authority to make the final call, even if the team disagrees and commits.

---

## Deliverable Format: Strategic Decision Memo (`DECISION-RECORD.md`)

```markdown
# Strategic Decision Memorandum: [Decision Title]
*Date: [YYYY-MM-DD] | Decision Owner (Accountable): [Name, Title]*

## 1. Decision Classification & Core Question
- **Decision Question**: Should we rewrite our core backend API in Go or maintain our current TypeScript codebase?
- **Decision Type**: **TYPE 1 (One-Way Door)** — High migration cost, 6-month engineering lock.

## 2. Evaluated Alternatives
| Dimension | Option A: Full Rewrite in Go | Option B: Optimize Existing TypeScript | Option C: Hybrid (Go Worker for Hot Paths)|
|---|---|---|---|
| Development Velocity | High disruption (4 mos) | Immediate | Moderate (4 weeks) |
| Latency Ceiling (p99) | < 15ms (10x gain) | ~120ms (Current) | < 25ms (5x gain) |
| Team Training Overhead| High (Team knows TS) | Zero | Low (Only 2 devs learn Go) |
| 12-Month Infra Cost | $60,000 / year | $180,000 / year | $85,000 / year |

## 3. Pre-Mortem Findings (Why This Could Fail)
- *Risk 1*: Full rewrite drags from 4 months into 9 months, halting product feature roadmap.
- *Mitigation*: Reject Option A. Adopt **Option C (Hybrid)** to bound risk.

## 4. Final Decision & Rationale
- **Chosen Course**: **Option C: Hybrid Go Worker Architecture**.
- **Rationale**: Captures 80% of the latency and compute savings while protecting feature roadmap velocity.
- **RACI**: Accountable: VP Eng | Responsible: Staff Backend Dev | Consulted: Product Director | Informed: All Engineering.
```

---

## Worked Example: Resolving Co-Founder Deadlock on Pricing

- **Deadlock**: Founders argued for 6 weeks over freemium vs 14-day free trial.
- **Resolution**: Classified decision as Type 2 (Two-Way Door). Decided to run a 30-day split test in production with explicit kill metrics.
- **Outcome**: Data proved free trial generated 3x higher paid conversion; debate settled with zero emotional friction.

---

## Verification Checklist

- [ ] Decision classified as Type 1 (irreversible) or Type 2 (reversible).
- [ ] At least 3 distinct alternatives evaluated in a comparison matrix.
- [ ] Pre-mortem conducted to uncover silent risks and failure modes.
- [ ] Inversion exercise executed to identify actions to avoid.
- [ ] Single Accountable owner (RACI) designated with authority to decide.

---

## Anti-Patterns

- **Consensus-Seeking Paralysis**: Waiting for 10 people to agree 100% on a simple reversible decision.
- **Sunk Cost Fallacy**: Continuing to throw money at a failing project because "we've already spent $200k on it".
- **Binary Blindness**: Framing complex strategic choices as simple "Yes/No" questions without exploring hybrid alternatives.

---
name: okrs
last_reviewed: 2026-09-06
group: Product and delivery
description: >-
  Write measurable objectives and key results with cascading alignment from company to individual.
  Use when drafting company or team OKRs, metric ladders, and scoring.
---

# okrs

## Core Philosophy
Objectives and Key Results (OKRs) are not a micromanagement task checklist, nor are they an annual corporate HR performance appraisal system. Originating with Andy Grove at Intel and popularized by John Doerr, OKRs are an operational alignment and ambition engine. Objectives define qualitative, inspirational direction; Key Results define aggressive, quantitative, mathematically verifiable outcomes. If an OKR does not influence daily resource allocation decisions, it is useless bureaucracy.

---

## 4-Step Scalable OKR Architecture

### Step 1: The Objective (Qualitative & Directional)
1. **The Anatomy of a Great Objective**:
   - Must be qualitative, ambitious, memorable, and time-bound.
   - Answers: *"Where do we want to go this quarter?"*
   - Avoid task language: Never write "Ship the new billing API" (that is a project, not an objective).
   - Write: *"Establish our platform as the undeniable gold standard for enterprise database reliability."*

### Step 2: The Key Results (Quantitative & Falsifiable)
1. **The Key Result Standard (From X to Y by Date)**:
   - Must be strictly measurable and verifiable. A Key Result has a number, a baseline, and a target:
     $$text{"Increase [Metric] from [Baseline X] to [Target Y] by [Date]"}$$
   - *Bad Key Result*: "Improve test coverage."
   - *Great Key Result*: "Increase automated unit test coverage from 62% to 85% by end of Q3."
   - *Great Key Result*: "Slash p99 database query latency from 420ms to under 50ms across 10M daily requests."
2. **The 3–5 Rule**:
   - Maximum **3 to 5 Key Results** per Objective. Any more dilutes focus.

### Step 3: Committed vs Aspirational (Moonshot) OKRs
1. **The Two OKR Tiers**:
   - *Committed OKRs (1.0 = 100% Target)*: Essential operational deliverables (e.g. 99.99% uptime, security audit compliance, bug zero). Expected achievement score is **1.0 (100%)**. Missing a committed OKR requires an operational post-mortem.
   - *Aspirational / Moonshot OKRs (0.7 = Success)*: Bold, high-uncertainty growth bets. Success is defined as achieving **0.7 (70%)**. If a team hits 100% on all moonshot OKRs every quarter, their goals were sandbagged.

### Step 4: Scoring, Weekly Check-Ins & Decoupling from Comp
1. **The Weekly 15-Minute OKR Pulse**:
   - Check in weekly during sprint planning: Update confidence scores (0.0 to 1.0) on each Key Result.
2. **Decoupling from Compensation (The Golden Rule)**:
   - **Never tie individual bonuses or salary increases directly to OKR score completion.**
   - Doing so incentivizes sandbagging: teams set laughably easy goals to ensure 100% bonus payouts, destroying corporate innovation.

---

## Deliverable Format: Quarterly Company & Engineering OKR Specification (`OKRS.md`)

```markdown
# Q3 Company & Engineering OKRs: [Quarter / Year]

## Company Objective: Accelerate Enterprise Market Penetration
- **KR 1 (Committed)**: Achieve SOC 2 Type II compliance audit certification by September 15.
  - *Baseline*: Type I achieved | *Target*: Type II certified | *Confidence*: 0.9 | *Owner*: Head of Security
- **KR 2 (Aspirational)**: Grow Enterprise Tier ARR from $450,000 to $1,200,000.
  - *Baseline*: $450k | *Target*: $1.2M | *Confidence*: 0.7 | *Owner*: VP Sales
- **KR 3 (Committed)**: Maintain production platform availability >= 99.98%.
  - *Baseline*: 99.95% | *Target*: 99.98% | *Confidence*: 1.0 | *Owner*: SRE Lead

---

## Engineering Squad Objective: Deliver Lightning-Fast Local Development
- **KR 1 (Aspirational)**: Reduce local CLI container cold-boot time from 14.2s to < 2.0s.
  - *Baseline*: 14.2s | *Target*: 1.8s | *Confidence*: 0.6 | *Owner*: Staff Platform Engineer
- **KR 2 (Committed)**: Zero open P1/P2 regression bugs in production for 60 consecutive days.
  - *Baseline*: 4 bugs | *Target*: 0 bugs | *Confidence*: 0.8 | *Owner*: QA Lead
```

---

## Worked Example: Reforming Sandbagged Product OKRs

- **Problem**: Product team scored 100% on OKRs for 4 consecutive quarters, yet product adoption was stagnating.
- **Diagnosis**: Goals were sandbagged (e.g. "Publish 3 blog posts", "Attend 2 conferences").
- **Reform**: Replaced tasks with outcome metrics: "Increase self-serve trial-to-paid activation from 4.2% to 11.0%".
- **Outcome**: Team achieved 0.78 (8.6% conversion); trial conversion doubled, generating $340k in incremental revenue.

---

## Verification Checklist

- [ ] Objectives are qualitative, ambitious, and directional (no numbers or task lists).
- [ ] Every Key Result is strictly quantitative and follows the "From X to Y" formula.
- [ ] No more than 3–5 Key Results per Objective.
- [ ] OKRs are explicitly categorized as Committed (1.0 bar) or Aspirational (0.7 bar).
- [ ] OKR scoring is strictly decoupled from individual salary and bonus compensation.

---

## Anti-Patterns

- **Task Lists Masquerading as OKRs**: Writing "Ship v2.0" as a Key Result without measuring whether anyone uses it.
- **Sandbagging**: Setting trivial, easily achieved goals to look good in end-of-quarter reviews.
- **Set-and-Forget**: Writing OKRs on day 1 of the quarter and never looking at them again until day 90.

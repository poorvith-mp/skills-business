---
name: internal-reporting
last_reviewed: 2026-09-06
group: Reporting
description: >-
  Turn company data into dashboards and KPI tracking with a stated recommendation. Not channel
  performance. Use when building company KPI scorecards, department reviews, or updates.
---

# internal-reporting

## Core Philosophy
Internal operational reporting—weekly metric updates, departmental scorecards, and leadership dashboards—is frequently treated as a bureaucratic chore. Teams paste 40 disjointed graphs into an internal wiki that nobody reads until an emergency occurs. High-impact internal reporting is an operational steering engine: organizing company telemetry around an explicit North Star Metric hierarchy, tracking leading indicators, enforcing strict RAG (Red/Amber/Green) escalation thresholds, and pairing every metric with an actionable management recommendation.

---

## 4-Step Internal Operational Reporting Framework

### Step 1: North Star Metric & Departmental Metric Trees
1. **The Single North Star Metric (NSM)**:
   - Identify the single metric capturing core customer value delivery and long-term business health (e.g. *Weekly Active Workspaces with >= 5 Deploys*).
2. **The Metric Tree Hierarchy**:
   - *Level 1*: North Star Metric.
   - *Level 2 (Input Drivers)*:
     - Acquisition: Qualified Inbound Signups.
     - Activation: First Successful Deployment in $< 15text{ mins}$.
     - Retention: 30-day cohort active usage retention.
     - Monetization: Free-to-Paid conversion rate.

### Step 2: Leading vs Lagging Indicators
1. **Balancing the Scorecard**:
   - *Lagging Indicators (Historical Reality)*: Monthly Recurring Revenue (MRR), Gross Logo Churn, EBITDA. These metrics tell you what happened 30 days ago.
   - *Leading Indicators (Predictive Signals)*: Pricing page visits, API key creations, webhook volume drops, open P1 tickets. These metrics predict what revenue and churn will look like 60 days from now.

### Step 3: Red / Amber / Green (RAG) Exception Protocol
1. **Deterministic Status Definitions**:
   - **GREEN**: On track; within $\pm 5\%$ of quarterly target. No executive action required.
   - **AMBER**: At risk; lagging target by 6–15% or showing 2 consecutive weeks of negative velocity. Owner must deliver remediation plan.
   - **RED**: Critical failure; lagging target by $> 15\%$ or catastrophic incident. Requires immediate executive sponsor escalation and emergency resource reallocation.

### Step 4: The Decision-Oriented Delivery Format
1. **Never Present Data Without a Recommendation**:
   - A report is not a dump of raw numbers. If a metric is Red or Amber, the section must include:
     - Root-Cause Diagnostic (Why it missed).
     - Concrete Corrective Action (Who is doing what).
     - Expected Recovery Horizon (When metric returns to Green).

---

## Deliverable Format: Internal Executive KPI Dashboard (`INTERNAL-REPORT.md`)

```markdown
# Weekly Company Operations & KPI Report: Week of [YYYY-MM-DD]
*Distributed to Executive Leadership | Prepared by RevOps & FP&A*

## 1. North Star Metric Snapshot
- **North Star**: Weekly Active Productive Workspaces (WAPW)
- **Current Value**: **3,420** (+3.8% WoW | Target: 3,350) — **STATUS: GREEN**

## 2. Departmental KPI Scorecard
| Department | Core KPI | Current Value | Target | WoW Delta | Status |
|---|---|---|---|---|---|
| Engineering | Mean Time to Resolve P1 (MTTR) | 24 Minutes | < 30 Mins | -6 mins (Better) | **GREEN** |
| Product | Day-14 Activation Rate | 28.4% | 35.0% | -2.1% | **AMBER** |
| Sales | Qualified Outbound Demos | 14 Demos | 25 Demos | -44.0% | **RED** |
| Customer Success | Net Revenue Retention (NRR) | 114.5% | 110.0% | +0.4% | **GREEN** |

## 3. Red & Amber Variance Deep-Dive & Action Plans

### [RED] Outbound Sales Demo Shortfall
- **Diagnostic**: SDR outbound email deliverability dropped 30% due to DNS DKIM misconfiguration on secondary domain.
- **Corrective Action**: RevOps restored DKIM and warmed up 3 replacement domains; shifted SDR focus to LinkedIn social selling for next 7 days.
- **Recovery ETA**: Outbound demo velocity expected to return to Green by Sprint 16.

### [AMBER] Day-14 Product Activation Dip
- **Diagnostic**: Release of new onboarding modal introduced mobile browser UI clipping on Safari.
- **Corrective Action**: Frontend hotfix deployed Wednesday (PR #512); monitoring cohort recovery.
```

---

## Worked Example: Catching Churn Early via Leading Indicators

- **Incident**: Monthly revenue reports looked healthy (MRR flat), but internal leading indicator showed API webhook traffic had dropped 42% across 10 mid-market accounts.
- **Intervention**: Customer Success team reached out immediately; uncovered that a recent client API change broke client endpoints. CS assisted with the patch before clients decided to cancel.
- **Outcome**: Saved $140,000 in ARR that would have churned silently 60 days later.

---

## Verification Checklist

- [ ] Telemetry organized under a single clearly defined North Star Metric.
- [ ] Metrics balance leading predictive signals with lagging financial outcomes.
- [ ] RAG criteria (Green, Amber, Red) have mathematical threshold definitions.
- [ ] Every Amber or Red metric is accompanied by a concrete corrective action plan and recovery date.
- [ ] Distributed on a reliable, scheduled weekly cadence.

---

## Anti-Patterns

- **Metric Overload**: Dumping 80 graphs into a report until executives ignore the entire document.
- **Watermelon Reporting**: Marking metrics "Green" on the outside while underlying operational infrastructure is rotting "Red" on the inside.
- **Reporting Without Action**: Documenting that outbound sales missed target for 8 consecutive weeks without proposing a single change in strategy.

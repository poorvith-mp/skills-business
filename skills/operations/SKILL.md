---
name: operations
group: Operations
description: >-
  Own process, capacity planning, exception handling and performance tracking day to day. Use when
  running daily business operations, workflows, or SOP execution.
---

# operations

## Core Philosophy
Business operations is not keeping chaotic spreadsheets updated or firefighting emergencies as they occur. True operational excellence is systems engineering applied to human and technical workflows. High-performance operations is governed by queue theory, Little's Law, Eliyahu Goldratt’s Theory of Constraints, standardized capacity models, and automated exception routing. If a routine operational workflow depends on heroics or memory, the operating system has failed.

---

## 4-Step Scalable Business Operations Architecture

### Step 1: Bottleneck Identification & Theory of Constraints
1. **The Five Focusing Steps (Goldratt)**:
   - *1. Identify the Constraint*: Locate the single operational station or resource that limits total organizational throughput (e.g. security review queue).
   - *2. Exploit the Constraint*: Maximize output of that bottleneck (ensure the security team never wastes time on trivial administrative tasks).
   - *3. Subordinate Everything Else*: Align upstream workflows to feed the bottleneck at its optimal processing speed (never overwhelm the bottleneck).
   - *4. Elevate the Constraint*: Invest capital or headcount to expand bottleneck capacity.
   - *5. Repeat*: Once elevated, identify the new operational constraint.

### Step 2: Queue Theory & Little’s Law
1. **The Mathematical Law of Work-in-Progress (WIP)**:
   $$L = \lambda  imes W$$
   - Where:
     - $L$ = Average number of items in the system (WIP).
     - $\lambda$ = Throughput rate (items processed per day).
     - $W$ = Average lead time through the system.
   - *Operational Axiom*: To reduce cycle time ($W$), you must **reduce Work-in-Progress ($L$)**. Capping concurrent active projects cuts delivery lead time dramatically.

### Step 3: Capacity Planning & Utilization Thresholds
1. **The 80% Utilization Guardrail**:
   - In highway traffic and human operational teams alike, when utilization approaches 100%, queue wait times explode toward infinity.
   - Schedule operational teams for a **maximum of 80% baseline capacity**. Reserve the remaining 20% buffer for unexpected outages, emergencies, and continuous system improvement.

### Step 4: Standard Work Instructions & Exception Routing
1. **Standardized Operations Runbooks**:
   - Document deterministic operational routines in executable SOPs with explicit SLAs.
2. **Automated Exception Handling**:
   - Route standard transactions automatically; isolate exceptions and route directly to specialized human operators with full context logs.

---

## Deliverable Format: Operational System Specification (`OPERATIONS-SPEC.md`)

```markdown
# Operational Process & Capacity Specification: [Department / Workflow]

## 1. System Throughput & Capacity Baseline
- **Core Workflow**: Customer Technical Onboarding Pipeline
- **Current Throughput ($\lambda$)**: 12 enterprise accounts onboarded / month
- **Average Lead Time ($W$)**: 21 days from contract sign to live deployment
- **Active Work-in-Progress ($L$)**: 8 accounts concurrently active
- **Team Utilization**: 78% (Target: < 80% to prevent queue delay explosions)

## 2. Identified Bottleneck & Mitigation
- **Current Constraint**: Security VPC peering configuration
- **Exploitation Action**: Automated Terraform script generation to replace manual AWS peering requests, cutting bottleneck processing time from 4 days to 2 hours.

## 3. Escalation SLA & Exception Matrix
| Exception Trigger | SLA | Assigned Resolver | Escalation Path |
|---|---|---|---|
| Client webhook failure > 5% | < 2 Hours | Tier 2 Support Engineer | Lead Solutions Architect |
| Security questionnaire stall > 48h | < 24 Hours | Compliance Specialist | General Counsel |
| Onboarding milestone delayed > 5 days | Immediate | Dedicated Account Manager | VP of Operations |
```

---

## Worked Example: Slashing Client Onboarding Lead Time via Little's Law

- **Problem**: Client onboarding was dragging to 48 days; onboarding specialists managed 25 active clients simultaneously, feeling overwhelmed.
- **Intervention**: Applied Little's Law. Capped WIP to strictly 10 concurrent active accounts per specialist.
- **Outcome**: Average lead time dropped from 48 days to 14 days; client satisfaction jumped from 72% to 96%.

---

## Verification Checklist

- [ ] Primary operational constraint (bottleneck) identified and exploited.
- [ ] Work-in-Progress (WIP) limits enforced to reduce cycle times.
- [ ] Operational capacity planned with at least 20% reserve buffer.
- [ ] Standard work instructions documented with explicit SLAs.
- [ ] Automated exception routing prevents standard workflows from stalling.

---

## Anti-Patterns

- **Running Teams at 100% Utilization**: Ensuring every engineer or operator is 100% booked, guaranteeing that a single emergency causes system-wide cascading delays.
- **Local Optimization**: Spending $50,000 optimizing a non-bottleneck station, producing zero increase in overall system throughput.
- **Hero Culture**: Relying on specific individual employees working 16-hour days to keep broken processes running.

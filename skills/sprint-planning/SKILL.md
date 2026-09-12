---
name: sprint-planning
last_reviewed: 2026-09-06
group: Product and delivery
description: >-
  Prioritise features, allocate capacity and make the scope trade-offs explicit. Use when running
  agile ceremonies, story point sizing, or sprint backlogs.
---

# sprint-planning

## Core Philosophy
Sprint planning is not a ritualistic exercise in estimating imaginary story points or negotiating how many Jira tickets can be crammed into a two-week container. Sprint planning is the operational execution of the **Iron Triangle of Project Management** (Scope, Time, Resources). Fixed time (2 weeks) and fixed resources (team capacity) require variable, ruthlessly prioritized scope. High-performing engineering teams protect sprint commitments by budgeting for capacity realities, allocating explicit buffers for bugs and on-call, and making trade-offs explicit before work begins.

---

## 4-Step Rigorous Sprint Planning Framework

### Step 1: Capacity Planning & The 60-20-20 Rule
1. **Never Plan for 100% Feature Capacity**:
   - Software teams operating at 100% capacity inevitably fail sprint commitments due to unexpected production outages, sick leave, and code reviews.
2. **The 60-20-20 Capacity Budget**:
   - **60% Feature Epics**: Strategic roadmap deliverables that move company OKRs.
   - **20% Technical Debt & Bug Remediation**: Refactoring fragile code, updating dependencies, improving tests.
   - **20% Operational Buffer & On-Call**: Production alerts, code reviews, architectural discussions, meetings.
3. **Calculating True Developer Availability**:
   $$text{Sprint Hours} = (text{Working Days} - text{Holidays/PTO})  imes 6text{ Productive Hours/Day}$$

### Step 2: Backlog Refinement & Sizing Discipline
1. **Story Pointing (Fibonacci Sequence: 1, 2, 3, 5, 8)**:
   - Sizing measures **complexity, uncertainty, and effort**, not raw hours.
   - *The 8-Point Ceiling*: Any user story sized at **8 or higher is too large and ambiguous** for a single sprint. It must be broken down into smaller, testable sub-stories before entering the sprint.
2. **Definition of Ready (DoR)**:
   - A ticket cannot enter a sprint unless it has: Clear user story, technical architecture notes, unambiguous acceptance criteria (BDD/Gherkin), and designs attached.

### Step 3: Sprint Goal & Scope Commitment
1. **The Single Unifying Sprint Goal**:
   - Every sprint must have **one** overarching business objective that unifies the team:
     - Example: *"Enable enterprise users to successfully authenticate via Okta SAML SSO in staging."*
   - If a sprint has no goal, it is simply a random collection of disconnected chores.

### Step 4: Handling Mid-Sprint Interruptions
1. **The Scope Trade-Off Law**:
   - When leadership or sales requests an emergency mid-sprint feature addition:
     - Scope is never simply added on top of existing commitments.
     - **The Swap Principle**: *"We can pull in Feature X (5 points), provided we drop Feature Y (5 points) back into the backlog. Which is the higher business priority?"*

---

## Deliverable Format: Sprint Commitment Plan (`SPRINT-PLAN.md`)

```markdown
# Sprint Commitment Plan: Sprint [Sprint #]
*Duration: [YYYY-MM-DD to YYYY-MM-DD] (2 Weeks) | Sprint Lead: [Name]*

## 1. Sprint Goal
**Deliver production-ready OAuth2 refresh token rotation and session revocation across web and mobile.**

## 2. Capacity & Allocation Budget
- **Total Team Available Days**: 45 Dev Days (9 engineers x 5 days)
- **Committed Story Points**: **42 Points** (Historical rolling velocity: 44 points)
- **Allocation Breakdown**:
  - Feature Work (60%): 26 Points
  - Technical Debt & Maintenance (20%): 8 Points
  - Bug Fixes & Buffer (20%): 8 Points

## 3. Sprint Backlog & Priority Epics
| Issue ID | Summary | Story Points | Assignee | Priority |
|---|---|---|---|---|
| ENG-412 | Implement Redis token family revocation | 5 | @Dave | P0 (Goal) |
| ENG-415 | Wire client-side silent refresh interceptor | 3 | @Sarah | P0 (Goal) |
| ENG-420 | Fix PostgreSQL deadlock on customer export | 5 | @Elena | P1 (Tech Debt) |
| ENG-428 | Update Docker container base image to Alpine 3.20 | 2 | @Marcus | P2 (Chore) |

## 4. Definition of Done (DoD) Gate
- [ ] Automated tests pass in CI (`npm run test:all`).
- [ ] Code reviewed and approved by at least 1 peer engineer.
- [ ] Deployed and smoke-tested in staging environment.
- [ ] Documentation updated in `docs/api/`.
```

---

## Worked Example: Preventing Sprint Over-Commitment Failure

- **Context**: Team committed 65 story points in Sprint 12; completed only 38 points, leaving morale shattered.
- **Remediation**: In Sprint 13, applied the 60-20-20 capacity rule; calculated rolling 3-sprint velocity (40 points); capped backlog commitment at 38 points.
- **Outcome**: Team completed 100% of committed stories on time; delivered the core sprint goal with zero weekend overtime.

---

## Verification Checklist

- [ ] Clear, unifying Sprint Goal articulated and agreed upon by team.
- [ ] Team capacity accounts for holidays, PTO, and 20% operational buffer.
- [ ] No user story exceeds the 8-point complexity ceiling.
- [ ] Backlog stories satisfy the Definition of Ready (DoR).
- [ ] Mid-sprint scope additions enforce the reciprocal swap principle.

---

## Anti-Patterns

- **100% Feature Planning**: Planning zero capacity for bugs, code reviews, or production emergencies.
- **Sprint Goals with 12 Disjointed Bullet Points**: Having no cohesive focus for the two-week cycle.
- **Mid-Sprint Scope Ballooning**: Letting stakeholders dump 5 new urgent features into the active sprint without dropping existing tickets.

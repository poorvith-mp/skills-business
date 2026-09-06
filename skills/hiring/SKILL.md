---
name: hiring
group: People
description: >-
  Run it end to end: headcount planning, levelling, sourcing, assessment, offer and the first
  ninety days. Use when designing job descriptions, interview scorecards, or compensation.
---

# hiring

## Core Philosophy
Hiring is the single highest-leverage operational decision a company makes. Bad hires drain leadership time, demoralize high-performing teams, and burn immense capital in recruitment and severance costs. Great hiring is not relying on charismatic interviews, pedigree bias, or resume buzzwords. Professional technical hiring is a standardized, objective evaluation system: role leveling, structured interview scorecards, practical work-sample tests, and calibrated behavioral scoring.

---

## 4-Step Structured Hiring & Evaluation Framework

### Step 1: Role Definition, Leveling & Compensation Modeling
1. **The Role Blueprint**:
   - Define exact business outcomes expected in the first 90 days (e.g. "Ship the v2 database migration engine and mentor 2 junior engineers").
2. **Engineering Leveling Grid**:
   - *L3 (Software Engineer)*: Executes scoped tasks, writes clean tested code, learns codebase.
   - *L4 (Senior Engineer)*: Autonomously owns complex epics, drives architecture choices, debugs production outages.
   - *L5 / Staff Engineer*: Multi-team technical leadership, sets organization-wide technical standards, de-risks multi-quarter roadmaps.
3. **Compensation Banding**:
   - Benchmark against market databases (Option Impact, Pave, Levels.fyi): Base Salary, Equity Grants (BPS), and Target Performance Bonus.

### Step 2: Sourcing & The Anti-Bias Job Description
1. **Crafting the High-Signal Job Description**:
   - Lead with the technical mission and specific problems to be solved.
   - Cut generic corporate checklists ("Must have 8+ years experience in a dynamic fast-paced environment").
   - Replace with verifiable capabilities: *"Must have designed and deployed high-throughput distributed systems in Go or Rust in production."*

### Step 3: The Structured 4-Stage Interview Loop
1. **The Structured Assessment Architecture**:
   - *Stage 1: Recruiter / Hiring Manager Screen (30 Mins)*: Culture alignment, mutual expectations, communication clarity.
   - *Stage 2: Technical Work-Sample Test (60 Mins)*: Real-world practical coding or code review session (never whiteboard trivia or inverted binary trees). Give candidates a real bug in an isolated container and watch how they debug.
   - *Stage 3: System Design & Architecture (60 Mins)*: Interactive whiteboard design of a distributed system matching real company challenges.
   - *Stage 4: Behavioral & Culture Values (STAR Method - 45 Mins)*: Evaluate past behavior under stress, conflict resolution, and ownership mindset.

### Step 4: Objective Scorecards & The Offer Close
1. **Independent Scorecard Submission**:
   - Every interviewer must submit their written evaluation and binary rating (**Strong Hire / Hire / No Hire / Strong No Hire**) *before* talking to other interviewers to prevent groupthink.
2. **Closing the Top Candidate**:
   - Pitch the trajectory: Connect the candidate with the CEO/CTO for a final closing conversation. Walk through the equity model demonstrating potential financial upside.

---

## Deliverable Format: Structured Hiring Scorecard (`INTERVIEW-SCORECARD.md`)

```markdown
# Candidate Evaluation Scorecard: [Candidate Name]
*Role: Senior Systems Engineer (L4) | Interviewer: [Name, Title] | Stage: System Design*

## 1. Overall Recommendation
- **Verdict**: **[STRONG HIRE / HIRE / NO HIRE / STRONG NO HIRE]**
- **Confidence Score (1-5)**: [5 - High]

## 2. Core Competency Evaluations
| Competency | Score (1-5) | Evidence / Observed Behavior |
|---|---|---|
| Distributed Systems Architecture | 5/5 | Proactively identified database connection pool bottleneck; proposed Redis caching layer with TTL jitter. |
| Operational Reliability & Error Modes| 4/5 | Designed circuit-breaker failover; clearly articulated failure scenarios during AWS region outages. |
| Technical Communication | 5/5 | Explained complex trade-offs clearly; collaborated smoothly during requirements changes. |

## 3. Key Strengths & Growth Areas
- **Top Strength**: Exceptional understanding of PostgreSQL concurrency locking mechanisms.
- **Concern / Growth Area**: Less familiar with Kubernetes Helm charts; will require minor onboarding ramp.

## 4. Quantitative Decision
- **Recommend Moving to Offer**: **YES**. Candidate exceeds our L4 engineering bar.
```

---

## Worked Example: Eliminating Hiring Bias via Work-Sample Testing

- **Problem**: Engineering team suffered high failure rates from candidates who excelled at algorithmic LeetCode trivia but could not debug real production code.
- **Solution**: Replaced LeetCode tests with a 60-minute practical debugging session in a real GitHub repository containing a realistic race-condition bug.
- **Outcome**: 90-day new-hire performance ratings increased from 65% to 92%; turnover dropped to zero.

---

## Verification Checklist

- [ ] Role has documented leveling criteria and market compensation bands.
- [ ] Job description specifies tangible 90-day deliverables over arbitrary years of experience.
- [ ] Technical assessment evaluates realistic work samples (debugging, code review, system design).
- [ ] Behavioral interviews use structured STAR questions.
- [ ] Interviewers submit independent scorecards prior to debrief discussions.

---

## Anti-Patterns

- **LeetCode Brain Teasers**: Asking candidates to invert binary trees on a whiteboard for a role that writes standard CRUD APIs.
- **Unstructured "Gut-Check" Chats**: Making hiring decisions based on whether the interviewer would "like to have a beer with them".
- **Hiring Under Panic**: Lowering the hiring bar during high-pressure sprints, inheriting months of technical debt and team friction.

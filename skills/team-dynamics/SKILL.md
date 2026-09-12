---
name: team-dynamics
last_reviewed: 2026-09-06
group: People
description: >-
  Diagnose motivation, conflict, structure and the cross-cultural blind spots nobody names out
  loud. Use when resolving co-founder friction, team conflict, or trust issues.
---

# team-dynamics

## Core Philosophy
High-performing engineering and executive teams do not collapse because of technical deficiencies. They collapse because of unaddressed interpersonal friction, avoidance of difficult conflict, toxic passive-aggression, and structural ambiguity. Team dynamics is not touchy-feely team-building games or superficial happy hours. Building high-leverage team dynamics is an organizational discipline based on **Patrick Lencioni's 5 Dysfunctions of a Team** and Amy Edmondson’s psychological safety research—establishing radical candor, transparent accountability, and healthy ideological conflict.

---

## 4-Step Team Dynamics & Conflict Resolution Framework

### Step 1: Psychological Safety & The Vulnerability Foundation
1. **The Foundation of Psychological Safety (Amy Edmondson)**:
   - Team members must feel confident that they will not be punished, humiliated, or marginalized for speaking up with ideas, questions, concerns, or mistakes.
2. **Leader Vulnerability Modeling**:
   - Leaders must publicly admit when they make mistakes:
     - *"I made the wrong architectural call on that database migration. Here is what I learned, and here is how we are fixing it."*
   - Vulnerability from leadership unlocks psychological safety across the team.

### Step 2: Patrick Lencioni's 5 Dysfunctions Audit
1. **The Pyramidal Diagnostic**:
   - *1. Absence of Trust*: Unwilling to be vulnerable about weaknesses and mistakes.
   - *2. Fear of Conflict*: Preserving artificial harmony while venting frustration privately in backchannels.
   - *3. Lack of Commitment*: Feigning agreement in meetings, then passive-aggressively dragging execution.
   - *4. Avoidance of Accountability*: Hesitant to hold peers accountable for missed deadlines or sub-par standards.
   - *5. Inattention to Results*: Prioritizing personal ego, status, or career over collective team victory.

### Step 3: Cultivating Healthy Ideological Conflict (Disagree and Commit)
1. **Artificial Harmony vs Productive Conflict**:
   - When a team never argues about technical architecture, they are not aligned—they are disengaged.
   - Separate **Cognitive Conflict** (debating ideas, data, technical trade-offs) from **Affective Conflict** (personal attacks, ego, politics).
2. **The "Disagree and Commit" Principle**:
   - Everyone must vigorously debate their perspective before the decision is made.
   - Once the decision owner decides, debate ends immediately. Every team member commits 100% of their energy to making the decision a success, with zero second-guessing or "I told you so" sabotage.

### Step 4: Resolving Co-Founder & Leadership Friction
1. **The Structured Neutral Mediation Protocol**:
   - When co-founder or executive friction threatens the organization:
     - 1. **Deconstruct Role Overlap**: Friction usually stems from ambiguous role boundaries (e.g. CEO and CTO both trying to manage product roadmap). Establish strict operational swimlanes.
     - 2. **Separate Facts from Inferences**: Force each party to state observable facts vs internal assumptions.
     - 3. **Draft a Binding Working Agreement**: Document decision authority, communication protocols, and escalation rules.

---

## Deliverable Format: Team Health & Working Agreement Spec (`TEAM-HEALTH.md`)

```markdown
# Team Dynamics Diagnostic & Working Agreement: [Team / Squad Name]

## 1. Lencioni 5-Dysfunctions Diagnostic Audit
- **Team Trust Score (1-5)**: 4/5 (Healthy vulnerability observed in retrospectives)
- **Constructive Conflict (1-5)**: 2/5 (Warning: Team shows artificial harmony; hesitant to debate tech choices)
- **Accountability (1-5)**: 3/5 (Relies on manager to call out missed deadlines rather than peer-to-peer)

## 2. Team Working Agreements (The Social Contract)
1. **Radical Candor in Reviews**:
   - We critique code and architecture vigorously; we never critique individual character.
2. **No Backchannel Venting**:
   - If you have an issue with a teammate's decision, you address it directly with them within 24 hours. Private Slack complaints to third parties are prohibited.
3. **Disagree and Commit**:
   - Once an architectural RFC is approved, all engineers execute with full commitment.
4. **Meeting Presence**:
   - Zero multitasking or laptops during sprint planning and retrospective discussions.

## 3. Co-Founder / Executive Swimlanes
- **Co-Founder A (CEO)**: 100% final decision authority on GTM, Hiring, Pricing, Fundraising.
- **Co-Founder B (CTO)**: 100% final decision authority on Architecture, Infrastructure, Tech Stack.
```

---

## Worked Example: Healing Co-Founder Gridlock

- **Situation**: Technical CEO and CTO were engaged in passive-aggressive conflict, paralyzing the sprint roadmap for 3 months.
- **Mediation**: Neutral facilitator ran a role clarity audit. Discovered both were attempting to act as the primary product manager.
- **Resolution**: Codified explicit swimlanes: CEO owned customer problem definition and market validation; CTO owned technical architecture and engineering delivery.
- **Outcome**: Roadblock dissolved; product shipping velocity doubled in the subsequent quarter.

---

## Verification Checklist

- [ ] Team assessed against Lencioni's 5 Dysfunctions framework.
- [ ] Explicit working agreements established and signed off by all team members.
- [ ] Role boundaries and decision-making authority (swimlanes) clearly separated.
- [ ] Disagree-and-commit discipline practiced on major architectural decisions.
- [ ] Constructive ideological conflict is encouraged and distinguished from personal attacks.

---

## Anti-Patterns

- **Artificial Harmony**: Smiling in meetings while privately complaining to colleagues in private Slack channels.
- **The Dictator CEO**: Demanding total consensus while privately overruling every decision, destroying psychological safety.
- **Ignoring Toxic High-Performers**: Tolerating an abusive, brilliant engineer who destroys the morale of 10 other teammates.

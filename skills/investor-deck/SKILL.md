---
name: investor-deck
last_reviewed: 2026-09-06
group: Fundraising and board
description: Build the raise narrative: problem-solution, TAM/SAM/SOM, traction and model. For full pro formas, see business-plan. Use when structuring seed, Series A, or venture pitch decks.
---

# investor-deck

## Core Philosophy
A venture capital pitch deck is not a product user manual, nor is it a comprehensive operational plan. A pitch deck is a 12-slide narrative sales document designed to do exactly one thing: **secure a partner meeting**. Great pitch decks construct an airtight logical progression: highlighting an undeniable macroeconomic market shift, illustrating an acute customer pain, showcasing a defensible solution, and proving exponential commercial traction.

---

## 4-Step Venture Pitch Deck Architecture (The 12-Slide Canon)

### Step 1: Narrative Progression & Emotional Arc
1. **The 12-Slide Canonical Sequence**:
   - **Slide 1: Title & Value Hook**: 1-sentence declarative statement of what you do.
   - **Slide 2: The Urgent Problem**: The acute, quantified bleeding experienced by enterprise buyers.
   - **Slide 3: The Broken Status Quo**: Why current legacy solutions and workarounds fail.
   - **Slide 4: The "Why Now?"**: The external catalyst (regulatory, technological, architectural shift) that makes this possible today.
   - **Slide 5: The Solution & Product**: Concrete UI/architecture demonstration of the product in action.
   - **Slide 6: Market Sizing (TAM/SAM/SOM)**: Bottom-up market calculation demonstrating a path to $100M+ ARR.
   - **Slide 7: Traction & Velocity**: The single most impressive graph (ARR growth, active users, net retention).
   - **Slide 8: Business Model & Unit Economics**: Pricing tiers, ACV, Gross Margins ($\ge 80\%$), CAC Payback.
   - **Slide 9: Competitive Moat & Counter-Positioning**: Why competitors cannot easily replicate the value.
   - **Slide 10: Go-to-Market Engine**: How you acquire customers efficiently at scale.
   - **Slide 11: Team Pedigree**: Why this specific founding team has unfair domain insight.
   - **Slide 12: The Ask & Milestones**: Capital requested and the exact milestones it unlocks.

### Step 2: Visual Discipline & Cognitive Load
1. **The 3-Second Slide Rule**:
   - An investor should understand the core takeaway of any slide within 3 seconds of scanning.
   - Use declarative slide titles that state the conclusion, not the topic:
     - *Bad Title*: "Market Size"
     - *Good Title*: "A $4.2B Market Created by the Shift to Cloud Infrastructure"
2. **Zero Dense Text Paragraphs**:
   - Maximum 20 words of text per slide. Replace text with bold metrics, diagrams, and clean UI screenshots.

### Step 3: Bottom-Up Market Sizing & Financial Realism
1. **Bottom-Up Math Only**:
   - Show the multiplication: `(60,000 ICP accounts) x ($24,000 ACV) = $1.44B TAM`.
   - Never use arbitrary top-down percentages of broad industries.

### Step 4: The Traction Slide: Show the "T2D3" Curve
1. **Demonstrating Venture Velocity**:
   - Investors look for evidence of the **T2D3** trajectory (Triple, Triple, Double, Double, Double ARR growth).
   - If pre-revenue, showcase technical velocity: weekly active GitHub contributors, pilot letters of intent (LOIs), or enterprise waitlist growth.

---

## Deliverable Format: Venture Pitch Deck Storyboard (`PITCH-DECK.md`)

```markdown
# 12-Slide Venture Pitch Deck Storyboard: [Company Name]
*Target Raise: $2.0M Seed | Focus: Enterprise Developer Tools*

## Slide 1: Title & Vision
- **Header**: [Company Name]
- **Subtitle**: Automated, zero-downtime database migrations for high-throughput Postgres.
- **Visual**: High-contrast mockup of CLI terminal running zero-downtime schema migration.

## Slide 2: The Problem (Quantified Bleed)
- **Header**: Database Outages Cost Enterprise Tech $120k Per Incident
- **Bullet Points**:
  - DDL operations lock production tables during high traffic.
  - 68% of engineering teams experience deployment delays due to database fears.
- **Visual**: Excerpt of real post-mortem incident report showing database lock downtime.

## Slide 3: The Solution
- **Header**: Instant, Ephemeral Database Emulation in Local Docker
- **Visual**: Split-screen showing automatic detection of blocking locks before PR merge.

## Slide 6: Market Size (Bottom-Up)
- **Header**: A $2.1B Addressable Market Across Cloud-Native Tech
- **Math**: 70,000 mid-market engineering orgs x $30,000 annual contract = $2.1B TAM.

## Slide 7: Traction (The Core Proof)
- **Header**: $42k MRR Growing 22% MoM Across 120 Engineering Teams
- **Visual**: Up-and-to-the-right ARR bar chart with 118% Net Revenue Retention callout.

## Slide 12: The Ask & Milestones
- **Header**: Raising $2.0M Seed to Scale Enterprise GTM and Reach $2M ARR
- **Milestone 1**: Expand engineering team from 3 to 7 FTEs.
- **Milestone 2**: Reach 400 paying enterprise teams in 18 months.
```

---

## Worked Example: Turning a 30-Slide Deck into a Seed Winner

- **Original**: 32 slides filled with dense technical explanations of database internals; investors tuned out after slide 5.
- **Overhaul**: Condensed to the 12-slide canonical narrative. Changed slide titles to declarative statements; highlighted a single graph showing 22% MoM revenue growth.
- **Outcome**: Pitched 14 venture firms; received 3 term sheets within 12 days.

---

## Verification Checklist

- [ ] Exactly 12 slides following the canonical narrative sequence.
- [ ] Every slide title is a declarative conclusion sentence (not a generic topic label).
- [ ] Market sizing uses bottom-up math (Accounts $ imes$ ACV).
- [ ] Traction slide prominently displays MoM growth and retention metrics.
- [ ] Slides contain minimal text ($< 25$ words) with large, readable typography.

---

## Anti-Patterns

- **The Product Manual**: Spending 8 slides explaining every technical dropdown in the software settings.
- **Top-Down Sizing Hand-Waving**: Claiming "Software is a $1 Trillion industry and if we get 0.1% we are a unicorn".
- **Hiding the Traction**: Placing your revenue and user growth numbers on slide 28 where investors never see it.

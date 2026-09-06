---
name: business-plan
group: Strategy
description: Build the plan: market analysis, value proposition, and revenue model. For pitch decks, see investor-deck. Use when drafting formal business plans, executive summaries, or pro formas.
---

# business-plan

## Core Philosophy
A business plan is not an academic 50-page theoretical treatise written to sit in a drawer. An institutional-grade business plan is an operational and financial blueprint. It proves that a market opportunity exists, that your solution has a defensible competitive moat, that customer acquisition unit economics are mathematically profitable, and that capital will be converted into enterprise enterprise valuation through disciplined milestone execution.

---

## 4-Step Bank- & Venture-Grade Business Plan Architecture

### Step 1: Executive Summary & Value Proposition
1. **The Core Business Thesis**:
   - Who is the customer? What acute commercial pain do they suffer? How does your proprietary solution solve it 10x better, faster, or cheaper than the status quo?
2. **Business Model & Unit Economics Snapshot**:
   - Pricing architecture, Gross Margins, Average Contract Value (ACV), Target Customer Acquisition Cost (CAC), and Lifetime Value (LTV).

### Step 2: Market Sizing & Competitive Moat (7 Powers)
1. **Bottom-Up Market Sizing (TAM / SAM / SOM)**:
   - Never use top-down hand-waving: *"If we capture 1% of China's $500B market..."*
   - Calculate strictly bottom-up:
     $$text{TAM} = (text{Total Addressable Accounts Globally})  imes (text{Realistic Annual Contract Value ACV})$$
     $$text{SAM} = text{Subset of TAM fitting core ICP technographic filters}$$
     $$text{SOM} = text{Target obtainable market in next 24–36 months}$$
2. **Moat Architecture (Hamilton Helmer's 7 Powers)**:
   - Explicitly identify which power defends your gross margins: *Switching Costs, Network Effects, Counter-Positioning, Scale Economies, Cornered Resource, Brand, or Process Power*.

### Step 3: Go-to-Market (GTM) & Operational Engine
1. **Customer Acquisition Channels & Funnel Mechanics**:
   - Detailed channel economics: Inbound SEO / Content, Outbound Enterprise SDR, Product-Led Growth (PLG), or Channel VARs.
2. **Organizational Headcount Scaling Plan**:
   - Hiring roadmap mapped to revenue milestones (e.g. Engineer #4 hired at $50k MRR; VP of Sales hired at $1M ARR).

### Step 4: 3-Statement Pro Forma Financial Model (3–5 Years)
1. **Integrated Pro Forma Statements**:
   - *Income Statement (P&L)*: Revenue, Cost of Goods Sold (COGS), Gross Profit, Operating Expenses (R&D, S&M, G&A), EBITDA.
   - *Cash Flow Statement*: Operating cash flow, burn rate, minimum cash trough.
   - *Key Ratios*: Gross Margin ($\ge 75\%$), CAC Payback Period ($< 12text{ mos}$), LTV/CAC ($\ge 3:1$).

---

## Deliverable Format: Comprehensive Business Plan (`BUSINESS-PLAN.md`)

```markdown
# Comprehensive Business Plan: [Company Name]

## 1. Executive Summary & Problem-Solution
- **Problem**: Enterprise engineering teams spend 40% of sprint capacity managing fragile Kubernetes infrastructure, costing $120k/year in wasted senior dev time.
- **Solution**: Ephemeral internal developer platform that provisions isolated staging environments in 10 seconds.
- **Core Business Model**: Tiered B2B SaaS ($50/developer/month + usage compute).

## 2. Market Sizing (Bottom-Up Analysis)
- **TAM**: 45,000 mid-market software companies x $36,000 ACV = **$1.62 Billion**
- **SAM**: 12,000 US/EU tech companies running Kubernetes on AWS = **$432 Million**
- **SOM (36 Months)**: 350 enterprise customers = **$12.6 Million ARR**

## 3. Competitive Moats & Defensive Strategy
- **Switching Costs**: Deep integration into developer CI/CD workflows and automated secrets stores creates massive organizational inertia against replacement.
- **Counter-Positioning**: Incumbent enterprise vendors rely on heavy professional services consulting contracts; our self-serve CLI deploys in 4 minutes.

## 4. 3-Year Pro Forma Financial Summary
| Metric | Year 1 | Year 2 | Year 3 |
|---|---|---|---|
| Ending ARR | $480,000 | $2,100,000 | $6,400,000 |
| Gross Margin % | 78% | 82% | 84% |
| Headcount | 6 FTEs | 14 FTEs | 32 FTEs |
| Net Monthly Burn (Avg)| -$42,000 | -$65,000 | +$12,000 (Cash flow positive)|
| Required Capital | $800,000 Seed | $3,000,000 Series A | Self-sustaining |
```

---

## Worked Example: Securing $1.5M Seed Round via Bottom-Up Business Plan

- **Strategy**: Replaced a vague top-down 40-page market report with a crisp 12-page bottom-up business plan mapping verified developer survey data to unit economics.
- **Outcome**: Closed a $1.5M Seed financing round from lead institutional venture fund in 3 weeks.

---

## Verification Checklist

- [ ] Market sizing calculated bottom-up using verifiable account numbers and ACVs.
- [ ] Competitive moat explicitly identified using Helmer's 7 Powers framework.
- [ ] GTM strategy details CAC, payback period, and primary acquisition channel.
- [ ] Financial pro forma includes integrated P&L, burn rate, and gross margin projections.
- [ ] Headcount hiring schedule is tied directly to revenue milestone triggers.

---

## Anti-Patterns

- **The 1% of a Giant Market Myth**: Claiming your TAM is $500 Billion without defining the specific addressable ICP.
- **Hockey Stick Without Costs**: Projecting revenue to jump from $100k to $10M with flat operational expenses.
- **No Competitive Moat**: Assuming nobody else will build your feature once you demonstrate market demand.

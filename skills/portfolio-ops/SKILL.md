---
name: portfolio-ops
group: Operations
description: >-
  Allocate resources and sequence work across several projects competing for the same people. Use
  when orchestrating multiple business units, ventures, or shared ops.
---

# portfolio-ops

## Core Philosophy
Managing a multi-product portfolio, holding company, or studio of competing technical ventures is fundamentally different from running a single startup. Portfolio operations is capital and talent allocation across competing priorities. The primary failure mode of multi-project organizations is spreading key technical talent so thin across 6 initiatives that all 6 stall. High-leverage portfolio operations enforces strict capital tiering, clear kill criteria, and shared infrastructural platform services.

---

## 4-Step Multi-Venture Portfolio Operations Architecture

### Step 1: Strategic Portfolio Segmentation & Capital Tiering
1. **The 3-Bucket Portfolio Allocation**:
   - *Core Engine (Cash Cows - 60% Resources)*: Profitable, proven product lines generating predictable cash flow. Focus on margin defense, retention, and operational efficiency.
   - *Growth Bets (Scale-Ups - 30% Resources)*: High-conviction products with verified product-market fit scaling toward profitability. Focus on market capture and feature expansion.
   - *Venture Labs / Spikes (Frontier R&D - 10% Resources)*: High-uncertainty experimental throwaway prototypes exploring novel capabilities. Time-boxed and budget-capped.

### Step 2: Resource Contention & The Critical Path Method (CPM)
1. **The Zero-Fractional-Engineer Rule**:
   - Never assign a senior engineer to 3 different portfolio projects simultaneously (context-switching destroys 40% of cognitive productivity).
   - Core engineers are assigned **100% dedicated** to a single project per quarter.
2. **Critical Path Dependency Mapping**:
   - Map shared infrastructural dependencies across the portfolio (e.g. Shared Auth, Payment rails, Compliance certifications). Prevent one project's delay from bottlenecking the entire portfolio.

### Step 3: Centralized Shared Services (Platform Ops)
1. **Shared Platform Infrastructure**:
   - Centralize operational overhead into high-leverage shared internal services:
     - Legal & Compliance (Corporate entity management, trademarking, customer contracts).
     - Finance & Accounting (Centralized payroll, billing engines, tax optimization).
     - Core Infrastructure & Cloud (Consolidated AWS enterprise discount agreements, centralized Datadog monitoring).
2. **Internal Service Level Agreements (SLAs)**:
   - Shared services must operate with clear internal SLAs to prevent becoming bureaucratic roadblocks for autonomous venture teams.

### Step 4: Objective Kill Criteria & Milestone Governance
1. **The Capital Gate Milestone**:
   - Every experimental venture receives capital in tranches tied to binary milestone achievements (e.g. "$100k allocated to reach 500 active weekly developers in 90 days").
2. **The Rational Cull**:
   - If a venture misses its milestone gate, ruthlessly kill it or archive it. Reallocate engineering talent to the fastest-growing growth bet.

---

## Deliverable Format: Portfolio Resource & Allocation Matrix (`PORTFOLIO-OPS.md`)

```markdown
# Portfolio Operations & Capital Allocation Plan: [Holding Co / Studio Name]
*Review Period: Q3-Q4 | Portfolio Director: [Name, Title]*

## 1. Portfolio Asset Tiering & Resource Distribution
| Venture / Product Name | Tier Classification | Target ARR | Headcount Allocation | Quarterly Budget |
|---|---|---|---|---|
| Project Titan (Flagship)| Core Engine (Cash Cow)| $4,200,000 | 12 Dedicated FTEs | $450,000 |
| Project Pulse (Analytics)| Growth Bet | $850,000 | 6 Dedicated FTEs | $220,000 |
| Project Nova (AI Agent) | Frontier Lab Spike | $0 | 2 Dedicated FTEs | $60,000 (Capped) |

## 2. Milestone Gates & Kill Criteria
- **Project Nova (Lab Spike)**:
  - *Target Gate*: Acquire 1,000 active CLI installs and 20 paying beta accounts by [Date].
  - *Kill Criteria*: If paid accounts < 5 by [Date], project is terminated and code archived. Engineers return to Project Titan.

## 3. Shared Services SLA Matrix
- **Legal Review (Customer MSAs)**: Turnaround <= 48 hours for deals > $25k.
- **Cloud Infrastructure Provisioning**: Ephemeral staging environments deployed in <= 15 minutes.
```

---

## Worked Example: Rescuing an Over-Extended Tech Studio

- **Problem**: Studio was building 7 products simultaneously with 14 engineers. Every product missed delivery deadlines; zero products reached profitability.
- **Intervention**: Killed 4 stagnant products immediately; consolidated all 14 engineers onto the top 2 products with proven customer traction.
- **Outcome**: The flagship product reached $2M ARR within 9 months; overall studio turned cash-flow positive.

---

## Verification Checklist

- [ ] Portfolio segmented into Core Engines, Growth Bets, and Frontier Labs.
- [ ] Core technical talent assigned 100% dedicated to a single venture (no fractional engineers).
- [ ] Shared services (Legal, Cloud, Finance) operate under documented internal SLAs.
- [ ] Every experimental venture has explicit, binary kill criteria and budget caps.
- [ ] Quarterly portfolio review reallocates capital and talent from laggards to winners.

---

## Anti-Patterns

- **The Zombie Portfolio**: Continuing to fund 5 dead projects for years because "someone worked hard on it".
- **Fractional Staffing Chaos**: Assigning 1 principal engineer to 4 projects, ensuring nothing ships on time.
- **Subsidy Traps**: Forcing a profitable cash-cow product to subsidize poorly conceived pet projects indefinitely.

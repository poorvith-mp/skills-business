---
name: market-trends
last_reviewed: 2026-09-06
group: Strategy
description: >-
  Identify where a market is heading and size the opportunity, with sourced evidence rather than
  vibes. Use when analyzing industry reports, market shifts, or macro trends.
---

# market-trends

## Core Philosophy
Analyzing market trends is not summarizing Twitter/X hot takes, reading generic blog posts, or falling for ephemeral hype cycles. Professional market intelligence is an empirical, quantitative discipline. It requires triangulating primary industry data, auditing regulatory filings (SEC 10-K reports), tracking developer adoption telemetry, analyzing patent filing trajectories, and understanding technological S-curves. Rigorous trend analysis separates permanent tectonic industry shifts from temporary speculative bubbles.

---

## 4-Step Empirical Market Intelligence Framework

### Step 1: Macro Forces & PESTLE Deconstruction
1. **The 6 Structural Drivers (PESTLE)**:
   - *Political / Geopolitical*: Trade tariffs, supply chain on-shoring, export controls (e.g. GPU chip embargoes).
   - *Economic*: Interest rate cycles, enterprise IT budget contraction/expansion, venture capital deployment velocity.
   - *Social / Demographic*: Aging workforces, remote work geographic dispersion, developer generational preferences.
   - *Technological*: Fundamental capability shifts (e.g. local LLM inference, WebAssembly runtimes).
   - *Legal / Regulatory*: Statutory compliance mandates (EU AI Act, CSRD, SEC climate disclosure rules).
   - *Environmental*: Energy grid constraints, data center power density limitations.

### Step 2: The S-Curve & Hype Cycle Calibration
1. **The Technology S-Curve**:
   - *Inflection Point*: When a new technology shifts from slow experimental R&D into exponential real-world adoption.
   - *Gartner Hype Cycle Phase*: Determine if the trend is at the *Peak of Inflated Expectations*, the *Trough of Disillusionment*, or the *Slope of Enlightenment*.
2. **The "Lasting Shift vs Passing Fad" Filter**:
   - Ask: *"Does this technology reduce unit costs by 10x or eliminate a fundamental human friction?"* If yes, it is an enduring structural shift. If it only creates speculative novelty, it is a passing bubble.

### Step 3: Primary Data Triangulation (Zero Vibes)
1. **Verifiable Data Sources**:
   - *SEC 10-K & Earnings Calls*: Search transcript keyword frequency across publicly traded enterprises (e.g. mentions of "cloud repatriation" or "AI capex").
   - *Developer & Open-Source Telemetry*: GitHub star velocity, PyPI/npm download trajectories, Stack Overflow Developer Survey data.
   - *Patent & Trademark Filings*: USPTO / WIPO filings indicating where Big Tech is allocating multi-year R&D capital.

### Step 4: Opportunity Sizing & Strategic Implications
1. **Translating Trends into Enterprise Action**:
   - What new category does this trend create?
   - What legacy incumbents will this trend render obsolete in 36 months?
   - What is the specific product wedge that captures this shift?

---

## Deliverable Format: Market Intelligence Report (`MARKET-TRENDS.md`)

```markdown
# Strategic Market Trend Intelligence: [Trend Title]
*Date: [YYYY-MM-DD] | Focus: Enterprise Cloud Infrastructure & AI Compute*

## 1. Executive Thesis & The Structural Shift
- **Core Trend**: Enterprise migration toward specialized, private on-premise AI inference clusters driven by cloud GPU token costs and data sovereignty.
- **Horizon**: 24–48 Month Expansion Window
- **Confidence Rating**: High (Backed by primary hardware telemetry and CapEx data)

## 2. Quantitative Evidence & Triangulation
| Data Source | Metric / Observation | Historical Baseline | Trend Signal |
|---|---|---|---|
| Enterprise SEC 10-Ks | Mentions of "Private Cloud AI" | 12 mentions (2024) | 148 mentions (2026) (+1,130%) |
| Open-Source Telemetry | Ollama & vLLM GitHub Stars | 8k stars | 92k stars combined |
| Hardware Lead Times | Enterprise H100/B200 order wait | 42 Weeks | 8 Weeks (Supply normalizing) |

## 3. Disruption & Incumbent Vulnerability
- **Vulnerable Status Quo**: Hyperscaler multi-tenant API token wrappers charging 300% markup on inference.
- **Emerging Winners**: Local orchestration engines, quantization compilers, and private bare-metal GPU hosts.

## 4. Strategic Recommendations for Leadership
1. Build local-first inference capabilities into v3 enterprise product.
2. Develop VPC-isolated on-premise container deployment option.
```

---

## Worked Example: Predicting the Microservice Repatriation Trend

- **Analysis**: Triangulated AWS data egress charges, cloud monitoring bills, and engineer survey sentiment in 2024.
- **Finding**: Identified that companies spending $> $100text{k/month}$ on AWS were actively consolidating microservices back into modular monoliths to slash latency and network costs.
- **Strategic Pivot**: Developer tool shifted marketing from "Microservice Mesh Manager" to "Modular Monolith Performance Engine", driving a 3x surge in enterprise inbound leads.

---

## Verification Checklist

- [ ] Trend thesis is supported by at least 3 distinct primary data sources (SEC filings, telemetry, patents).
- [ ] Technology adoption is plotted on the S-Curve and Hype Cycle.
- [ ] Analysis identifies both the emerging market winners and vulnerable incumbents.
- [ ] PESTLE drivers are evaluated for legal, technological, and economic headwinds.
- [ ] Actionable strategic recommendations are provided for leadership.

---

## Anti-Patterns

- **Vibe-Based Forecasting**: Declaring a trend exists because 5 influencers on Twitter/X posted about it.
- **Confusing Hype with Adoption**: Assuming high media coverage equals commercial paying customer adoption.
- **Ignoring Physics and Capital**: Forecasting exponential data center growth while ignoring municipal power grid limits.

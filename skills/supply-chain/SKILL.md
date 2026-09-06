---
name: supply-chain
group: Operations
description: >-
  Plan strategic sourcing, supplier development, quality control and logistics. Use when managing
  physical inventory, manufacturing lead times, or logistics.
---

# supply-chain

## Core Philosophy
Physical hardware, electronic component, and product supply chains are governed by global lead times, manufacturing yields, tariffs, geopolitical bottlenecks, and inventory carrying costs. A software bug can be patched in minutes; a missing $0.05 microcontroller stops a $5,000,000 automated assembly line for 6 months. Managing high-reliability supply chains requires rigorous Bill of Materials (BOM) hygiene, Total Cost of Ownership (TCO) modeling, multi-source supplier risk mitigation, and scientific safety stock calculations.

---

## 4-Step Strategic Supply Chain & Hardware Logistics Framework

### Step 1: Bill of Materials (BOM) & Lifecycle Sourcing
1. **The Indented Engineering BOM (eBOM -> mBOM)**:
   - Map every physical component down to primary manufacturer part numbers (MPN), approved alternate sources, and lifecycle status:
     - *Active*: In volume mass production.
     - *Not Recommended for New Designs (NRND)*: Flagged for phase-out.
     - *End of Life (EOL)*: Must identify replacement drop-in equivalents immediately.
2. **Single-Source Risk Elimination**:
   - Every mission-critical component (ASIC, sensor, battery, PCB substrate) must have at least **two qualified, production-tested suppliers** (Dual-Sourcing Strategy).

### Step 2: Total Cost of Ownership (TCO) & Landed Cost Modeling
1. **The Landed Cost Formula**:
   - Never evaluate suppliers solely on unit purchase price (FOB factory gate). Calculate true Landed Cost:
     $$text{Landed Cost} = text{Unit Ex-Works Price} + text{Ocean/Air Freight} + text{Customs Tariffs} + text{Insurance} + text{Scrap Rate} + text{Inventory Carrying Cost}$$
2. **Incoterms 2020 Standardization**:
   - Define exact legal transfer of risk and freight liability:
     - *EXW (Ex Works)*: Buyer assumes 100% of transport risk and customs from factory floor.
     - *FOB (Free on Board)*: Seller handles local transport to port; buyer assumes ocean freight risk.
     - *DDP (Delivered Duty Paid)*: Seller covers all shipping, insurance, and import duties to buyer’s warehouse.

### Step 3: Scientific Inventory Control & Safety Stock
1. **Economic Order Quantity (EOQ)**:
   $$EOQ = \sqrt{rac{2  imes D  imes S}{H}}$$
   - Where $D$ = Annual Demand, $S$ = Order Setup Cost, $H$ = Annual Holding Cost per unit.
2. **Safety Stock Formula (Demand & Lead Time Variability)**:
   $$text{Safety Stock} = Z  imes \sqrt{L  imes \sigma_D^2 + D^2  imes \sigma_L^2}$$
   - Where $Z$ = Service level factor (e.g. $1.65$ for 95% fill rate), $L$ = Lead time, $\sigma_D$ = Demand variance, $\sigma_L$ = Lead time variance.

### Step 4: Quality Assurance & Factory Audits (AQL Standard)
1. **Acceptance Quality Limit (ISO 2859 / ANSI/ASQ Z1.4)**:
   - Enforce standard AQL sampling on factory shipments:
     - *Critical Defects (Safety/Fire Hazard)*: 0% tolerance (AQL 0).
     - *Major Defects (Device inoperable)*: AQL 1.0 or 1.5.
     - *Minor Defects (Cosmetic scratch)*: AQL 4.0.

---

## Deliverable Format: Supply Chain Architecture & Sourcing Spec (`SUPPLY-CHAIN-SPEC.md`)

```markdown
# Strategic Sourcing & Supply Chain Specification: [Hardware Product]

## 1. Indented Bill of Materials (BOM) Risk Matrix
| Subsystem | Component Name | Primary MPN | Alternate MPN | Lifecycle Status | Lead Time | Single Source Risk |
|---|---|---|---|---|---|---|
| Compute | Main MCU 32-bit | STM32F405 | GD32F405 | Active | 14 Weeks | Low (Dual-sourced) |
| Power | Buck Converter | TPS62130 | RT6253 | Active | 8 Weeks | Low (Footprint compatible)|
| Enclosure | Anodized Aluminum Shell | Custom CNC | Local Sheetmetal | Custom Tooling | 6 Weeks | Medium (1 tooling set) |

## 2. Landed Unit Economics Model
- **Ex-Works Factory Cost**: $42.50
- **Ocean Freight + Logistics**: $3.20 / unit
- **Import Tariffs (Harmonized Code 8471)**: $4.25 (10%)
- **Warehousing & Carrying Cost**: $1.80 / unit
- **Total Landed Unit Cost**: **$51.75** (Target retail MSRP: $199.00 | Gross Margin: 74%)

## 3. Inventory Reorder & Safety Buffer
- **Target Customer Fill Rate**: 98% ($Z = 2.05$)
- **Required Safety Stock**: 1,200 units in central 3PL warehouse
- **Reorder Point**: Trigger production run when inventory drops to 2,800 units.
```

---

## Worked Example: Navigating Semiconductor Component Allocations

- **Crisis**: Primary microcontroller lead time exploded from 12 weeks to 52 weeks during global chip shortage.
- **Execution**: Hardware team had pre-qualified a pin-compatible alternative microcontroller in the original eBOM design.
- **Outcome**: Swapped parts on the SMT assembly line without a board redesign; preserved 100% on-time customer delivery while competitors halted production for 9 months.

---

## Verification Checklist

- [ ] All critical electrical and mechanical components have verified second sources.
- [ ] Landed cost calculated including tariffs, freight, insurance, and inventory carrying cost.
- [ ] Safety stock mathematically derived from demand and lead time variances.
- [ ] Incoterms explicitly defined on all international purchase orders.
- [ ] Factory quality inspections enforce standard AQL sampling criteria.

---

## Anti-Patterns

- **Single-Source Complacency**: Relying on a single specialized component vendor with zero alternate footprint on the PCB.
- **FOB Price Myopia**: Choosing a factory 2% cheaper on purchase price whose freight and tariffs make it 15% more expensive landed.
- **Ignoring EOL Notices**: Ignoring component manufacturer end-of-life notices until production stops.

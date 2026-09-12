---
name: vendor-selection
last_reviewed: 2026-09-06
group: Operations
description: >-
  Run RFI/RFP, scoring matrices, contract negotiation and vendor performance tracking. Use when
  evaluating RFP proposals, scoring vendors, or procurement.
---

# Vendor Selection

Vendor decisions are usually made on price alone by default, but price is only one of several factors that determine whether a vendor relationship actually works out — get the evaluation criteria right before comparing quotes, or the comparison itself will mislead.

## Workflow

1. **Define evaluation criteria before soliciting or comparing proposals.** A reasonable default weighting to adapt: price/total cost of ownership, quality/reliability track record, delivery/SLA terms, contract flexibility (exit clauses, scaling terms), and vendor financial stability (a cheap vendor that goes under mid-contract creates far more cost than it saved). Ask which matter most for this specific decision rather than assuming price dominates.
2. **Structure the RFP around outcomes, not just specs** — describe what the business needs to achieve, and let vendors propose how, rather than over-specifying a solution that might not be the best approach. Over-specified RFPs tend to just get the incumbent's existing approach re-quoted.
3. **Build a comparison scorecard**, not just a price table — score each vendor against the weighted criteria from step 1, so the comparison reflects total value, not just headline cost.
4. **Identify negotiation leverage before the conversation, not during it:**
   - Multiple qualified alternatives (real leverage, only if the alternatives are genuinely viable, not just for show)
   - Contract timing (end of vendor's fiscal quarter/year often creates urgency on their side)
   - Volume/commitment length (longer terms or higher volume in exchange for better pricing)
   - Reference/case-study value (a notable client name can be leverage in the other direction — the vendor wants you as a reference)
5. **For renewals specifically**, don't assume the incumbent's renewal price is fair just because switching has friction — check current market rates, and use switching cost as a negotiating fact, not a reason to skip negotiating.

## Anti-Patterns & Constraints

- Don't recommend selecting purely on lowest price without surfacing the tradeoffs on quality, reliability, and contract terms — that's a legitimate choice, but it should be a conscious one, not a default.
- Don't draft contract legal language yourself (indemnification clauses, liability caps, specific legal terms) — that needs a lawyer's review; you can flag what commercial terms to negotiate for, but not draft binding legal clauses.

## Output format

```markdown
## Vendor evaluation: <category>

**Criteria & weights:**
| Criterion | Weight | Notes |

**Vendor comparison:**
| Vendor | Price | [criterion 2] | [criterion 3] | Weighted score |

**Negotiation leverage available:** [specific to this situation]

**Recommendation:** [with reasoning tied to the weighted criteria, not just price]
```

## Verification & Quality Checklist

- [ ] Each step has a named owner, not a team-shaped placeholder.
- [ ] Inputs and outputs defined for every step, including their format.
- [ ] Failure and escalation path defined for the steps that can block.
- [ ] Completion is measurable - someone can tell whether it is done.

# Customer Onboarding Trial Handoff Checklist

Package: [[../../Generated-Packages/Vertical Agent Template Kit/README|Vertical Agent Template Kit]]
Related packet: [[Customer Onboarding Trial Packet]]
Related role card: [[Non-Release Role Card Evidence - Customer Onboarding Agent]]
Status: ready for next real onboarding trial; no validation proof has been claimed.

## Purpose

Make the next real customer-onboarding trial executable in one pass by turning the prepared packet into a preflight → run → review → decision handoff.

## 1. Preflight before the trial

- [ ] Name the customer/onboarding scenario or use a private alias if sensitive.
- [ ] Attach the source context that triggered onboarding work.
- [ ] Pick the exact workflow boundary: `intake`, `handoff draft`, `checklist generation`, or `follow-up summary`.
- [ ] Confirm which artifacts will be filled during the run:
  - [ ] [[Customer Onboarding Trial Packet]]
  - [ ] [[Non-Release Role Card Evidence - Customer Onboarding Agent]]
- [ ] Identify one human reviewer and the review standard before running the agent.

## 2. Trial capture fields

| Field | Fill during real trial |
| --- | --- |
| Source context link |  |
| Workflow boundary |  |
| Agent role card version |  |
| Inputs provided |  |
| Generated output location |  |
| Human reviewer |  |
| Review notes |  |
| Safety/quality issue observed |  |
| Reuse potential |  |

## 3. Decision gate

Choose exactly one after review:

- [ ] **Promote** — output passed review, workflow is repeatable, and the role card can be reused without major edits.
- [ ] **Pilot-only** — useful for this customer/workflow, but not enough evidence for a general template.
- [ ] **Iterate** — promising, but a role boundary, input, guardrail, or review criterion must change.
- [ ] **Retire** — too bespoke, unsafe, or low-leverage for a vertical-agent template.

Decision rationale:

> 

## 4. Follow-up update checklist

- [ ] Update [[Customer Onboarding Trial Packet]] with source-backed evidence.
- [ ] Update [[Non-Release Role Card Evidence - Customer Onboarding Agent]] with the actual role-card result.
- [ ] Add one sentence to [[../Generated-Packages/Vertical Agent Template Kit/README|package changelog]] summarizing the decision, not just the activity.
- [ ] Update [[../Improvement-Loops/Vertical Agent Template Kit Loop|improvement loop]] `next_focus` based on the selected gate.
- [ ] If promoted, revisit the skill draft; if not, keep it as a draft and record why.

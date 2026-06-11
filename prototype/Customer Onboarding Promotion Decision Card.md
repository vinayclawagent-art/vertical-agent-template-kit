# Customer Onboarding Promotion Decision Card

Status: decision-card ready; no validation proof recorded yet.

Use after `Customer Onboarding Operator Trial Packet.md` is filled from a real onboarding workflow. Do not complete from memory.

## Trial identity

| Field | Fill |
|---|---|
| Customer / segment | |
| Workflow date | |
| Operator | |
| Human reviewer | |
| Source request / issue / CRM link | |
| Filled operator packet | |
| Generated role card / output | |
| Review notes / objections | |

## Evidence checklist

- [ ] Trial packet contains source context, input artifacts, generated output, human review notes, and follow-up decision.
- [ ] Every claim links to a source artifact: CRM note, issue, transcript, diff, screenshot, packet section, reviewer note, or repo commit.
- [ ] Guardrails held: no customer-visible action without human review; no fabricated customer context; no hidden scope expansion.
- [ ] Reuse value is visible in at least one concrete next action, handoff, or saved role-card edit.

## Decision gate

Choose exactly one outcome.

| Outcome | When to choose | Evidence required | Next patch |
|---|---|---|---|
| Promote template format | The onboarding run reused the vertical-agent template with low friction and reviewer approval. | Filled packet + reviewer signoff + at least one role-card improvement. | Patch README, skill draft, and package backlog with source-backed proof. |
| Pilot-only | Useful for onboarding but too narrow for a general skill. | Filled packet + specific customer/onboarding constraints. | Keep as package artifact; add one more pilot task. |
| Iterate card | The structure helped but missed key fields, guardrails, or handoff steps. | Filled packet + reviewer objections + proposed field changes. | Patch role-template-card and builder fields. |
| Retire / hold | The template added process drag or produced weak output. | Filled packet + reviewer rationale. | Mark skill draft as not promoted; capture failure lesson. |

Selected outcome: `Promote template format / Pilot-only / Iterate card / Retire-hold`

Decision rationale:

> 

## Patch queue after decision

- [ ] Update `prototype/README.md` with the source-backed result.
- [ ] Update package README backlog and changelog.
- [ ] Patch the skill draft only if the promote or pilot-only outcome has evidence.
- [ ] Add a filled example note only when the packet links to real artifacts.
- [ ] Update the improvement loop `next_focus` to the next evidence-backed step.

## Guardrail

Prepared for the next real trial only. This card is not validation proof until the fields above cite real artifacts.

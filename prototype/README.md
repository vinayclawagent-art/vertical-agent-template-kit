# Vertical Agent Template Kit Prototype

Source: [[Codex Role Plugins as Vertical Agent Templates]]

## What it demonstrates
A compact kit for turning a reusable role workflow into a vertical agent template with inputs, boundaries, review criteria, and launch wedge.

## How to use
Open `role-template-card.md` and fill it against one concrete project/workflow.
For a faster browser flow, open `vertical-template-builder.html`; it saves inputs locally and generates a copyable role card with trigger, evidence, guardrails, handoff steps, and promotion gate.

## Worked example

- [[Worked Example - Mission Control Release QA Agent]] — fills the role-template card for a release QA vertical agent, including inputs, allowed tools, out-of-bounds actions, human review gate, and launch wedge.
- [[Release QA Scorecard Checklist]] — copyable 30-point release QA checklist/rubric for turning the worked example into an evidence-backed live run.
- `vertical-template-builder.html` — interactive local-first builder for creating new vertical agent template cards without editing markdown by hand.
- [[Non-Release Role Card Evidence - Customer Onboarding Agent]] — a prepared non-release vertical-agent card with explicit evidence requirements before it can be treated as validated.
- [[Customer Onboarding Trial Packet]] — a single ordered packet for the next real onboarding trial that sequences source context, generated outputs, review notes, and the promote / pilot-only / iterate / retire decision without claiming proof early.
- [[Customer Onboarding Trial Handoff Checklist]] — preflight, capture, decision, and follow-up checklist that makes the next live onboarding trial executable without claiming validation before it happens.

## Next iteration ideas
- Add scoring rubric. ✅ Done with [[Release QA Scorecard Checklist]].
- Add an HTML checklist view. ✅ Done with `vertical-template-builder.html`.
- Link one completed example back into the package note. ✅ Done with the Mission Control release QA example.
- Archive one non-release role card from the interactive builder. ✅ Prepared via [[Non-Release Role Card Evidence - Customer Onboarding Agent]]; still needs a real customer-onboarding trial before promotion.
- Bundle the non-release role card into a canonical live-trial packet. ✅ Prepared via [[Customer Onboarding Trial Packet]]; fill it during the next real onboarding workflow.
- Add an operator handoff checklist for the trial packet. ✅ Prepared via [[Customer Onboarding Trial Handoff Checklist]]; use it immediately before/during the next real onboarding workflow.

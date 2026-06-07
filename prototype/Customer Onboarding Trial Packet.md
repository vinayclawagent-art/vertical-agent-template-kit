# Customer Onboarding Trial Packet

Source package: [[../../Generated-Packages/Vertical Agent Template Kit/README|Vertical Agent Template Kit]]
Loop: [[../../Improvement-Loops/Vertical Agent Template Kit Loop|Vertical Agent Template Kit Loop]]
Prepared: 2026-06-07
Status: packet ready; no live onboarding proof has been invented

## When to use

Use this packet when a real customer onboarding workflow is available and the Customer Onboarding Prep Agent role card is ready to be tested against actual source context.

## Ordered packet steps

| Step | Artifact / action | Fill during live run | Minimum proof |
|---|---|---|---|
| 1 | Open `vertical-template-builder.html` or the existing [[Non-Release Role Card Evidence - Customer Onboarding Agent]] | Confirm agent name, trigger, allowed actions, and out-of-bounds constraints still match the real customer | Link to source context and owner |
| 2 | Fill the evidence checklist in [[Non-Release Role Card Evidence - Customer Onboarding Agent]] | Attach onboarding brief, review notes, corrected assumptions, and reuse decision | At least one generated output and one human review note |
| 3 | Compare output to the review gate | Record whether customer-facing language, timeline, and risk severity needed edits | Explicit pass / needs-iteration decision |
| 4 | Update the package and loop | Add only completed proof and the resulting next focus | Changelog line with source-backed evidence |
| 5 | Decide promotion path | Promote, keep as pilot-only, or retire the preset | Rationale tied to observed reuse |

## Trial fields

- Real customer / pilot: _TBD during live run_
- Source context links: _TBD during live run_
- Human owner: _TBD during live run_
- Generated artifacts attached: _TBD during live run_
- Assumptions removed or corrected: _TBD during live run_
- Reuse decision: _TBD during live run_

## Minimum evidence checklist

- [ ] Source context is linked and accessible.
- [ ] Generated onboarding brief or kickoff agenda is attached.
- [ ] Human review notes are attached.
- [ ] At least one incorrect or risky assumption was checked explicitly, even if none were found.
- [ ] Reuse decision is recorded as `promote`, `pilot-only`, `iterate`, or `retire`.

## Copyable handoff block

```markdown
### Customer Onboarding Prep Agent trial
- Customer / pilot: 
- Source context: 
- Output attached: 
- Human reviewer: 
- Assumptions corrected: 
- Decision: promote / pilot-only / iterate / retire
- Next action: 
```

## Copyable changelog line

Paste this only after the real trial is complete:

```markdown
- 2026-__: Filled [[../Prototypes/Vertical Agent Template Kit/Customer Onboarding Trial Packet|Customer Onboarding Trial Packet]] against a real onboarding workflow and recorded the reuse decision without fabricating evidence.
```

## Next action

Run this packet during the next real onboarding trial. The packet is ready, but the role card is not validated until real source context, generated output, and human review notes are attached.

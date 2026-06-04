# Worked Example - Mission Control Release QA Agent

Package: [[../../Generated-Packages/Vertical Agent Template Kit/README|Vertical Agent Template Kit]]
Source template: [[role-template-card]]

## Role wedge

**Role:** Mission Control release QA agent  
**Buyer/user:** Vinay or an engineering lead preparing a Hermes/Mission Control release  
**Promise:** Turn a messy pre-release branch into a reviewed, evidence-backed release candidate without handing the agent broad, vague authority.

## Template card

| Field | Filled example |
|---|---|
| Role-specific job | Audit a release branch for regression risk, docs drift, and missing verification evidence. |
| Inputs | PR/branch URL, changelog draft, modified file list, latest test output, known risk notes. |
| Allowed tools | Git diff/status/log, read/search files, targeted tests, docs validation, GitHub comments or checklist updates. |
| Out-of-bounds | No production deploys, no credential edits, no scheduler/cron changes, no speculative rewrites outside changed surface. |
| Required output | Release readiness score, blocking issues, non-blocking follow-ups, exact commands run, evidence links. |
| Human review gate | Human approves before merge/deploy; agent may only mark readiness and propose fixes. |

## Vertical packaging choices

- **Starter artifact:** `release-qa-card.md` template plus a checklist section in the release PR.
- **Reusable memory:** Keep a small catalog of recurring release failure modes: stale docs, unverified migrations, broad permission changes, and missing rollback notes.
- **Launch wedge:** Start with Hermes/Mission Control release branches, then generalize to any VinClawLabs repo after 2 clean runs.

## Done condition

The vertical template is ready for one live trial when it can answer all five questions without extra prompting:

1. What branch or PR is being released?
2. What changed since the previous release?
3. What evidence proves the critical path still works?
4. What risks need a human decision?
5. What exact next action should the human take?

## Follow-up backlog

- Convert this worked example into a copyable `release-qa-card.md` starter.
- Add a lightweight score rubric: environment realism, diff coverage, evidence quality, rollback clarity, and human-gate safety.
- If reused twice, fold the pattern into the `vertical-agent-template-kit` skill draft instead of promoting a duplicate skill.

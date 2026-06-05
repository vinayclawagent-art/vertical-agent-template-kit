# Release QA Scorecard Checklist

Package: [[../../Generated-Packages/Vertical Agent Template Kit/README|Vertical Agent Template Kit]]
Worked example: [[Worked Example - Mission Control Release QA Agent]]

Use this copyable scorecard when a Mission Control / Hermes release branch needs a narrow, role-specific QA agent instead of an open-ended coding agent.

## Copyable release QA scorecard

```markdown
# Release QA Agent Scorecard

Branch/PR: <link>
Release owner: <name>
Target release: <version/date>
Agent run: <Hermes/Codex/Claude session link or note>

| Dimension | Score 0-5 | Evidence required | Notes |
|---|---:|---|---|
| Diff coverage |  | Changed files, risky modules, migrations/config touched |  |
| Test realism |  | Exact commands, environment, fixtures, skipped tests |  |
| Critical-path proof |  | Screenshots, logs, CLI output, smoke-test notes |  |
| Docs/changelog alignment |  | Updated docs, release notes, operator-facing changes |  |
| Rollback clarity |  | Rollback command, feature flag, migration reversal, owner |  |
| Human-gate safety |  | Explicit merge/deploy approval step and unresolved decisions |  |

Total: __ / 30
Readiness band: Green 25-30 / Yellow 18-24 / Red <18

## Blocking issues
- [ ] <issue, file/path, reproduction, owner>

## Non-blocking follow-ups
- [ ] <follow-up, why it can wait, owner/date>

## Exact commands run
- `<command>` → `<result / log link>`

## Human decision required
Decision: <merge / defer / run more tests / ship behind flag>
Reason: <one paragraph>
```

## Rubric

| Score | Meaning |
|---:|---|
| 0 | Not checked or no evidence. |
| 1 | Mentioned, but evidence is missing or speculative. |
| 2 | Light evidence; narrow happy path only. |
| 3 | Adequate evidence for normal release risk. |
| 4 | Strong evidence across changed surface and likely regressions. |
| 5 | Strong evidence plus clear rollback/handoff for operators. |

## Done condition

The QA agent may mark the release **ready for human approval** only when:

- Total score is **25+**.
- No blocking issues remain open.
- Every command/result is copied into the release note or PR checklist.
- Rollback owner and rollback path are explicit.
- Human approval is still required before merge/deploy.

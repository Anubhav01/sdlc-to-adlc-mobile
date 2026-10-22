# Appendices

## A. Agent task spec template
```
Title:
Goal (user outcome):
Scope / Non-goals:
Acceptance criteria (testable):
Edge cases and worst cases:
Constraints (platform, min OS, design system, privacy):
Dependencies (APIs, flags, analytics):
Out-of-bounds files/areas:
Definition of done (tests, PR, review):
```

## B. PR review checklist (human or agent)
- Matches the spec and acceptance criteria
- Tests cover edge cases, not only the happy path
- No secrets, no new risky permissions or dependencies
- Handles offline, permission denial, backgrounding
- Accessibility and large text considered
- Small, single-purpose change

## C. Sample ADLC pipeline
Intent, clarify, spec, plan approval, build plus tests per subtask, self-correct, PR, agent review, human review, merge, CI, beta, staged rollout, monitoring, triage, back to intent.

## D. Glossary
- **Agent**: software that pursues a goal using tools in a loop.
- **ADLC**: Agentic Development Lifecycle.
- **CI/CD**: automated build, test, and delivery.
- **Feature flag**: a switch to enable or disable a feature without a new release.
- **Kill switch**: a flag used to turn off a broken feature quickly.
- **Staged rollout**: releasing to a growing percentage of users.
- **Prompt injection**: hidden instructions in content that steer an agent.
- **Spec**: the written, testable description of what to build.

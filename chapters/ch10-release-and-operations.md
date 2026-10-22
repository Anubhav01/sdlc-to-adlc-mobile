# Chapter 10: Release and Operations

## Where mobile ADLC must go beyond the PR
Merging is not shipping. Mobile adds build signing, store submission, review, and staged rollout.

## The release pipeline
CI builds and tests, then signed build, internal testers, beta (TestFlight / Play testing tracks), store submission, staged rollout, monitoring.

## Where agents help
- Drafting release notes and store metadata from merged PRs.
- Checking submission requirements and privacy declarations against the code.
- Triage of crash reports: group, find likely cause, propose a fix PR.
- Watching rollout metrics (crash-free rate, ANRs, key flows) and recommending pause or continue.

## Where humans must stay
Release approval, rollback decisions, anything touching signing keys, and policy or legal declarations.

## Staged rollouts and kill switches
Release to a small percentage, watch metrics, then expand. Feature flags and remote config let you disable a broken feature without a new store release.

## The self-healing loop (and its limits)
Crash detected, agent proposes a fix, tests pass, human approves, hotfix. Full auto-deploy without a human gate is risky on mobile because you cannot easily recall a build.

## Doubt Box
- **Can an agent submit to the store?** Technically possible with automation; keep a human approval before submit.
- **What if a bad build already shipped?** Use kill switches, pause rollout, and ship a fix.
- **Which metrics matter?** Crash-free users/sessions, startup time, key-flow success, ratings.

## Try it
Write a one-page rollout plan: percentages, metrics, and the pause trigger.

# Chapter 8: Agentic Coding

## The working loop
Plan, implement a subtask, write tests alongside, run them, fix failures, repeat until green, open a PR.

## Context is everything
Agents only know what they can see. Give them:
- The spec for this task.
- Project rules (architecture, naming, banned patterns) in an instructions file the tool reads.
- Relevant code locations, not the whole repo.

## Guardrails
- Limit what agents may change (no touching signing keys, release config, or payment logic without review).
- Never put secrets in prompts or code.
- Run in branches, never directly on the main branch.
- Cap the number of fix attempts, then escalate to a human.

## Small PRs per subtask
One subtask, one PR, one clear purpose. Small changes are reviewable, revertible, and easier for agents to get right.

## Agent-as-reviewer
Use an agent for a first review pass: bugs, style, missing tests, security smells. Prefer a different tool or model than the one that wrote the code; same-source review shares blind spots. A human still approves.

## Case study: the review loop
Raise PR, agent review, comments, agent fixes and updates PR, request merge approval, maintainer re-reviews, merge, CI/CD.

## Doubt Box
- **How do I know the agent isn't looping forever?** Set limits on attempts and time.
- **Should I read all generated code?** Yes, with attention proportional to risk.
- **Why do agents over-engineer?** They try to be thorough. Say "minimal change" in the spec.

## Try it
Add a rule file to a project and watch how agent output changes.

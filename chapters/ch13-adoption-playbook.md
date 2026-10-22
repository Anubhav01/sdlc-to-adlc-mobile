# Chapter 13: Adoption Playbook

## Migrate in stages, not in one jump

**Stage 0: Baseline.** Measure today's cycle time, defect rate, and review wait.

**Stage 1: Assisted.** Autocomplete and chat for everyone. Set policies on approved tools and data.

**Stage 2: Agent on low-risk work.** Unit tests, refactors, documentation, boilerplate. Easy to verify, low blast radius.

**Stage 3: Agent on features with checkpoints.** Clarify-first, plan approval, small PRs, agent plus human review.

**Stage 4: Agent in operations.** Crash triage, release notes, rollout monitoring, with human gates.

**Stage 5: Multi-agent workflows.** Specialized agents with orchestrated handoffs.

## Making it stick
- Shared instruction files and spec templates in the repo.
- A short team agreement: what agents may do, what needs approval.
- Weekly review of what worked and failed; update the instructions.
- Train reviewers: reviewing agent code is a skill.

## Common failure modes
Skipping specs, rubber-stamp reviews, giant PRs, no metrics, tool sprawl, and ignoring security.

## Doubt Box
- **Where do I start tomorrow?** Pick one low-risk task type and run it with clarify-first and small PRs.
- **How long does adoption take?** Weeks for habits, months for reliable workflows.
- **What if the team resists?** Start with volunteers, show measured results.

## Try it
Place your team on the stage ladder and choose the next rung.

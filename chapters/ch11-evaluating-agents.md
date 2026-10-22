# Chapter 11: Evaluating Agents

## Why measure
Without measurement, "the agent feels faster" is a guess. Evaluate to decide where to trust agents more or less.

## What to measure
- **Quality**: defects found after merge, review comments per PR, test failures after agent-claimed completion.
- **Speed**: time from spec to merged PR, review turnaround.
- **Cost**: tokens or subscription cost per merged PR.
- **Reliability**: how often the agent finishes without human rescue.
- **Trust signals**: how often reviewers accept agent output unchanged.

## Compare fairly
Compare similar tasks, include human review time in the agent cost, and track rework, not just first-draft speed.

## Build a small eval set
Keep 10 to 20 representative tasks from your project. Re-run them when you change tools, models, or instructions and compare results.

## Watch for
Over-trust (reviewers rubber-stamping), hidden costs (review time rising), and quality drift after tool or model updates.

## Doubt Box
- **Is lines of code a good metric?** No. More code is not more value.
- **How do I compare Cursor vs Codex vs Copilot?** Run the same eval tasks through each and compare quality, rework, and cost.
- **How often should I re-evaluate?** After any major tool or model change.

## Try it
Pick five past tasks and score agent output on quality, rework, and time.

# Chapter 3: From Tools to Agents

## Three levels of AI in development
1. **Autocomplete and chat (assistants).** You type, it suggests. You stay in control of every step.
2. **Agents.** You give a goal; it plans, edits files, runs commands and tests, and iterates. You supervise.
3. **Multi-agent systems.** Several agents with roles (planner, coder, tester, reviewer) coordinate on one goal.

## Copilot vs agent
A copilot suggests, and you do. An agent acts toward a goal across steps, and you check the result.

## What makes something an agent
- A **goal** rather than a single prompt.
- **Tools**: file editing, terminal, browser, test runners.
- A **loop**: act, observe the result, adjust.
- **Memory/context**: the repo, the spec, earlier steps.

## The tools you may already use
Editor agents (Cursor, Copilot agent mode), CLI/cloud agents (Codex), and agent-first environments (Antigravity). They differ in interface and autonomy, but share the loop above. Features change quickly, so check each tool's current documentation.

## Doubt Box
- **Do these tools share memory?** Usually not. Each needs the same spec, which is why Chapter 6 treats specs as the source of truth.
- **Is more autonomy always better?** No. Match autonomy to risk: high for tests and boilerplate, low for payments, auth, and data deletion.
- **Can an agent be wrong confidently?** Yes. That is why verification (Chapter 9) matters.

## Try it
Take one task and run it twice: as chat help, then as an agent goal. Compare time and review effort.

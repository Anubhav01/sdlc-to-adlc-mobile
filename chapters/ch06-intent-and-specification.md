# Chapter 6: Intent and Specification

## Why specs matter more with agents
A human teammate fills gaps with common sense and questions. An agent fills gaps with guesses. The spec is the cheapest place to prevent wrong code.

## What a good agent-ready spec contains
1. **Goal**: the user outcome, in one or two sentences.
2. **Scope and non-goals**: what is explicitly not included.
3. **Acceptance criteria**: testable statements ("When offline, the cart still opens and shows cached items").
4. **Edge cases and worst cases**: empty states, slow network, permission denied, low storage, interrupted flows, old OS versions.
5. **Constraints**: platforms, minimum OS, design system, performance and privacy rules.
6. **Dependencies**: APIs, feature flags, analytics events.

## The clarify-first habit
Ask the agent: "Before writing code, list every question you need answered and every edge case you see." Answer them, then freeze the result as the spec. This is the single highest-value ADLC habit.

## Mobile-specific spec questions
- What happens on permission denial or revocation mid-flow?
- Offline and flaky network behavior?
- Backgrounding, process death, and state restoration?
- Accessibility (screen readers, dynamic text size)?
- Behavior on the oldest supported OS?

## Keeping one spec across several tools
If you use multiple agents, keep the spec in the repo (for example a `specs/` folder) so every tool reads the same source.

## Doubt Box
- **How detailed should a spec be?** Detailed on behavior and edge cases, silent on implementation unless a constraint requires it.
- **Isn't this just the old requirements doc?** Similar, but it must be testable and unambiguous because the reader cannot ask hallway questions.
- **Can the agent write the spec?** It can draft it from your answers; you approve it.

## Try it
Take a vague ticket and run the clarify-first prompt. Count how many questions surface.

# Chapter 2: Where the SDLC Strains

Chapter 1 showed the lifecycle. This chapter shows where it hurts, because those pain points are exactly where agents get applied.

## The five pressure points in mobile
1. **Slow feedback loops.** Build, sign, upload, store review, rollout: days between a change and real user data.
2. **Device and OS fragmentation.** A feature that works on your phone can crash on a three-year-old budget device.
3. **Testing cost.** Real devices are expensive; manual regression grows with every release.
4. **Rising complexity.** Two platforms (or one cross-platform framework), backend APIs, analytics, permissions, accessibility, localization.
5. **Coordination overhead.** Requirements, designs, tickets, and code drift apart. Reviews queue up.

## Where developer time actually goes
Writing new code is often a minority of the week. The rest is understanding old code, waiting on reviews and CI, reproducing bugs, writing boilerplate and tests, and chasing unclear requirements.

## Why this matters for ADLC
Agents are good at the repetitive, well-defined parts: boilerplate, tests, first-pass reviews, triage. They are weak where context is missing, which is why unclear requirements hurt agents even more than humans.

## Doubt Box
- **Is the problem that developers are slow?** No. Most delay is waiting and rework, not typing.
- **Will agents fix fragmentation?** Not by themselves. They can generate and run more tests, but you still need real device coverage.
- **Which pain should I tackle first?** Start where work is repetitive and the result is easy to verify, such as unit tests.

## Try it
List your top three time sinks last month. Mark which are repetitive and verifiable.

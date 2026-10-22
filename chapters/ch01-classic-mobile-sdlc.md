# Chapter 1: The Classic Mobile SDLC

## What is SDLC?
The Software Development Life Cycle is the journey software takes from idea to retirement. Like building a house: decide what you need, draw plans, build, inspect, move in, keep repairing.

Six stages:
1. **Plan**: what are we building and why?
2. **Design**: how will it look and work?
3. **Build**: write the code.
4. **Test**: does it work, and what breaks it?
5. **Release**: put it in users' hands.
6. **Maintain**: fix, improve, repeat.

## How teams organize the stages
- **Waterfall**: finish each stage fully before the next. Predictable, but painful when requirements change.
- **Agile (Scrum, Kanban)**: repeat all stages in short cycles of one to two weeks. Most mobile teams work this way.
- **CI/CD**: automation that builds, tests, and ships code on every change.

## Why mobile is different from web
On the web, a bug fix reaches everyone in minutes. On mobile:
- **Store review** sits between you and users.
- **Users control updates**, so several versions live at once.
- **Fragmentation**: many devices, OS versions, and screen sizes, especially on Android.
- **Hard to undo**: you cannot recall a bad build from phones. Teams use kill switches and feature flags.
- **Device realities**: battery, weak networks, offline use, permissions.

Result: heavy testing before release and staged rollouts (1%, then 10%, then everyone).

## Case study: a real agent-driven workflow
A developer using Cursor, Codex, Copilot, and Antigravity works like this: share requirement, agent asks clarifying questions, discuss edge cases and worst cases, plan development and testing, build subtask by subtask with parallel unit tests, loop until tests pass, one PR per subtask, agent reviews the PR, fix comments, human maintainer approves and merges, CI/CD runs. This is already ADLC in practice. Chapter 4 names the pattern.

## Doubt Box
- **Is Agile a replacement for SDLC?** No. SDLC is the set of stages; Agile runs them in small loops.
- **Is CI/CD the same as DevOps?** No. DevOps is a culture; CI/CD is one of its main practices.
- **Why can't mobile auto-update like websites?** The app lives on the user's phone, and the store and user control updates.

## Try it
Draw your last feature's journey from idea to production. Mark every place you waited.

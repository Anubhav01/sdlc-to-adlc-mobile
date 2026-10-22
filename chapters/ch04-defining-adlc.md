# Chapter 4: Defining ADLC

## Definition
The **Agentic Development Lifecycle (ADLC)** is a way of building software where agents own well-defined tasks end to end, and humans decide at checkpoints. It is not SDLC plus a chatbot; the unit of work, feedback loops, and artifacts change.

## SDLC vs ADLC
| | SDLC | ADLC |
|---|---|---|
| Who does the work | Humans, helped by tools | Agents, supervised by humans |
| Human role | Doer | Specifier, reviewer, decider |
| Unit of work | Ticket / story | Spec'd, verifiable subtask |
| Feedback | After build, test, release | Inside the loop, continuously |
| Key artifact | Code | Spec, tests, and agent logs, plus code |

## Seven principles
1. **Clarify before coding.** Agents ask; humans answer.
2. **Spec is the source of truth.**
3. **Plan, then execute.**
4. **Small, verifiable units** (one subtask, one PR).
5. **Independent verification**: tests and reviews not written by the same blind spot.
6. **Human gates at decisions**: plan approval, merge approval, release approval.
7. **Everything is traceable**: what the agent did and why.

## The ADLC loop
Intent, clarify, plan, build with tests, self-correct, review, human gate, ship, observe, back to intent.

## Case study
The workflow in Chapter 1 follows all seven principles. The gaps for mobile (real devices, store review, post-release monitoring) are covered in Chapters 9 and 10.

## Doubt Box
- **Is using Cursor the same as ADLC?** Not by itself. ADLC begins when the agent owns tasks and the process is designed around checkpoints.
- **Does ADLC replace Agile?** No. Agile cadence can wrap ADLC; sprints still make sense.
- **Where is the human?** At the decisions, not at the keyboard for every line.

## Try it
Score your current workflow against the seven principles. Which are missing?

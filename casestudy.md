# Running Case Study: ExampleMart

A small e-commerce app used as the one example that threads through every chapter. Readers meet the same app, team, and problems from Chapter 1 to Chapter 14.

## The app
**ExampleMart** is a mobile app for a local home-goods store that sells online across Indian cities.
- **Team:** 1 product owner, 2 mobile developers (one Android, one iOS), 1 QA, 1 part-time designer, 1 backend developer. Small on purpose, so agents make a visible difference.
- **Platforms:** Android first (most of its users), iOS second.
- **Core features:** browse products, search, cart, checkout with UPI / cards / cash on delivery, order tracking, push notifications.
- **Users:** many on budget Android phones, patchy mobile data, a mix of English and regional languages.

Why this app works for teaching: every mobile pain point from Chapter 2 shows up naturally. Budget devices (fragmentation), weak networks (offline cart), payments (security and privacy), and festival-season traffic spikes (release risk).

## The characters
- **Asha**, product owner: writes the requirements.
- **Ravi**, Android developer: the main agent user, works like the workflow in Chapter 1.
- **Meera**, QA: learns to judge agent-written tests.
- **Imran**, tech lead and maintainer: owns the merge gate.

## The running feature thread
Each chapter picks up one of these.

| Chapter | ExampleMart scenario |
|---|---|
| 1. Classic SDLC | How "Add to cart" shipped under the old process, including a two-day store review that delayed a sale |
| 2. Where SDLC strains | A bug appears only on a low-memory budget phone, found three days after release |
| 3. Tools to agents | Ravi tries the same small task as chat help, then as an agent goal |
| 4. Defining ADLC | The new workflow applied to the feature "Save cart offline" |
| 5. Changing roles | Who owns what on the ExampleMart team once agents join |
| 6. Specs | Asha's vague ticket "make checkout faster" turned into an agent-ready spec through clarifying questions |
| 7. Design to code | Product listing screen built from the ExampleMart design tokens, with and without them |
| 8. Agentic coding | UPI payment flow built as small PRs, with agent review comments shown |
| 9. Testing | Agent tests pass but miss a payment-timeout case; Meera's independent tests catch it |
| 10. Release and ops | Festival-sale release: staged rollout, crash spike, kill switch |
| 11. Evaluating agents | Imran compares three tools on the same ten ExampleMart tasks |
| 12. Governance | A leaked payment-gateway test key and a risky dependency; rules the team adopts |
| 13. Adoption | ExampleMart moves from Stage 1 to Stage 3 over a quarter |
| 14. Road ahead | ExampleMart adds an on-device assistant and exposes "reorder" to agents |

## The story arc
1. **Before:** the team ships slowly, bugs reach users, releases are stressful.
2. **Experiments:** Ravi starts using agents; early wins and surprising failures.
3. **Structure:** the team writes specs, small PRs, and review gates (ADLC).
4. **Crisis:** a festival-sale release goes wrong; the process catches or fails to catch it.
5. **Maturity:** metrics, governance, and a repeatable playbook.

## Writing rules for the case-study boxes
- Every chapter gets a box titled **"ExampleMart: [scenario]"**, 150 to 300 words.
- Show the real artifact where possible: the prompt, the spec, the PR comment, the test, the rollout plan.
- Include at least one thing that **went wrong**, because failures teach more than clean wins.
- Keep names and details consistent across chapters.
- Where a scenario is illustrative rather than real, label it clearly as a composite example.

## Decisions (current defaults)
1. **Fictional sample.** ExampleMart is an illustrative example created for learning. It is not a real company or project, and no confidential details are used. The book states this plainly in the introduction.
2. **Stack for code samples: Kotlin with Jetpack Compose (Android).** Chosen because ExampleMart is Android first. Each chapter explains the idea in platform-neutral terms, so iOS and cross-platform readers can follow. Revisit if the author prefers another stack.
3. **Ending: an honest mix of wins and remaining problems.** Readers trust a story that admits what is still hard.

These are defaults and can change at any time.

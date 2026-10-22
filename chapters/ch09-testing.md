# Chapter 9: Testing

## "Repeat until bug-free" and its limits
Code is only as correct as its tests. If the same agent writes code and tests, both can share one wrong assumption and pass together. Passing tests mean "matches the tests", not "correct".

## The testing layers for mobile
1. **Unit tests**: logic in isolation. Agents excel here.
2. **Integration tests**: modules and APIs together.
3. **UI tests**: flows on emulators/simulators.
4. **Device farm tests**: real devices across OS versions and models.
5. **Visual regression**: screenshot comparison to catch layout breaks.
6. **Exploratory testing**: agents or humans poking for unexpected failures.

## Independent verification
- Write acceptance tests from the **spec**, before or separate from implementation.
- Use a different agent or model to review tests.
- Add mutation testing or edge-case lists to check tests actually fail when code is wrong.
- Keep a human-reviewed set of critical-path tests.

## Mobile-specific cases agents forget
Permission denial, rotation, backgrounding, low memory, offline, slow network, interrupted installs, old OS, accessibility settings.

## Doubt Box
- **If tests pass, is it safe to ship?** No. It means the tests passed.
- **Can agents replace QA?** They scale test writing and execution; QA judgment on strategy and risk remains.
- **Do I need real devices?** For release confidence on mobile, yes, at least for critical flows.

## Try it
Ask a second agent to write tests from the spec only, then run them against the first agent's code.

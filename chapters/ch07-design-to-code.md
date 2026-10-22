# Chapter 7: Design to Code

## The idea
Agents can turn designs (images, design files, or descriptions) into screens. Quality depends on the rules you give them.

## Give agents your design system, not just a picture
A screenshot shows one state. A design system defines reusable rules: colors, typography, spacing, components, and their states. Provide tokens and component names so output reuses what exists instead of inventing new styles.

## Platform conventions
- **iOS (SwiftUI/UIKit)** and **Android (Jetpack Compose)** have different navigation, gestures, and accessibility patterns. Tell the agent which platform conventions to follow.
- **Cross-platform (Flutter, React Native)** share code but still need platform-aware behavior.

## What agents do well and badly
- Well: layout scaffolding, repeating components, wiring state to UI, previews.
- Badly: subtle spacing, motion polish, unusual platform behavior, accessibility details unless asked.

## Review checklist for generated UI
Uses design tokens, handles all states (loading, empty, error), supports large text and screen readers, works on small and large screens, matches platform navigation.

## Doubt Box
- **Can I paste a screenshot and get a finished screen?** You get a starting point. Expect to refine.
- **Why does generated UI look generic?** Because it lacked your design system. Provide it.
- **Should agents create new components?** Only if no existing one fits; prefer reuse.

## Try it
Generate one screen twice: once from a screenshot alone, once with tokens and component list. Compare.

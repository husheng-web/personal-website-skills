---
name: portfolio-motion-qa
description: Review or implement portfolio UI motion against an existing motion system, including reduced-motion, keyboard, performance, and responsive constraints.
---

# Portfolio Motion QA

Use motion only when it clarifies hierarchy, orientation, feedback, sequence, or continuity.

## Inspect first

Read the project's motion rules, token source, and existing motion primitives. Reuse their semantics and durations instead of adding an independent scale or a new animation library.

## Decision rules

- Keep reading-first content static unless animation provides a clear benefit.
- Prefer opacity and transform; avoid layout animation, ambient loops, scroll hijacking, character staggering, and `transition: all`.
- Keep motion optional: reduced-motion resolves immediately and keyboard operation never waits for animation.
- Check hover and focus produce equivalent state changes; do not depend on pointer behavior on mobile.

## Validate

Test normal and reduced-motion states, keyboard focus, desktop/mobile layout, and replay/exit behavior where applicable. Report the reason for each motion choice, its token/primitive, and any deviation requiring a documented project decision.

---
name: portfolio-visual-qa
description: Compare a portfolio website route with an approved visual reference at desktop and mobile sizes, then report evidence-backed visual defects and fixes.
---

# Portfolio Visual QA

Perform visual verification rather than a code-only review.

## Setup

Confirm the reference, route, UI state, viewport sizes, and whether the task permits implementation. Start the site through its established command and inspect rendered output at the requested sizes; include one mobile size when the request does not specify it.

## Compare

Assess hierarchy, typography and wrapping, spacing and geometry, colors and contrast, asset fidelity, responsive crop/overflow, and interactive states. Verify keyboard reachability and reduced-motion behavior when motion or navigation is involved.

## Report

State the evidence and limitations first. Group findings by priority:

- `P1`: blocks the intended hierarchy, access, or core task.
- `P2`: material visual or responsive mismatch.
- `P3`: polish that can wait.

For each finding, name the affected route/state, observed behavior, likely source, and the smallest credible fix. Retest fixes in the affected viewport. Do not claim a visual check passed when the browser capture or target reference was unavailable.

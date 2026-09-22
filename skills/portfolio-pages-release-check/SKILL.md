---
name: portfolio-pages-release-check
description: Validate a statically exported portfolio website for GitHub Pages release readiness. Use before publishing or diagnosing deployment regressions.
---

# Portfolio Pages Release Check

Establish whether the checked-out site is ready for its configured static-hosting release.

## Inspect

Read package scripts, framework export configuration, configured public site URL, robots/sitemap behavior, and the GitHub Actions workflow. Preserve the repository's deployment target and branch unless the user requests a change.

## Validate

Run the repository's formatting check when practical, then lint, typecheck, and production build. Confirm the expected static output exists, configured base/public URL is used in generated metadata where relevant, and no server-only route or runtime dependency prevents static export. Review the workflow for install, build, artifact, permissions, and deploy stages.

## Reporting and safety

Report exact commands, exit states, salient warnings, and any unverified remote setting separately. This skill validates readiness; it must not push commits, enable Pages, change repository settings, or create releases unless the user explicitly asks.

---
name: portfolio-bilingual-qa
description: Validate Chinese and English portfolio routes, content states, metadata, and fallbacks. Use when adding or reviewing localized portfolio content.
---

# Portfolio Bilingual QA

Check localization as a publishing-integrity problem, not merely a string comparison.

## Inspect

Read the locale helpers, dictionaries, project/case registry, route generation, metadata, sitemap, and language-switch behavior. Compare equivalent Chinese and English routes where source content exists.

## Required checks

- Locale validation, fallback, and switching preserve the current route when an equivalent exists.
- Navigation, CTA, status, empty-state, metadata, and alt-text paths are localized.
- Approved English copy is used as supplied; unsupported English claims remain pending or are omitted according to the project's policy.
- Sitemaps expose only publishable pages and canonical URLs use the configured public site URL.
- Mixed CJK/Latin text wraps without truncation at desktop and mobile sizes.

## Deliverable

Report a route-by-route matrix of pass, pending, mismatch, and evidence. Make minimal safe corrections only when asked; never silently translate or fabricate factual content.

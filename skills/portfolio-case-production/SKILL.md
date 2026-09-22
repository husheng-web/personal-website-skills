---
name: portfolio-case-production
description: Build or update an evidence-backed portfolio case study in an existing website. Use after narrative facts and media have been approved.
---

# Portfolio Case Production

Implement a project case without turning incomplete material into fabricated narrative.

## Before editing

Inspect the repository's project registry, content contract, case components, locale handling, and an existing comparable case. Identify which facts and media are actually approved.

## Implementation shape

- Keep identity, route/status, and compact metadata in the registry; put approved narrative in the repository's established content layer; keep layout and media treatment in reusable components.
- Render only supported sections and blocks. A partial case is valid when it honestly omits unavailable evidence.
- Attach localized copy deliberately. Do not auto-translate factual content merely to fill an English route.
- Add media only with meaningful alt text and known dimensions where the host contract requires them. Preserve the intended reading width and avoid forcing dense diagrams into mobile layouts.

## Validation

Run relevant lint, type, and production-build checks. Verify the target locale routes, pending/partial behavior, SEO metadata, keyboard links, image loading, and mobile overflow. Report approved content used separately from remaining gaps.

## Boundary

Do not use this skill to create a new design system or make unapproved public claims. Use content intake first when source material is ambiguous.

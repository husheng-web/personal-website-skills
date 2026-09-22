---
name: portfolio-project-preview-reader
description: Add or review an accessible portfolio project-preview reader for ordered long images, document pages, or staged visual modules.
---

# Portfolio Project Preview Reader

Present approved long-form project visuals inside an existing archive preview without breaking the surrounding browsing flow.

## Before implementation

Inspect the archive/dialog state model, existing document-reader paths, project registry, source asset order, and mobile styles. Generalize only an actual repeated behavior; keep one-off project rules local when no reusable abstraction is justified.

## Requirements

- Preserve declared source order and give each page or module an accessible localized label.
- Use a contained vertical reading surface; do not expand the page unexpectedly or introduce horizontal overflow.
- Preserve close, Escape, focus restoration, scroll lock, and keyboard behavior already provided by the preview dialog.
- Route to a detail page only when one is publishable; do not expose a broken or semantically duplicate destination.

## Validation

Check all assets load, ordered labels are present, preview open/close works, and reader width has no horizontal overflow at desktop and mobile sizes. Run type, lint, and production build checks after code changes.

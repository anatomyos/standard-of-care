# standard-of-care
A scroll-driven essay: The mundane checkup, and the fortune you unwittingly inherited.
   
    **inspired by https://ordinaryabundance.com/

## Files

| File | Purpose |
|---|---|
| `index.html` | **The site.** Deploy this + `images/`. |
| `images/` | 11 illustrations + `og-card.jpg` for social previews. |
| `preview-interactive.html` | Self-contained preview with design controls + spotlight tuner. **Do not deploy.** |
| `preview-standalone.html` | Self-contained, no controls. For emailing to people. **Do not deploy.** |

Deploy payload is `index.html` + `images/` only — about 1.4 MB.

## Editing

All copy lives in the `BEATS` and `ENTRIES` objects at the top of the `<script>`
block in `index.html`. Each entry takes:

- `station` / `title` — labels above the entry
- `img` / `alt`
- `spot` — `{x,y,w,h}` as percentages of the hero; drives the spotlight
- `quote` / `cite` / `note`
- `noteOpen: true` — show the context paragraph expanded (default: collapsed)
- `status` — `"ready"` or `"tk"` (renders a NEEDS SOURCING badge)


# Project structure and ownership

## Root files

| Path | Responsibility |
|---|---|
| `README.md` | Single source of truth for profile copy, section order, links, and asset references. |
| `LICENSE` | Reuse permissions for repository content. |
| `docs/design.md` | Visual concept and section-level design decisions. |
| `docs/analysis.md` | Analysis of the reference project; not a source to copy. |

## Folder responsibilities

| Path | Responsibility | Rules |
|---|---|---|
| `assets/images/` | Raster screenshots and original images. | Prefer compressed WebP/PNG; store source attribution when needed. |
| `assets/svg/` | Static diagrams and vector artwork. | Use descriptive names and `viewBox`; do not hide key text only in artwork. |
| `assets/icons/` | Small icons. | Keep a single visual family and license compatible with this repository. |
| `assets/background/` | Non-content visual layers. | Keep contrast low so text stays primary. |
| `assets/animations/` | Motion assets. | No script or rapid flashing; every effect needs a readable static state. |
| `assets/typing/` | Terminal/typing visuals and configuration. | Use sparingly; the hero is the preferred location. |
| `docs/` | Decisions, architecture, and change notes. | Update documentation when a convention changes. |
| `.github/workflows/` | CI and scheduled automation. | Pin third-party actions before production and use least-privilege permissions. |
| `scripts/` | Local repeatable helpers. | Scripts must be documented, idempotent where practical, and never modify profile facts silently. |

## Naming convention

- Use lowercase kebab-case: `hero-neural-grid.svg`, `project-commerce-dashboard.webp`.
- Name by role, not version: avoid `final.svg`, `new.svg`, and `v2.svg`.
- Keep a single asset in a single role folder. If an old asset is no longer referenced, remove it only as part of an explicit cleanup.

## Safe update sequence

1. Update content or asset in its owning location.
2. Update the relative reference in `README.md`.
3. Check all links and alt text.
4. Validate the rendered README in GitHub dark and light modes.
5. Record non-obvious design or automation changes in `docs/`.

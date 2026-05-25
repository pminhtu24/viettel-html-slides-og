# Icon Sourcing Guide

Use this only when a suitable icon is not available in `./assets/viettel-icon-v1/icons/`.

## Purpose

- This file guides icon sourcing at authoring time (JSON preparation), not runtime fallback in HTML.
- Goal: all `icon_src` in JSON must point to existing local files before generation.

## Pre-Generation Validation

1. Collect all icon paths from JSON (`icon_src` and icon `<img src="...">` in `icon_svg`).
2. Check file existence in workspace.
3. For missing paths, resolve by semantic mapping (see `SKILL.md` Icon Fallback Mapping).
4. If still unresolved, use `./assets/viettel-icon-v1/icons/info.svg`.
5. Generate HTML only after missing icon count = 0.

## Trusted Sources

- Feather Icons: https://feathericons.com
- Heroicons: https://heroicons.com
- Font Awesome (SVG only): https://fontawesome.com
- Bootstrap Icons: https://icons.getbootstrap.com
- Material Symbols: https://fonts.google.com/icons

## Processing Steps

1. Download an SVG in monochrome or single-color style.
2. Normalize to fit a `64x64` visual box.
3. Save in `./assets/viettel-icon-v1/icons/` with a descriptive filename.
4. Prefer stroke/shape simplicity consistent with existing Viettel icon style.
5. Verify rendering in a generated slide before final output.

## Quality Checklist

- No external references/scripts in SVG.
- Consistent visual weight with existing icon set.
- Clear readability at small slide size.
- Optimized file size (use SVGOMG if needed).
- Local path is valid and render-tested in generated slide.

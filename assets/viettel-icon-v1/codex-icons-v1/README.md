# Viettel Icon Library (SVG)

Hand-drawn style icon assets for slide use.

## Spec

- `64x64` viewBox
- Circular background (`#E4002B` or `#1F2937`)
- White glyph (`#FFFFFF`)
- Rounded caps/joins for clean small-size rendering

## Icons Included

- analytics
- api
- automation
- cloud
- compliance
- cost
- data-pipeline
- database
- devops
- innovation
- integration
- network
- performance
- platform
- reliability
- security
- settings
- speed
- strategy
- support
- team
- uptime

## Usage in `icon-text-grid`

Use inline SVG string in JSON:

```json
{
  "layout": "icon-text-grid",
  "items": [
    {
      "icon_svg": "<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 64 64'><circle cx='32' cy='32' r='30' fill='#E4002B'/><path d='M18 44h28M22 40V30M32 40V22M42 40V27' fill='none' stroke='#fff' stroke-width='4' stroke-linecap='round' stroke-linejoin='round'/></svg>",
      "title": "Analytics",
      "copy": "Operational metrics and KPIs."
    }
  ]
}
```

Or load file content from `assets/viettel-icon-v1/codex-icons-v1/*.svg` and inject to `icon_svg`.

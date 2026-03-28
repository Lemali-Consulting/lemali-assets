# Lemali Consulting — Brand Assets

Canonical source of truth for Lemali Consulting brand assets. Use this repo as a submodule or package dependency in any Lemali-branded project.

## Structure

```
logos/
  svg/          # SVG logo variants (primary, wordmark, icon; on-dark and on-light)
  png/          # PNG renders of each SVG variant (for OG/social meta tags)
colors/
  tokens.json   # Color tokens as JSON (for tooling, design systems)
  tokens.css    # CSS custom properties
fonts/          # Font metadata and Google Fonts embed snippet
styles/
  global.css    # Shared brand utilities (data-dots, grid patterns, dividers)
favicons/       # favicon.svg, favicon.ico
```

## Logo Variants

| File | Variant | Background |
|------|---------|------------|
| `primary-on-dark.svg` | Bracket + "Lemali" + "Consulting" | Dark (navy) |
| `primary-on-light.svg` | Bracket + "Lemali" + "Consulting" | Light (white/cream) |
| `wordmark-on-dark.svg` | Bracket + "Lemali" | Dark |
| `wordmark-on-light.svg` | Bracket + "Lemali" | Light |
| `icon-on-dark.svg` | Bracket + dot only | Dark (navy) |
| `icon-on-light.svg` | Bracket + dot only | Light (white) |
| `icon-transparent.svg` | Bracket + dot only | Transparent |
| `*-on-dark-transparent.svg` | (primary / wordmark) | Transparent, white text for dark surfaces |
| `*-on-light-transparent.svg` | (primary / wordmark) | Transparent, dark text for light surfaces |

## Colors

| Token | Hex | Usage |
|-------|-----|-------|
| Brand Blue | `#2563EB` | Bracket stroke, links, primary actions |
| Brand Blue Light | `#3B82F6` | Hover states |
| Amber | `#E5A920` | Data dot accent |
| Navy | `#0F1D2F` | Dark backgrounds, text on light |
| Cream | `#F5F0E8` | Warm light backgrounds |
| Cool Gray | `#F3F4F6` | Cool light backgrounds |

## Fonts

- **IBM Plex Sans** (400, 600) — body, headings, wordmark
- **IBM Plex Mono** (400) — data labels, subtitle, code

See `fonts/google-fonts.html` for the embed snippet.

## Usage

Add as a git submodule:

```bash
git submodule add git@github.com:Lemali-Consulting/assets.git assets
```

Then reference assets by path (e.g., `assets/logos/svg/primary-on-dark.svg`).

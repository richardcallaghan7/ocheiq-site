# OcheIQ Landing Page Screenshots

Screenshots for the landing page at https://ocheiq.com

## Current Screenshots (Build #56)

| Filename | WebP | Description | Used In |
|----------|------|-------------|---------|
| `score.png` | `score.webp` | Session detail — 90 Elite Mechanics, all 5 metric bars | Hero, Features |
| `results.png` | `results.webp` | Insights tab — "Dart 1 was rushed", pattern detection, recent sessions | Hero, Features |
| `consistency.png` | `consistency.webp` | Throw overlay paths view with coaching drill | Hero, Features |
| `coaching.png` | `coaching.webp` | Wrist heatmap with release cluster zone | Features |
| `replay-overlay.png` | `replay-overlay.webp` | Skeleton overlay with trajectory path and phase nav | Features |
| `upload.png` | `upload.webp` | Record tab — OcheIQ logo, Today's Focus, Analyze Video | Solution section |

## Image Formats

All screenshots are served as WebP with PNG fallback via `<picture>` elements:

```html
<picture>
    <source srcset="screenshots/score.webp" type="image/webp">
    <img src="screenshots/score.png" alt="..." class="pos-score-hero">
</picture>
```

| Format | Total Size | Notes |
|--------|-----------|-------|
| PNG (fallback) | ~4.0 MB | Original high-res, used by older browsers |
| WebP (primary) | ~422 KB | Served to all modern browsers (~90% reduction) |

## Image Positioning (CSS Classes)

### Hero Section (Phone Mockups)
- `results.png` - `pos-results-hero` (top center) - Shows "Dart 1 was rushed"
- `score.png` - `pos-score-hero` (center 38%) - Shows 90 Elite score ring
- `consistency.png` - `pos-consistency-hero` (center 12%) - Shows throw overlay

### Solution Section (Phone Mockup)
- `upload.png` - `pos-upload` (top center) - Shows clean upload UI

### Features Section (Feature Cards)
- `replay-overlay.png` - `pos-replay` (center 45%) - Shows skeleton overlay
- `consistency.png` - `pos-consistency` (center 20%) - Shows throw paths
- `score.png` - `pos-score` (center 45%) - Shows score ring and metrics
- `coaching.png` - `pos-results` (top center) - Shows heatmap and coaching

## How to Update Screenshots

1. Take new screenshots from TestFlight or Simulator (iPhone 17 Pro)
2. Copy PNG to this folder with appropriate name
3. Generate WebP: `cwebp -q 80 screenshot.png -o screenshot.webp`
4. Update `index.html` positioning classes if needed
5. Push to main (Vercel auto-deploys)

## Screenshot Guidelines

- **Format**: PNG source + WebP optimized (both required)
- **WebP conversion**: `cwebp -q 80` (quality 80 — good balance for UI screenshots)
- **Resolution**: iPhone 17 Pro (1206x2622) for website, resize to 1320x2868 for App Store
- **Mode**: Dark mode (matches landing page theme)
- **Content**: Show real analysis data, not empty states
- **Scores**: Aim for good scores (85+) for impressive presentation

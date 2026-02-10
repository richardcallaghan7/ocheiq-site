# OcheIQ Landing Page Screenshots

Screenshots for the landing page at https://ocheiq.com

## Current Screenshots (Build #37)

| Filename | Source | Description | Used In |
|----------|--------|-------------|---------|
| `upload.jpg` | IMG_9057 | Upload screen with "Upload Video" button and Video Requirements | Solution section |
| `results.jpg` | IMG_9058 | Results showing "Dart 2 was rushed" with baseline building | Hero, Features |
| `share.jpg` | IMG_9059 | Session detail with 85 ±6 score, skill band, timing insight | Hero, Features |
| `consistency.jpg` | IMG_9060 | Arm path overlay with 96% consistency, analysis insights | Hero, Features |
| `replay-overlay.jpg` | IMG_9061 | Video replay with skeleton tracking overlay | Features |

## Image Positioning (CSS Classes)

### Hero Section (Phone Mockups)
- `results.jpg` - `pos-results-hero` (top center) - Shows "Dart 2 was rushed"
- `share.jpg` - `pos-score-hero` (center 38%) - Shows score card and skill band
- `consistency.jpg` - `pos-consistency-hero` (center 12%) - Shows arm path graph

### Solution Section (Phone Mockup)
- `upload.jpg` - `pos-upload` (top center) - Shows clean upload UI

### Features Section (Feature Cards)
- `replay-overlay.jpg` - `pos-replay` (center 45%) - Shows person with skeleton
- `consistency.jpg` - `pos-consistency` (center 20%) - Shows arm path visualization
- `share.jpg` - `pos-score` (center 45%) - Shows skill band progress
- `results.jpg` - `pos-results` (top center) - Shows pattern detection insight

## How to Update Screenshots

1. Take new screenshots from TestFlight or Simulator
2. Copy to this folder with appropriate name
3. Update `index.html` positioning classes if needed
4. Deploy: `vercel --prod`

## Screenshot Guidelines

- **Format**: JPG preferred (smaller file size)
- **Resolution**: iPhone native resolution (1179x2556 for iPhone 14 Pro)
- **Mode**: Dark mode (matches landing page theme)
- **Content**: Show real analysis data, not empty states
- **Scores**: Aim for good scores (70+) for impressive presentation

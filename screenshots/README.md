# OcheMaster Landing Page Screenshots

Add the following screenshots to this folder. Use PNG format, captured from an iPhone at native resolution (preferably iPhone 14/15 Pro for best quality).

## Required Screenshots

### Hero Section (3 phones side by side)

| Filename | Description | What to Capture |
|----------|-------------|-----------------|
| `results.png` | Main results screen | Overall score circle, stability/alignment scores, metric breakdown |
| `replay.png` | Throw replay viewer | Video playing with skeleton overlay visible, phase colors showing |
| `progress.png` | Progress tracking tab | Trend charts, practice calendar, or goal progress |

### Feature Cards (4 screenshots)

| Filename | Description | What to Capture |
|----------|-------------|-----------------|
| `replay-overlay.png` | Full-screen throw replay | Best with skeleton and trajectory both visible, mid-throw phase |
| `consistency.png` | Throw overlay analysis | All throws superimposed, showing consistency patterns |
| `quadrant.png` | Two-axis diagnostic | The stability vs alignment quadrant with your position marked |
| `trends.png` | Progress over time | Line chart showing improvement, or the two-axis scatter plot |

### Solution Section (1 screenshot)

| Filename | Description | What to Capture |
|----------|-------------|-----------------|
| `metrics.png` | Metric cards expanded | Individual metric scores with skill bands (Elite/Advanced/Developing) |

## Tips for Great Screenshots

1. **Use Dark Mode** - The landing page is dark-themed, screenshots look better in dark mode
2. **Use a Real Session** - Capture actual analysis results, not empty states
3. **Show Good Scores** - Aim for sessions with decent scores (70+) to look impressive
4. **Crop Carefully** - Remove status bar if possible, or ensure it's clean (no low battery, no notifications)
5. **Consistent Size** - All screenshots should be the same dimensions

## How to Capture

### Option 1: Simulator
```bash
# Run app in simulator
cd mobile
npx expo start --ios

# Use Cmd+S to capture screenshot in simulator
```

### Option 2: Physical Device
1. Open the app on your iPhone
2. Navigate to the screen you want to capture
3. Press Side Button + Volume Up simultaneously
4. Find screenshot in Photos app
5. AirDrop to your Mac

### Option 3: From TestFlight Build
Use the TestFlight app version for the most accurate production screenshots.

## After Adding Screenshots

Update `index.html` to use the images. Replace the placeholder divs:

```html
<!-- Change this: -->
<div class="placeholder">
    <p>Add screenshot: screenshots/results.png</p>
</div>

<!-- To this: -->
<img src="screenshots/results.png" alt="Analysis Results">
```

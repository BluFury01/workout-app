# Workout App

A progressive web app (PWA) for home full-body workouts. Works offline, installs on your phone like a native app.

## Features
- 10 built-in routines across Fat Burn / Strength / Muscle (Beginner / Intermediate / Advanced)
- 35+ exercise library with muscle group filters and form instructions
- Rest timer with auto-start on exercise check-off
- Session history stored locally via IndexedDB (no cloud, fully private)
- Installable on Android and iOS

## Hosting on GitHub Pages

1. Create a new repo on GitHub (e.g. `workout-app`)
2. Upload all these files keeping the same folder structure
3. Go to **Settings → Pages → Source** and select `main` branch / root
4. Your app will be live at `https://yourusername.github.io/workout-app/`

## Installing on your phone (Android / Honor 200 Lite)

1. Open the GitHub Pages URL in **Chrome**
2. Tap the three-dot menu → **Add to Home screen**
3. Tap **Add** — it appears as an app icon
4. Open it once with internet to cache everything, then it works fully offline

## File structure

```
workout-app/
├── index.html      # Main app
├── manifest.json   # PWA manifest
├── sw.js           # Service worker (offline support)
└── icons/
    ├── icon-192.png
    └── icon-512.png
```

## Data storage

All session history is saved to **IndexedDB** on your device. Nothing is sent to any server. Clearing your browser data will clear history.

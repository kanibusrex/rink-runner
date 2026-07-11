# Rink Runner

A neon-themed indoor roller skating session tracker. Single-file web app — no build step, no dependencies.

**Live app:** https://kanibusrex.github.io/rink-runner/

## What it does

Indoor rinks have no GPS, so Rink Runner tracks laps manually — with an
optional GPS mode for outdoor tracks and open skating:

- Tap the lap button each time you pass the start line
- An oval "rink" visual with a skater dot circles based on your average lap pace
- Set your rink's lap length once (in feet) and distance auto-calculates
- **Auto-distance (GPS):** flip the toggle to measure distance from real
  movement instead — the browser's Geolocation API tracks your path and
  sums it up (with accuracy/jitter filtering). Off by default; falls back
  to manual laps if location is unavailable or blocked
- Stats: elapsed time, distance, average lap, best lap
- Pause / resume mid-session (GPS pauses too)
- Sessions save automatically to a local history, tagged `GPS` when tracked that way

> GPS needs a secure context (HTTPS) — it works on the live GitHub Pages
> URL. Indoors, GPS is unreliable, so manual lap mode remains the default.

## Design

- Roller-disco neon palette: hot pink, cyan, violet, amber
- Bungee + Space Grotesk + IBM Plex Mono type
- Custom neon "track" app icon (favicon + Apple touch icon embedded inline)
- Respects `prefers-reduced-motion`

## Running locally

Just open `index.html` in a browser. That's it.

## Deploy

Hosted on GitHub Pages from the `main` branch root. Any push to `main` updates the live app.

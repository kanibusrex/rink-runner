# Rink Runner

A neon-themed indoor roller skating session tracker. Single-file web app — no build step, no dependencies.

**Live app:** https://kanibusrex.github.io/rink-runner/

## What it does

Indoor rinks have no GPS, so Rink Runner tracks laps manually:

- Tap the lap button each time you pass the start line
- An oval "rink" visual with a skater dot circles based on your average lap pace
- Set your rink's lap length once (in feet) and distance auto-calculates
- Stats: elapsed time, distance, average lap, best lap
- Pause / resume mid-session
- Sessions save automatically to a local history

## Design

- Roller-disco neon palette: hot pink, cyan, violet, amber
- Bungee + Space Grotesk + IBM Plex Mono type
- Custom neon "track" app icon (favicon + Apple touch icon embedded inline)
- Respects `prefers-reduced-motion`

## Running locally

Just open `index.html` in a browser. That's it.

## Deploy

Hosted on GitHub Pages from the `main` branch root. Any push to `main` updates the live app.

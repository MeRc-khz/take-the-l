# Take the 'L' — Classification Yard Rush

A mobile-first rail-yard puzzle game. Inbound train cars roll in; tap each car to
sort it onto the matching track before the yard overflows. Order the cars
ENGINE → cars → CABOOSE to complete a consist.

Built with [Babylon.js](https://www.babylonjs.com/) (CDN) + vanilla HTML/CSS/JS.
Single-file, zero build step.

Live: https://takethel.game4real.us

## Files

| File | Purpose |
|------|---------|
| `index.html` | Current build — Babylon.js yard rush (inbound train strip, tap-car → track, ENGINE → cars → CABOOSE completion) |
| `index-v1-static.html` | Original static v1 (kept for reference) |
| `gameplay.png` | Gameplay screenshot |
| `overlay.png` | Overlay / OG art |

## Deploy

Static host. Source of truth is `index.html`; copy to the web root
(`/var/www/takethel/html/index.html`) — nginx serves it with
`Cache-Control: no-cache, must-revalidate` so updates bust automatically.

# Take the 'L' — Zig-Zag Yard

A mobile-first rail-yard sorting game. Each level an inbound train **zig-zags
down** from the top of the yard — longer and with more engines the deeper you go.

- **Tap the engines** on the train to save them into your shed.
- **Tap a car** to grab it, then **tap a vertical track** to load it.
- Cars arrive in **colour groups of 2–5**. A track only accepts cars once it has
  an **engine**, takes one colour at a time, and ships the load (and empties)
  when a whole group is aboard.
- Out of engines? **Buy one with your points** (40).

Built with [Babylon.js](https://www.babylonjs.com/) (CDN) + vanilla HTML/CSS/JS.
Single-file, zero build step.

Live: https://takethel.game4real.us

## Files

| File | Purpose |
|------|---------|
| `index.html` | Current build — zig-zag inbound train (Babylon.js), vertical tracks, engine shed, buy-with-points |
| `index-v1-static.html` | Original static v1 (kept for reference) |
| `gameplay.png` | Gameplay screenshot |
| `overlay.png` | Overlay / OG art |

## Deploy

Static host. Source of truth is `index.html`; copy to the web root
(`/var/www/takethel/html/index.html`) — nginx serves it with
`Cache-Control: no-cache, must-revalidate` so updates bust automatically.

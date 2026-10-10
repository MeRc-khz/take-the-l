# Take the 'L' — Switchback Yard

A mobile-first rail-yard sorting game. Each level an inbound train **runs flat
across the yard**, slips behind a tunnel to drop one train height, and comes
back the other way — longer and with more engines the deeper you go.

- **Tap the engines** on the train to save them into your shed.
- **Tap a car** to grab it, then **tap a vertical track** to load it. Tapping a
  bare track while holding a car couples an engine first.
- Cars arrive in **colour batches of 2–5** and colours repeat, so a track can
  stack as long as you can feed it.
- At **3 cars or more**, buy a **caboose** (10 pts) to close the train and move
  it off the track — that frees the track for the next train.
  **The longer the train, the more it pays:** 3 cars 36 · 5 cars 100 · 8 cars 256.
- Tapping a track holding only **1–2 cars shunts them back onto the tail of the
  inbound train** — −6 a car, and they ride the whole switchback again. The engine
  stays coupled, so a track can never be permanently dead-ended.
- **🃏 Wild cards** join any colour already on a track. Buy one for **30**, or
  grab one off the inbound train when it rides past (up to 3 per level).
- Out of engines? **Buy one with your points** (40). Leave a train unclosed when
  the inbound train clears and the yard gives you 6 seconds before scrapping it.

Built with [Babylon.js](https://www.babylonjs.com/) (CDN) + vanilla HTML/CSS/JS.
Single-file, zero build step.

Live: https://takethel.game4real.us

## Files

| File | Purpose |
|------|---------|
| `index.html` | Current build — switchback inbound train through tunnels (Babylon.js), vertical tracks, engine shed, buy-with-points |
| `index-v1-static.html` | Original static v1 (kept for reference) |
| `gameplay.png` | Gameplay screenshot |
| `overlay.png` | Overlay / OG art |

## Deploy

Static host. Source of truth is `index.html`; copy to the web root
(`/var/www/takethel/html/index.html`) — nginx serves it with
`Cache-Control: no-cache, must-revalidate` so updates bust automatically.

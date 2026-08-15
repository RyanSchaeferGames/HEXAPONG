# Hexapong

Six walls, one survivor. A single-file browser arcade game with no build step, no dependencies.

Play: **https://ryanschaefergames.github.io/Hexapong/**

## How it plays

You control the paddle on the bottom wall. Five opponents hold the other five. Every ball that
gets past you burns a block off your wall; lose them all and your wall is removed and the arena
collapses to a smaller shape. Last wall standing wins.

- **Move** — drag anywhere on screen (touch) or move the mouse / arrow keys / A and D
- **Slice** — swipe through the ball and your paddle's motion carries into it
- **Tokens** — gold helps whoever hit the ball last, red punishes whoever hits it next, violet
  warps the arena for everyone. Vanilla Mode turns them off; Custom Mode picks them one by one.
- **Difficulty** — harder opponents do not just block better, they work the ball back toward
  your wall more often. Easy leaves the ball to wander.
- **Score** — Vanilla and Token matches score you on survival time, finishing place and difficulty.
  Your best sits on the main menu, your running score sits at the bottom of the arena next to the
  number to beat, and Stats keeps the top five runs per difficulty.

## Files

| File | Purpose |
|---|---|
| `index.html` | The entire game. Open it and it runs. |
| `manifest.webmanifest` | Makes "Add to Home Screen" launch fullscreen |
| `icon-180.png` | Home-screen icon for iOS |
| `icon-192.png` / `icon-512.png` | Icons for Android / Chrome |

## Updating the game

Replace `index.html` with a newer build, keeping the filename. GitHub Pages redeploys within a
minute or so. If your phone still shows the old version, close the tab and reopen it, or pull down
to refresh.

## Why host it instead of opening the file

Saving your settings and career stats relies on browser storage, which is unreliable when a page is
opened straight from a file. Served over HTTPS and added to the Home Screen, stats persist properly
and the Share button can use the real system share sheet.

---

Created by Ryan Schaefer.

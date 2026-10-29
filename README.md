# Snake

A fullscreen, Nokia-style Snake game in a single HTML file. No build step, no dependencies.

![Snake](https://img.shields.io/badge/keys-arrows%20%2F%20wasd-4b7734)

## Play

Open `index.html` in any modern browser.

Or serve it locally:

```bash
python3 -m http.server 8080
# then open http://localhost:8080
```

## Controls

| Key | Action |
| --- | --- |
| `↑` `↓` `←` `→` / `WASD` | Steer the snake |
| `Enter` | Start / restart |
| `Space` | Pause / resume |
| `M` | Mute sound |
| `F` | Toggle fullscreen |

Swipe to steer on touch devices.

## Rules

- Eat the pulsing square to grow and score 10 points.
- Hitting a wall or your own tail ends the run.
- The snake speeds up every 50 points.
- Your best score is saved in `localStorage`.

## Tech

- Single file: `index.html`
- Canvas 2D, ~60 fps fixed-step game loop
- Hand-drawn 5x7 bitmap font for the retro LCD look
- Web Audio square-wave blips
- Board scales to fill any window size

# 📼 Retro Lens

**Your hands are the viewfinder.** Frame a piece of the world with your fingers and watch it turn into thermal vision, a glitchy mess, or a pencil sketch. It runs in your browser, with no install and no server.

## Quick start

1. Open `retro-lens.html` in Chrome, Edge, or Firefox.
2. Click **Start camera** and allow access.
3. Hold up a hand (or two) and play.

## How it works

Your fingertips become the corners of a portal, and whatever sits inside gets filtered.

| You do this | This happens |
|---|---|
| Show one hand | A portal opens between thumb, index, middle, and pinky |
| Show two hands | A portal stretches between both hands |
| Twist a hand | The quad flips into a **bowtie** 😍✌🏼 |
| Pinch thumb to pinky | Cycles to the next filter |
| Make **two fists** | Toggles 2D ⇄ 3D mesh mode |

In **3D mesh mode** with two hands, you get two portals at once. The second one uses the *next* filter in the list.

## Filters

`dual-tone` · `thermal` · `sketch` · `pixelate` · `glitch` · `invert` · `red-channel` · `edge` · `blur` · `cartoon` · `rainbow-wave`

## Keyboard

| Key | Action |
|---|---|
| `N` / `P` | Next / previous filter |
| `C` | Toggle 2D / 3D mode |
| `S` | Save a PNG of the current frame |
| `Q` | Stop the camera |

## Tips

- Good light makes tracking much better.
- Pinching too close to the camera will spam the filters. There's a short cooldown, but you'll still cycle fast.
- Portals smaller than about 10px are skipped, so spread your fingers out.

## Known quirks

- The edge filter uses Sobel instead of Canny, so it looks a little different from the Python version.
- Cartoon swaps the bilateral filter for blur plus color quantization.
- Safari doesn't support `ctx.filter`, so blur-based filters won't work there.

## Built with

MediaPipe Hands, the Canvas API, and plain JavaScript.
*Point. Pinch. Glitch.*

**UMMM I NEED A PRESS RELEASE FOR THIS NOWWW 😍✌🏼**
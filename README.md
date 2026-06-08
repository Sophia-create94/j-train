# A Day on the J Train

An interactive scrollytelling piece that follows a single day's ride along the J line — from Bed-Stuy, Brooklyn into Lower Manhattan. As you scroll, a train dot travels down the line and stops at each station, where a short, personal note about that part of the day unfolds.

🔗 **Portfolio / case study:** [sophia-ux.framer.website](https://sophia-ux.framer.website/)

## The idea

The page borrows the visual language of a subway map and turns it into a vertical timeline. The line bleeds top to bottom behind everything; a single train dot is the "you are here." Scrolling *is* the journey — the dot advances, the active stop opens, and each station reveals a feeling rather than a fact:

| Stop | Moment |
| --- | --- |
| **Gates Av** | Starting the day in Bed-Stuy |
| **Marcy Av** | Favorite spots, over the Williamsburg Bridge |
| **Delancey St – Essex St** | First stops in the city |
| **Canal St** | A slower afternoon |
| **Chambers St** | Last stop of the day, big views |

## Design notes

- **Phone frame** — the whole experience is composed inside a single mobile viewport, treating the ride as something held in one hand.
- **Type** — [Fraunces](https://fonts.google.com/specimen/Fraunces) for expressive display, [Geist](https://fonts.google.com/specimen/Geist) for the interface.
- **Palette** — near-black ground (`#0a0807`) with a warm rust line (`#B8743D`), so the route reads as the one bright thread through the day.
- **Motion** — scroll-driven; the train dot, the active station, and the expanding content are choreographed so the page never feels like a list of cards.

## Running it locally

It's a single static file with no build step. Either open it directly:

```bash
open index.html
```

…or serve it (recommended, for correct font/asset loading):

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Project structure

```
index.html      # the entire experience — markup, styles, and scroll logic
README.md
```

## Deployment

Hosted on Vercel; pushes to `main` deploy automatically.

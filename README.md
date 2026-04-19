# Fair Play — household card game (unofficial)

A free, open-source companion app inspired by the **Fair Play** system created by Eve Rodsky. It's a lightweight way for two partners to talk through who holds which household card — Conception, Planning, and Execution — and make the invisible work visible.

> **Live demo:** _add your Vercel URL here after deploying_

## What this is

- A single-page web app (no backend, no build step)
- ~80 household cards organized into 7 categories (Home, Out, Caregiving, Magic, Wild, Unicorn Space, Daily Grinds)
- Each card shows its CPE breakdown (Conception · Planning · Execution)
- Two partners take turns assigning cards; a live scoreboard tracks the balance
- Names and assignments are saved in your browser's localStorage — nothing leaves your device

## Disclaimer

This project is **not affiliated with, endorsed by, or sponsored by** Eve Rodsky, her publisher, or the official Fair Play organization. The Fair Play system, the CPE framework, the original card illustrations, and the Fair Play name are the intellectual property of their respective owners. The icons and design here are original work.

Please support the original — buy *Fair Play* by Eve Rodsky and the official Fair Play Deck:
- https://www.fairplaylife.com
- https://fairplaypolicy.org/the-cards

## Run locally

It's a single HTML file with no dependencies. Either:

```bash
# Option 1: open directly
open index.html

# Option 2: serve it (recommended for proper localStorage scoping)
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy to Vercel (free)

The easiest path — no CLI required:

1. Push this repo to GitHub (already done if you cloned it).
2. Go to [vercel.com/new](https://vercel.com/new).
3. Click **Import** next to the `fairplay` repo.
4. Leave all settings as default — Vercel auto-detects this as a static site.
5. Click **Deploy**. In ~30 seconds you'll get a public URL like `fairplay-xxx.vercel.app`.
6. Share the URL.

Every push to `main` will auto-deploy.

### Or with the Vercel CLI

```bash
npm i -g vercel
vercel login
vercel --prod
```

## Project structure

```
.
├── index.html      # the entire app — HTML, CSS, SVG icons, JS
├── vercel.json     # tells Vercel this is a static site
├── README.md
└── .gitignore
```

## License

The code in this repository is released under the MIT License (see `LICENSE` if added). The Fair Play system, framework, and brand are the property of Eve Rodsky and are not licensed by this project.

# Alhassana Diallo — Portfolio

My personal portfolio site. It brings together the software, AI/ML, and
security work I've been building — from an app-health dashboard and a log
triage tool to multi-agent reinforcement-learning research and a full-stack
vendor-finder app.

**Live site:** https://diallosanazy.github.io

It's a single, self-contained page: dark theme, hand-written HTML and CSS, no
framework and no build step — just `index.html` and an `assets/` folder of
project artwork.

## What's on the site

- **About** — a short intro and background.
- **Selected projects** — App Health Dashboard, Street Vendor Finder,
  App Log Analyzer, RL Playground, NexGen CAV (multi-agent RL), and a
  Vigenère cipher toolkit, each linking to its own repository.
- **Experience** — including my Information Security Engineering internship at
  Ariat International.
- **Skills** — languages, frameworks, tools, and concepts I work with.

## Built with

- Plain HTML5 and CSS (all styling is inline in `index.html` — no dependencies)
- Google Fonts: **Inter** and **JetBrains Mono**
- SVG artwork for each project card
- Hosted free on **GitHub Pages**

## Project structure

```
portfolio/
├── index.html            the single-page site
├── README.md             this file
└── assets/
    ├── app-health-dashboard.svg    project artwork
    ├── vendor-app.svg              Street Vendor Finder map view
    ├── app-log-analyzer.svg        project artwork
    ├── rl-playground.svg           training curves
    ├── nexgen-cav-marl.svg         multi-agent routing diagram
    └── vigenere-toolkit.svg        cracker output
```

## Running it locally

Open `index.html` directly in a browser, or serve it so relative paths behave
exactly like production:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## License

Personal project — all rights reserved.

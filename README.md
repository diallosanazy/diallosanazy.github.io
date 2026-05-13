# Alhassana Diallo — Portfolio

Single-page personal portfolio. Dark theme, no framework, no build step.
Just `index.html` + an `assets/` folder of project screenshots.

## Preview locally

Double-click `index.html` — it opens in your browser. That's it.

If you'd rather use a local web server (so the relative paths and font CDN
behave exactly like production):

```bash
cd /path/to/portfolio
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deploy to GitHub Pages (recommended — free, fast, your-username domain)

You'll get a live URL at **https://diallosanazy.github.io**.

### One-time setup

1. On GitHub, create a new **public** repository named exactly:

   ```
   diallosanazy.github.io
   ```

   The repo name has to match `<your-username>.github.io` — that's the
   magic phrase GitHub Pages recognizes for a "user site."

2. On your computer, in a fresh terminal:

   ```bash
   cd ~/Documents/projects
   mkdir diallosanazy.github.io
   cd diallosanazy.github.io
   ```

3. Copy this portfolio folder's contents into that new folder:

   ```bash
   cp -R "<path-to>/outputs/portfolio/." .
   ```

   (Drag-and-drop from Finder works too. You should now see `index.html`,
   `README.md`, and `assets/` inside `diallosanazy.github.io/`.)

4. Initialize git and push:

   ```bash
   git init
   git add -A
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/diallosanazy/diallosanazy.github.io.git
   git push -u origin main
   ```

5. Wait 30–60 seconds. Visit **https://diallosanazy.github.io** — it should
   be live.

### Updating later

Edit `index.html`, then:

```bash
git add -A
git commit -m "Update portfolio"
git push
```

Changes go live in ~30 seconds.

## What's in here

```
portfolio/
├── index.html            single-page site
├── README.md             this file
└── assets/
    ├── app-health-dashboard.svg    project screenshot
    ├── app-log-analyzer.svg        project screenshot
    ├── rl-playground.svg           project screenshot (training curves)
    └── vigenere-toolkit.svg        terminal-style cracker output
```

The site uses Google Fonts for **Inter** and **JetBrains Mono**. Everything
else (icons, layout, color tokens) is inline in `index.html` — no
dependencies, no build step.

## Custom domain (optional, later)

If you ever buy a custom domain like `alhassanadiallo.com`:

1. In your domain registrar's DNS settings, add records pointing to
   GitHub Pages (the four A records for `185.199.108.153`,
   `185.199.109.153`, `185.199.110.153`, `185.199.111.153`).
2. In your repo on GitHub: **Settings → Pages → Custom domain** → enter the
   domain.
3. Check "Enforce HTTPS" once GitHub finishes the SSL handshake.

## License

You wrote it, it's yours. No license required for personal use.

<p align="center">
  <img src="img/appicon/appicon-256.png" srcset="img/appicon/appicon-512.png 2x" width="128" height="128" alt="sudo sudoku logo">
</p>

# sudosudoku.github.io

Marketing site for [sudo sudoku](https://github.com/sudosudoku/sudo-sudoku) —
`sudo solve`, logic is root access. A terminal-fantasy sudoku for iPhone;
v2.0.0 App Store submission in progress.

Plain HTML + CSS, no build step, served by GitHub Pages. Design language:
Apple's design principles — minimal, content-first — carrying the app's
phosphor-green terminal identity.

## Local preview

```sh
python3 -m http.server 8080
# open http://localhost:8080
```

That's it. There is nothing to install and nothing to build.

## Structure

| Path | Purpose |
| --- | --- |
| `index.html` | Landing page |
| `privacy.html` | Privacy policy (App Store requirement) |
| `support.html` | Support page (content from app repo SUPPORT.md) |
| `css/main.css` | All styles |
| `img/` | App icon renditions and future screenshots |
| `docs/DESIGN.md` | Design language spec |
| `docs/CONTENT.md` | Copy guidelines and canonical strings |
| `AGENTS.md` | Working agreement for AI agents (CLAUDE.md imports it) |
| `CONTRIBUTING.md` | How to contribute (what's welcome, verify checklist) |
| `LICENSE` | MIT, same as [the app](https://github.com/sudosudoku/sudo-sudoku) |
| `.github/` | Issue/PR templates, security policy, Proof HTML CI |

## Deploying

Push to `main`. Vercel serves the repo root at
<https://sudosudoku.kaichen.dev> (canonical). `vercel.json` enables
`cleanUrls` so extensionless links like `/privacy` resolve. GitHub Pages
still mirrors the site at <https://sudosudoku.github.io>.

## Before launch

- [x] Replace the `TODO(app-store-url)` placeholder once the App Store page is live
- [x] Screenshots section (8 shots, 640px JPEGs in `img/screenshots/`,
      resized from Kai's 921×2000 originals)

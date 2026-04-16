# Sritanya Suresh Andal - ePortfolio

Personal portfolio built with [Quarto](https://quarto.org), published via GitHub Pages from the `docs/` folder.

## Local development

Prereqs:

- [Quarto](https://quarto.org/docs/get-started/) (≥ 1.4)
- Python 3.10+ with `jupyter`, `numpy`, `pandas`, `scikit-learn`, `scipy`, `matplotlib`, `plotly`

Install the Python dependencies:

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

Add the FontAwesome extension once:

```bash
quarto add quarto-ext/fontawesome
```

Preview the site:

```bash
quarto preview
```

Render to `docs/`:

```bash
quarto render
```

## Deployment

The site is configured to output to `docs/`. On GitHub, set **Settings → Pages → Source** to the `main` branch and the `/docs` folder.

## Structure

```
.
├── _quarto.yml          # site config, navbar, footer, theme
├── .nojekyll            # stop GitHub Pages processing with Jekyll
├── .gitignore
├── styles.scss          # light theme overrides
├── styles-dark.scss     # dark theme overrides
├── index.qmd            # landing page (trestles About template)
├── about.qmd
├── reflection.qmd
├── contact.qmd
├── images/              # logo, favicon, profile, cover art
├── cv/                  # CV PDF
├── blog/
│   ├── index.qmd        # blog listing
│   └── posts/           # individual posts
├── projects/
│   ├── index.qmd        # projects grid listing
│   ├── projects.yml     # project index
│   └── list/            # individual project pages (executable Python)
└── docs/                # rendered output (do not edit)
```

## Credits

- Built with [Quarto](https://quarto.org) and Bootstrap/[Bootswatch](https://bootswatch.com) themes (cosmo light / darkly dark).
- Typography: [Inter](https://rsms.me/inter/), [Instrument Serif](https://fonts.google.com/specimen/Instrument+Serif), [JetBrains Mono](https://www.jetbrains.com/lp/mono/).
- Icons via [Bootstrap Icons](https://icons.getbootstrap.com/) and [FontAwesome](https://fontawesome.com).

© 2026 Sritanya Suresh Andal. All content rights reserved.

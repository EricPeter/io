# Personal site

Source for my personal website — built with [Quarto](https://quarto.org), deployed automatically to GitHub Pages on every push to `main`.

**Live:** https://ericpeter.github.io/io/

## Structure

| File | Content |
|------|---------|
| `index.qmd` | Home page — hero, experience, selected projects, publications, education, skills, contact |
| `projects.qmd` | Full AI engineering portfolio (20 projects) + earlier research/academic projects |
| `publications.qmd` | Full publication list |
| `styles.css` | Site-wide styling (flat/monochrome, single narrow column) |
| `_quarto.yml` | Site config — nav, theme, footer |
| `images/` | Favicon and other static images |
| `Eric_Peter_Wairagala_CV.pdf` | Downloadable CV, linked from the nav bar and hero |

The [`ai-projects`](https://github.com/EricPeter/ai-projects) portfolio referenced from `projects.qmd` lives in its own repo and isn't part of this one.

## Preview locally

```bash
quarto preview
```

## Build

```bash
quarto render
```

Output goes to `_site/`.

## Deploy

Deployment is automatic: pushing to `main` triggers [`.github/workflows/publish.yml`](.github/workflows/publish.yml), which renders the site with Quarto and publishes it to the `gh-pages` branch. No manual deploy step needed.

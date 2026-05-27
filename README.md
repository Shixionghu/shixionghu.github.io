# Shixiong Hu Academic Website

This repository contains two layers:

- `index.html`, `styles.css`, `script.js`, and `assets/`: the current reviewed static site.
- `_quarto.yml` and `*.qmd`: the Quarto source version for a GitHub Pages workflow.

## Local Quarto Preview

Install Quarto from <https://quarto.org/docs/download/>. Then run:

```bash
quarto preview
```

Render the full site:

```bash
quarto render
```

The Quarto project is configured to render into `docs/`, which is the simplest GitHub Pages publishing source for this site.

## GitHub Pages Setup

1. Create a GitHub repository, for example `academic-website`.
2. Push this project to GitHub.
3. On GitHub, open `Settings` -> `Pages`.
4. Set `Source` to `Deploy from a branch`.
5. Set `Branch` to `main` and folder to `/docs`.
6. Save. The site will publish at `https://<username>.github.io/<repository>/`.

## Update Workflow

Edit the `.qmd` files, then run:

```bash
quarto render
git add .
git commit -m "Update academic website"
git push
```

GitHub Pages will serve the updated rendered files from `docs/`.

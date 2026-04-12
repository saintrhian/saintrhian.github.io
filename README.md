# Lovers, Beekeepers, Epilepsy, Fainting, and the Plague

This repository is structured as a Jekyll site for GitHub Pages.

## Site structure

- `_config.yml`: GitHub Pages / Jekyll configuration
- `_layouts/`: shared page and post templates
- `assets/css/style.scss`: global styling
- `_posts/`: dated journal entries
- `index.html`: homepage and post list
- `about.md`: static about page

## Publishing with GitHub Pages

This repo includes a GitHub Actions workflow at `.github/workflows/pages.yml` that builds
the Jekyll site and deploys it to GitHub Pages on every push to `main`.

To enable it in GitHub:

1. Open `Settings`.
2. Open `Pages`.
3. Under `Build and deployment`, choose `GitHub Actions`.

The site will publish at `https://saintrhian.github.io`.

## Local development

Install the Jekyll dependencies:

```bash
bundle install
```

Then run the local server:

```bash
bundle exec jekyll serve
```

## Adding new entries

Create new Markdown files in `_posts/` using this filename format:

```text
YYYY-MM-DD-title.md
```

Each post should start with front matter like this:

```yaml
---
title: New Entry
date: 2026-04-11 09:00:00 -0500
---
```

Then write the body in Markdown.

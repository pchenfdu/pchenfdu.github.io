# Ping Chen Academic Homepage

This repository hosts the source for Prof. Ping Chen's academic homepage built on top of the [al-folio](https://github.com/alshedivat/al-folio) Jekyll theme.

## Quick Start

```bash
bundle install
npm install -g purgecss
bundle exec jekyll serve
```

The site will be available at `http://localhost:4000` and will automatically pick up changes to content in `_pages/`, `_data/`, `_projects/`, `_news/`, and `_bibliography/`.

## GitHub Pages Deployment

The repository is already wired to deploy to GitHub Pages via GitHub Actions:

1. Ensure the repository is named `leonidwang.github.io` (or `<username>.github.io` for your account).
2. In **Settings -> Actions -> General**, set *Workflow permissions* to **Read and write** and enable Actions for this repository.
3. Push changes to `master` (or `main`). The included workflow `.github/workflows/deploy.yml` will build the site and publish the generated `_site/` output to the `gh-pages` branch.
4. In **Settings -> Pages**, choose **Deploy from a branch**, select the `gh-pages` branch, and the `/ (root)` folder. Save the settings.
5. Wait for the `Deploy site` workflow and the `pages-build-deployment` workflow to finish. The live site will be available at `https://leonidwang.github.io`.

## Customization Checklist

- Update `_config.yml` with analytics IDs or additional metadata as needed.
- Replace `assets/img/prof_pic.jpg` with your preferred profile image (square or portrait).
- Add or remove news items in `_news/` to control the announcement feed.
- Manage bibliography entries in `_bibliography/papers.bib` to keep publications current.
- Projects showcased on the portfolio page live under `_projects/`.

## Folder Overview

- `_pages/` -- top-level pages (About, Projects, Publications, News, Teaching, CV).
- `_data/` -- structured data such as the CV, social links, and navigation metadata.
- `_news/` -- announcement snippets surfaced on the About page and News page.
- `_projects/` -- feature pages backing the Projects grid.
- `_sass/` -- SCSS theme overrides; `_sass/_themes.scss` contains the customized color palette.

Feel free to adjust the layouts, add blog posts under `_posts/`, or extend the theme with additional Jekyll plugins if required.

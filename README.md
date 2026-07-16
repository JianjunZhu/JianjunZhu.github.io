# Jianjun Zhu · Academic Homepage

[![Website](https://img.shields.io/badge/website-jianjunzhu.github.io-087e8b)](https://jianjunzhu.github.io)
[![GitHub Pages](https://github.com/JianjunZhu/JianjunZhu.github.io/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/JianjunZhu/JianjunZhu.github.io/deployments)
[![License](https://img.shields.io/badge/license-MIT-1e4d70)](LICENSE)

Source code for [jianjunzhu.github.io](https://jianjunzhu.github.io), the academic homepage of **Jianjun Zhu (朱建軍)**, Assistant Professor at Macau University of Science and Technology.

The site presents research in medical image computing, computer-assisted intervention, and interventional surgical robotics. It is built with Jekyll and GitHub Pages on top of the [Academic Pages](https://academicpages.github.io/) theme.

## Highlights

- Research-focused homepage with a concise academic introduction.
- Dedicated publication, teaching, and curriculum vitae pages.
- Responsive layout for desktop, tablet, and mobile screens.
- Light and dark themes using the existing theme switcher.
- Search and social metadata for Google, LinkedIn, and other link previews.
- Optimized WebP portrait for a faster first-page load.
- Sample theme content excluded from the production build and sitemap.

## Repository Structure

| Path | Purpose |
| --- | --- |
| `_pages/about.md` | Homepage content, research themes, grants, and recruitment information |
| `_pages/publications.html` | Selected-publication catalog |
| `_publications/` | Structured publication records used by the catalog |
| `_pages/cv.md` | Academic appointments, education, funding, awards, and service |
| `_pages/teaching.html` | Teaching overview |
| `_teaching/` | Individual course records |
| `_data/navigation.yml` | Main navigation links and order |
| `_config.yml` | Site identity, author profiles, SEO, collections, and build settings |
| `_sass/_personal.scss` | Custom visual system and responsive component styles |
| `images/profile-720.webp` | Optimized on-page portrait |
| `images/profile-social.jpg` | Social-preview image |

Do not edit `_site/` directly. Jekyll regenerates it during every build.

## Updating Content

### Homepage and CV

Edit `_pages/about.md` for the homepage and `_pages/cv.md` for the curriculum vitae. Keep research facts, dates, contact details, and funding information synchronized across both pages.

### Publications

Add one Markdown file to `_publications/` for each selected publication:

```yaml
---
title: "Publication title"
collection: publications
category: manuscripts # or conferences
permalink: /publication/short-name
date: 2026-01-01
venue: "Journal or conference"
paperurl: "https://doi.org/..."
citation: "Full citation"
---
```

The publications page sorts these records by date. The Google Scholar link remains the source for the complete and most current bibliography.

### Teaching

Add or update course records in `_teaching/`. Navigation labels and ordering are controlled by `_data/navigation.yml`.

## Local Development

Ruby 3.2 or newer and Bundler are recommended.

```bash
git clone https://github.com/JianjunZhu/JianjunZhu.github.io.git
cd JianjunZhu.github.io
bundle config set --local path vendor/bundle
bundle install
bundle exec jekyll serve --livereload
```

Open `http://localhost:4000` in a browser. Jekyll rebuilds the site when a source file changes.

Create a production build without starting a server:

```bash
JEKYLL_ENV=production bundle exec jekyll build
```

The generated site is written to `_site/`.

## Docker Preview

With Docker Desktop installed:

```bash
docker compose up --build
```

The preview is available at `http://localhost:4000`. Stop it with `Ctrl+C`.

## Validation Checklist

Before publishing:

1. Run `bundle exec jekyll build` and confirm that it finishes without errors.
2. Review the homepage at desktop and mobile widths.
3. Test the light/dark theme switcher.
4. Check the navigation, publication links, email address, Google Scholar, and ORCID links.
5. Confirm that new pages have a title and description in their front matter.

## Deployment

GitHub Pages publishes the site from this repository. After reviewing changes locally, commit them and push the `master` branch:

```bash
git add .
git commit -m "Update academic homepage"
git push origin master
```

Deployment status is available in the repository's [Deployments](https://github.com/JianjunZhu/JianjunZhu.github.io/deployments) view.

## Credits and License

The site is based on [Academic Pages](https://github.com/academicpages/academicpages.github.io), a fork of the [Minimal Mistakes](https://mademistakes.com/work/minimal-mistakes-jekyll-theme/) Jekyll theme. Repository code remains available under the [MIT License](LICENSE).

# Laura Blog

A Jekyll blog for `laura.kassovic.com`, using the Chirpy theme via `theme` and GitHub Pages deployment.

## Local preview

Install Ruby and Bundler, then run:

```bash
bundle install
bundle exec jekyll serve
```

Open:

```text
http://127.0.0.1:4000
```

## Writing posts

Add Markdown files in `_posts` using this filename format:

```text
YYYY-MM-DD-title-slug.md
```

Example front matter:

```yaml
---
title: "My post title"
date: 2026-05-17
categories: [Gradle]
tags: [gradle, build-systems]
---
```

## Customize

Edit `_config.yml` for:

- site title
- tagline
- description
- social links
- avatar image
- analytics

Replace `assets/img/avatar.png` and `assets/img/social-preview.png` later with real images.

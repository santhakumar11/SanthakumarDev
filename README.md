# Santhakumar's personal blog

A responsive Jekyll blog hosted on GitHub Pages. Blog entries are Markdown files in `_posts/`.

## Write a post

Create a file in `_posts/` named `YYYY-MM-DD-your-title.md`:

```markdown
---
layout: post
title: "Your post title"
date: 2025-03-01
tags: [notes]
excerpt: "A short description shown on the home page."
---

Write your post in Markdown.
```

Commit and push to `main`; the GitHub Actions workflow builds and deploys the site.

## Publish on GitHub Pages

In the repository settings, open **Pages** and select **GitHub Actions** as the build and deployment source. The workflow at `.github/workflows/pages.yml` publishes subsequent pushes to `main`.

The site URL is configured for `https://santhakumar11.github.io/SanthakumarDev`. If the repository name or GitHub account changes, update `url` and `baseurl` in `_config.yml`.

## Preview locally

With Ruby and Bundler installed:

```sh
bundle install
bundle exec jekyll serve
```

Then open `http://127.0.0.1:4000/SanthakumarDev/`.

# Augustus Shen — personal website

A clean, academic personal site built with [Jekyll](https://jekyllrb.com/).
No themes, no plugins — just plain Jekyll, so it builds identically on this Mac
and on GitHub Pages.

## Structure

```
_config.yml              Site settings, contact links, nav identity
index.html               Home / about (hero + interests + latest notes)
research.md              Research page
blog.md                  Notes index (lists _posts)
_posts/                  Blog/research-note entries (YYYY-MM-DD-title.md)
_layouts/                default · page · post
_includes/               head · nav · footer
assets/css/main.css      The entire theme (one stylesheet)
assets/img/              avatar.svg, favicon.svg  ← replace avatar with a photo
cv/                      Augustus_Shen_CV.pdf
.github/workflows/       GitHub Pages deploy (GitHub Actions)
```

## Run it locally

The system Ruby (2.6) already has a compatible Jekyll installed for this project.
Make sure the user gem bin is on your PATH, then serve:

```bash
export PATH="$HOME/.gem/ruby/2.6.0/bin:$PATH"
jekyll serve --livereload
# open http://127.0.0.1:4000
```

(If you ever install a modern Ruby via Homebrew, `bundle install && bundle exec
jekyll serve` will work too — the Gemfile auto-skips the legacy pins.)

## Add a note

Create `_posts/2026-07-01-my-title.md`:

```markdown
---
layout: post
title: "My title"
date: 2026-07-01
tags: [experiment, kinesin-14]
---

Write in Markdown here.
```

It shows up automatically on the home page and the Notes index.

## Deploy to GitHub Pages

1. Create a repo. For a personal site at `https://<username>.github.io`, name the
   repo exactly `<username>.github.io` and keep `baseurl: ""` in `_config.yml`.
   For a project site at `https://<username>.github.io/<repo>`, set
   `baseurl: "/<repo>"`.
2. Push this folder to the `main` branch.
3. In the repo: **Settings → Pages → Build and deployment → Source: GitHub Actions**.
4. The workflow in `.github/workflows/jekyll.yml` builds and deploys on every push.

## To-do / personalize

- [ ] Replace `assets/img/avatar.svg` with a real photo (`avatar.jpg`) and update
      the `src` in `index.html`.
- [ ] Fill in `social:` links in `_config.yml` (GitHub, Scholar, ORCID, LinkedIn) —
      they appear in the footer automatically once non-empty.
- [ ] Re-export `cv/Augustus_Shen_CV.pdf` whenever your CV changes.

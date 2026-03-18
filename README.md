# rydela.github.io

Portfolio site for Ryan Arias Delafosse, built on Jekyll Minimal theme.

## Site Structure

- `/` — project archive, reverse-chronological (`index.md`)
- `/about/` — bio, focus areas, contact (`about.markdown`)
- `/projects/<slug>/` — individual project pages from `_projects/`

## Content Model

Projects live in `_projects/*.md` with front matter fields:

- `title`
- `slug`
- `year`
- `section`
- `summary`
- `methods`
- `outcome`
- `status`
- `image` (optional)
- `organization`
- `links`

Each project page follows a **Problem / Work / Delivery** narrative structure in the body.

## Design

- Jekyll Minimal theme with custom overrides in `_sass/jekyll-theme-minimal.scss`
- 270px fixed sidebar (identity anchor) + 600px content column
- Noto Sans 16px / 1.65 line-height, #444 body text
- Navigation (`_includes/header.html`) and contact links in sidebar
- Shield.io badges for project links

## Local Preview

```bash
export HOME="$PWD/.home"
export GEM_HOME="$PWD/.local-gems"
export GEM_PATH="$PWD/.local-gems"
export PATH="$PWD/.local-gems/bin:$PATH"
bundle install
bundle exec jekyll serve
```

Note: changes to `_config.yml` require a server restart to take effect.

## Local-Only Files

The following are intentionally ignored and should not be committed:

- build output and caches (`_site`, `.sass-cache`, `.jekyll-cache`, `.jekyll-metadata`)
- local Ruby/Bundler environment (`.home`, `.local-gems`, `.bundle`, `.vendor`)
- local helper files (`scripts`, `.DS_Store`, `*.log`)

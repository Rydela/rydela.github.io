# rydela.github.io

Portfolio site for Ryan Arias Delafosse, built on Jekyll Minimal theme.

## Site Structure

- `/` chronological project narrative (`index.md`)
- `/portfolio/` compact chronological table (`portfolio.md`)
- `/projects/<slug>/` individual project pages from `_projects/`

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
- `image`
- `organization`
- `links`

## Local Preview

```bash
export HOME="$PWD/.home"
export GEM_HOME="$PWD/.local-gems"
export GEM_PATH="$PWD/.local-gems"
export PATH="$PWD/.local-gems/bin:$PATH"
bundle install
bundle exec jekyll serve --livereload
```

## Local-Only Files

The following are intentionally ignored and should not be committed:

- build output and caches (`_site`, `.sass-cache`, `.jekyll-cache`, `.jekyll-metadata`)
- local Ruby/Bundler environment (`.home`, `.local-gems`, `.bundle`, `.vendor`)
- local helper files (`scripts`, `.DS_Store`, `*.log`)

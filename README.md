# maosboo.com

Personal writing site for Maike Osborne.

## Tech Stack

- **Static site generator:** Jekyll ~4.3
- **Theme:** [Jekyll Curate](https://www.zerostatic.io/theme/jekyll-curate/) by Zerostatic, with Adobe Typekit fonts
- **Plugins:** `jekyll-environment-variables`, `jekyll-paginate`

## Deployment

The site is deployed via **Netlify**, configured in `netlify.toml`:

- **Build command:** `jekyll build`
- **Publish directory:** `_site`
- **Ruby version:** 3.2.3
- **Custom domain:** maosboo.com (configured in Netlify dashboard, linked to github account)

Netlify automatically rebuilds on every push to the repo.

## Key Files

- `_config.yml` — Main site configuration (colours, fonts, footer text, etc.)
- `netlify.toml` — Netlify build settings
- `collections/_posts/` — Blog posts
- `pages/` — Static pages
- `_data/` — Authors, contact info, menus, social links
- `assets/` — Images, CSS, JS, fonts

## Notes

- The `Gemfile` does **not** include `github-pages` gem — this is not a GitHub Pages-compatible setup, which is another reason GitHub Pages builds fail.
- Copyright text is set in `_config.yml` under `bottom.copyright_text`.

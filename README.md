# picolimpid.github.io

Personal website of Hanqi (Andy) Mao — https://picolimpid.github.io

Built with [Jekyll](https://jekyllrb.com/) and the [al-folio](https://github.com/alshedivat/al-folio) theme, starting from the layout of [melissashi2002.github.io](https://github.com/melissashi2002/melissashi2002.github.io).

## Editing

- Bio and profile box: `_pages/about.md` (photo: `assets/img/profile.jpg`)
- News items: `_news/*.md`
- Projects: `_pages/projects.md`
- Navbar links: `_includes/header.liquid`
- Name, email, social IDs: `_config.yml`

Pushing to `main` runs `.github/workflows/deploy.yml`, which builds the site and publishes it to the `gh-pages` branch.

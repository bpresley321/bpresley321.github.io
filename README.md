# Personal site (Jekyll + GitHub Pages)

## Publish it
1. Create a GitHub repo named `<your-username>.github.io` (public).
2. Upload everything in this folder to it.
3. Repo Settings > Pages > Source: "Deploy from a branch", branch `main`, folder `/ (root)`.
4. After a minute or two the site is live at `https://<your-username>.github.io`.

## Theme
This site uses the Minimal theme (`theme: jekyll-theme-minimal` in `_config.yml`).
Minimal only provides one layout, so `_layouts/page.html` and `_layouts/post.html` add a Home link and titles on top of it.
To switch to another built-in GitHub Pages theme, change the `theme:` line; other GitHub-hosted themes use `remote_theme: owner/repo` plus `jekyll-remote-theme` under `plugins:`. Layout names differ between themes, so ask Claude to adjust.

## Add content
- **Post:** new file in `_posts/` named `YYYY-MM-DD-title.md`.
- **Page:** new `.md` file in the top folder; link to it from `index.md`.
- **Tool:** drop an HTML file in a `tools/` folder and link it from `tools.md`.

## Preview locally (optional)
`bundle install` then `bundle exec jekyll serve`, and open http://localhost:4000.

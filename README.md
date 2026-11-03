# Personal site (Jekyll + GitHub Pages)

## Publish it
1. Create a GitHub repo named `<your-username>.github.io` (public).
2. Upload everything in this folder to it.
3. Repo Settings > Pages > Source: "Deploy from a branch", branch `main`, folder `/ (root)`.
4. After a minute or two the site is live at `https://<your-username>.github.io`.

## Change the theme
Edit the `theme:` line in `_config.yml`.
- Built-in GitHub Pages themes use a name, e.g. `theme: minima` or `theme: jekyll-theme-cayman`.
- Any other theme hosted on GitHub: replace `theme:` with
  `remote_theme: owner/repo-name` and add `- jekyll-remote-theme` under `plugins:`.

Themes differ in which layouts they provide. If a page looks wrong after a swap, the usual fix is the `layout:` line at the top of that file.

## Add content
- **Post:** new file in `_posts/` named `YYYY-MM-DD-title.md`.
- **Page:** new `.md` file in the top folder; add it to `header_pages` in `_config.yml` to show it in the menu.
- **Tool:** drop an HTML file in a `tools/` folder and link it from `tools.md`.

## Preview locally (optional)
`bundle install` then `bundle exec jekyll serve`, and open http://localhost:4000.

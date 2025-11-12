# Research Site (Jekyll on GitHub Pages)

This is a minimal, ready-to-deploy personal research website using Jekyll + the Minimal Mistakes theme.

## Quick start

1. **Create a repository** named `<your-username>.github.io` (for a user site).
2. Download this starter and put its contents in the repo root.
3. Commit & push. In your repo settings, ensure **Pages** is enabled (it should auto-deploy).
4. Edit `_config.yml` (title, author, URLs).
5. Update `_data/publications.yml` with your publications.
6. Replace the placeholder YouTube `{% include youtube.html id="VIDEO_ID" %}` in `index.md` with a real ID or remove it.
7. To embed a PDF deck on a page, use `{% include pdf_embed.html src="/assets/slides/mydeck.pdf" %}` and add the file to `assets/slides/`.

### Local preview (optional)

- Install Ruby and Bundler, then run:
  ```bash
  bundle install
  bundle exec jekyll serve
  ```
- Visit <http://localhost:4000>.

## Notes

- For a **project site** instead of a user site, set `baseurl: "/reponame"` in `_config.yml` and access it at `https://<username>.github.io/<reponame>/`.
- GitHub Pages builds are static; avoid plugins not supported by GitHub Pages.
- If you don't need local builds, you can omit the `Gemfile`.

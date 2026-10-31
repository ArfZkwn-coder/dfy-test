# Kopi Notes

Documentation site built with [Docsify](https://docsify.js.org/). There is no build step: the pages in `docs/` are rendered in the browser.

## Working locally

Serve the `docs/` folder with any static server, for example:

```bash
npx docsify-cli serve docs      # or: python -m http.server --directory docs 3000
```

Pages are Markdown files in `docs/`, listed in `docs/_sidebar.md`. Pictures go in `docs/img/` and are linked relative to the page. Keep `docs/.nojekyll`: without it GitHub Pages hides `_sidebar.md`.

## Deploying

Pushing to `main` publishes the site. Set it up once in the GitHub repo: **Settings → Pages → Source: Deploy from a branch**, branch `main`, folder `/docs`.

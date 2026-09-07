# selfdriven Shop — GitHub Pages assets

Ready-to-publish HTML, CSS, images and the existing Emergence designer. No npm, Python, Jekyll or build step is needed. Edit the HTML and CSS directly.

## Publish using your existing repository

1. Extract this ZIP.
2. Back up your existing `docs/CNAME` if it exists. Replace the repository's `docs` folder with the included `docs` folder; keep unrelated repository files and the `merch` artwork directory. Remove the old `docs/index.md`, `docs/pages` and `docs/_layouts` as part of this replacement so there are no stale source files.
3. Restore the existing `CNAME` into the new `docs` folder when retaining your current custom domain. The original repository contains `shop.selfdriven.foundation`, although the requested public address is `selfdriven.shop`. Retain the domain currently configured in GitHub Pages; do not change it just to install the redesign. No CNAME is bundled, so this also works for a github.io project URL.
4. Commit and push the files, including `docs/.nojekyll`.
5. In the repository, open **Settings → Pages**. Choose **Deploy from a branch**, select your publishing branch (typically `main`), and choose **/docs**. Save.
6. Once GitHub reports the deployment complete, open the published address.

If you already publish from `/docs`, keep that setting. If publishing from the repository root instead, copy the *contents* of `docs` to the root, including `.nojekyll`, and select `/(root)`.

## Included pages

- `/` — redesigned storefront
- `/merch/custom/` — ordering instructions
- `/merch/custom/templates/` — all original Screenlab template links
- `/merch/custom/by-selfdriven/` — special orders and artwork resources
- `/merch/custom/emergence/` — existing interactive wordmark designer
- `/merch/custom/orders-summary/` — existing order reference page

Internal links and asset paths are relative and include directory trailing slashes. They work under either a custom domain or a github.io repository subpath. Original external Screenlab checkout, artwork and community links are preserved. Fonts load from Google Fonts with local system fallbacks. No credentials or ChatGPT hosting configuration are included.

## Editing

- Homepage: `docs/index.html`
- Shared styling: `docs/assets/css/style.css`
- Images and logos: `docs/assets/`
- Other pages: the relevant directory's `index.html`

The navigation and footer are in each HTML page; update each copy when changing shared links.

## Optional local preview

From the extracted folder, run `python3 -m http.server 8000 --directory docs`, then open http://localhost:8000. Python is only for this optional preview, not deployment.

## Verification

All included local page and asset references and fragment targets were checked. The ZIP's integrity was checked. Browser visual testing and a GitHub deployment have not been performed for this package.

GitHub instructions: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
Static publishing: https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site

Original repository: https://github.com/selfdriven-engagement/selfdriven-shop
The original repository LICENSE is included.

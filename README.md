# Hydro-Sense website

Single-page website for Hydro-Sense Technologies. The site is served by `index.html`; images are stored in `assets/`.

## Test locally

From the repository folder, run:

```sh
python3 -m http.server 8000
```

Open:

- Public view: <http://localhost:8000/>
- Editor view: <http://localhost:8000/?edit=1>

## Editing workflow

The in-page editor requires a fine-grained GitHub token with access to this repository and `Contents: Read and write`. Each editor should use their own token. Tokens remain in the browser session unless **Remember on this device** is explicitly selected.

In the editor's **Publish to GitHub** settings, use:

- Owner: `Hydrosense-technologies`
- Repository: `hydrosense-website`
- Branch: `experimental`
- Path: `index.html`

Publishing from the editor commits the cleaned page to `experimental`. Test those changes locally and open a pull request from `experimental` into the production publishing branch when the update is ready for review.

## Publishing safety

The `?edit=1` parameter protects editing controls only; it does not make a deployed website private. Treat GitHub Pages output as public and do not publish confidential material.

Configure GitHub Pages to deploy only from the approved production branch, not from `experimental`.

# sevmorris.github.io

The landing page for my macOS apps, served at <https://sevmorris.github.io/>.

Hand-written HTML in `docs/`, served by GitHub Pages from `/docs` on `main`, with `.nojekyll` and no build step. Each app keeps its own page at `sevmorris.github.io/<App>/`; this page links to them.

`docs/icons/` holds 256 px copies of each app's icon. Download buttons link to each repository's latest release, and a small script swaps in the DMG's direct URL and the current version from the GitHub API when it can, so a release needs no edit here. A new app, or a new icon, does.

To preview, open `docs/index.html`, or serve the folder:

```bash
python3 -m http.server 8765 --directory docs
```

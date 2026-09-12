# WoW: Forever Talent Calculator

Static GitHub Pages version.

## Publish with GitHub Pages

1. Create a GitHub repository.
2. Upload these files to the repository root:
   - `index.html`
   - `forever_talents.json`
   - `.nojekyll`
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose:
   - **Source:** Deploy from a branch
   - **Branch:** `main`
   - **Folder:** `/ (root)`
5. Save.

GitHub will publish the site at a URL similar to:

`https://YOUR_USERNAME.github.io/YOUR_REPOSITORY/`

## Updating talents

Edit `forever_talents.json` and commit the new version.

The page also has a Data Editor. **Apply Locally** only stores changes in your
current browser. Use **Download JSON** to export those changes, then replace
`forever_talents.json` in the GitHub repository and commit it.

## Local preview

Because browsers usually block `fetch()` from `file://` pages, do not simply
double-click `index.html` if you want to test the JSON loading locally.

From this folder, run:

```bash
python -m http.server 8000
```

Then open:

`http://127.0.0.1:8000/`

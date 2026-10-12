# Algae Bioreactor 2.0 viewer

Static site: `index.html`, `meta.json` and six `*.txt` data files (gzip-compressed geometry, base64-encoded). Keep all files in the same folder.

## Run locally
The page loads its data with `fetch`, so it must be served over http (opening `index.html` by double-click will not load the model):

    python3 -m http.server 8000
    # then open http://localhost:8000

## GitHub Pages
Push this folder to a repository, then Settings → Pages → Deploy from branch (root).

## Vercel
`vercel deploy` from this folder, or import the repository in the Vercel dashboard. No build step and no framework preset needed ("Other").

Requires a browser with WebGL 2 (all current desktop and mobile browsers).

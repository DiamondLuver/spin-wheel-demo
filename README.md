# Sméan Spin Wheel

Single-page static spin-to-win wheel. No build step — `index.html` plus `assets/` is the whole site.

## Run locally

```sh
python3 -m http.server 8000
```

Then open http://localhost:8000. Open the file directly with `file://` only for a quick look; a server matches how GitHub Pages serves it.

## Deploy

Pushing to `main` triggers `.github/workflows/deploy.yml`, which publishes the repository root to GitHub Pages. Enable it once under **Settings → Pages → Source → GitHub Actions**.

Asset paths are relative and lowercase, so the site works from a project subpath (`/<repo>/`) as well as a custom domain.

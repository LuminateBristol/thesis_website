
# Thesis Supplementary (MkDocs + Material)

This repository hosts a wiki-style site for thesis supplementary material (summaries, figures, videos, simulator docs, and SWOOT notes) built with **MkDocs** and **Material for MkDocs**, and deployed to **GitHub Pages**.

## Quick start (local)

```bash
python -m venv .venv && source .venv/bin/activate  # On Windows: .venv\Scripts\activate
pip install -r requirements.txt
mkdocs serve
```
Open http://127.0.0.1:8000/

## Deploy (GitHub Pages via Actions)
1. Push this repo to GitHub.
2. In **Settings → Pages**, set **Source** to **GitHub Actions**.
3. The provided workflow will build and deploy automatically on push to `main`.

## Structure
- `docs/` — content (Markdown).
- `code/` — optional Python code to auto-document with `mkdocstrings`.
- `.github/workflows/deploy.yml` — builds and deploys to Pages.

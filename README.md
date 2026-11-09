# Guided Troubleshooter landing site

Static site (HTML/CSS/JS, no build step) for the Guided Troubleshooter widget.

- `/` landing page with demo video, live demo, free vs full comparison, FAQ
- `/editor/` free builder (10 steps, "Powered by" credit, inline embed code only)
- `/privacy/` privacy page

Placeholders to replace before launch:
- `#GUMROAD_LINK` → the Gumroad product URL (all pages, and `window.GT_UPGRADE_URL` in `/editor/`)
- `https://guided-troubleshooter.onrender.com` → the final domain (canonical, OG, sitemap, robots)

Generated from `/workspace/troubleshooter-product/src/landing/gen.py` (run with `SITE_URL=https://your.domain python3 gen.py`).

Local preview: `python3 -m http.server 8000`, then open http://localhost:8000/

## Deploy (Render static site)
New → Static Site (or Blueprint with `render.yaml`), publish directory `.`, build command empty.

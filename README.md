# Zoom Casa — Partner Intake

Single-page partner / agent / lender / homeowner intake form. Mirrors the design system of [zoomcasa-netsheet](https://github.com/Balinti/zoomcasa-netsheet).

- **Live:** https://partners.zoomcasa.com
- **Stack:** Single `index.html`, React 18 via CDN, Babel standalone — no build step.
- **Submissions:** POST to the n8n partner webhook (see `PARTNER_WEBHOOK` constant in `index.html`).
- **Hosting:** GitHub Pages, custom domain via `CNAME`.

## Local preview

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy

Push to `main` — GitHub Pages serves the root `index.html` automatically.

## Configuration

The n8n webhook URL is the constant `PARTNER_WEBHOOK` near the top of `<script type="text/babel">` in `index.html`.


# Deflectly — Static Site

This folder contains a production-ready static site you can deploy on **Cloudflare Pages** with your domain.

## Files
- `index.html` — main landing page
- `case-study.html` — live case study
- `privacy.html`, `terms.html` — basic legal pages
- `assets/logo.svg`, `assets/favicon.svg` — brand assets

## Quick Deploy (Cloudflare Pages)
1) Push these files to a new GitHub repo (e.g., `deflectly-site`).  
2) In Cloudflare → **Pages** → *Create project* → **Connect to Git** → choose the repo.  
3) **Build settings:** Framework = None (static); output directory = `/`  
4) After deploy, open Pages → **Custom domains** → add your domain (e.g., `deflectly.com`).  
5) Cloudflare will set DNS + SSL automatically.

## Wire your tools
- **Calendly:** In `index.html` under `#book`, paste your embed.
- **Tally:** Paste your intake form embed in the Pilot card.
- **Stripe:** Create a Payment Link for "Start pilot" and replace `href="#"` on the buttons.
- **Chat (optional):** Add Tidio/Intercom/Zendesk snippet before `</body>`.

## Branding tweaks
- Colors are Tailwind's `brand-*` indigo scale; change in the `tailwind.config` object in the `<head>`.
- Replace the logo SVG in `assets/logo.svg` if you want a custom mark.
- Update OpenGraph image at `/og-image.png` for rich link previews.

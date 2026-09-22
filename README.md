# desdemonatides-site

Static brand landing page for SLF's **DesdemonaTides** shop at
**desdemonatides.com** — a link-in-bio front door pointing at the Etsy shop and
Instagram. Pure HTML + CSS, no frameworks, no build step. Will deploy as flat
files on GitHub Pages with Porkbun DNS (same recipe as shellback-studio-site).

**Status: local scaffold only — NOT public.** SLF sign-off on look/feel is the
launch gate (D4 in `SCOPING_NOTES.md`): no GitHub remote, no Pages enable, no
DNS changes until it clears.

## Local preview

Open `index.html` in a browser. That's the whole deploy story for a static
page.

(Optional: run `python -m http.server` in this folder and visit
http://localhost:8000 — same result.)

## Files

- `index.html` — the entire page (styles inline in `<head>`)
- `assets/PLACEHOLDER.md` — where SLF's banner/avatar images go

## LAUNCH CHECKLIST

0. PREVIEW (current state): GitHub Pages draft URL shared with SLF for
   sign-off — page carries noindex; remove the noindex meta at public launch.
1. **SLF sign-off on look/feel** [GATE — nothing below happens before this]
2. Add banner/avatar assets (see `assets/PLACEHOLDER.md`)
3. Create GitHub repo + push
4. Enable GitHub Pages
5. Porkbun DNS: 4 apex A records for GitHub Pages
   (185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153)
   + www CNAME -> `<user>.github.io`
6. Verify HTTPS + domain
7. Confirm Porkbun auto-renew for the domain
   (registered 2026-06-30, expires 2027-06-30)

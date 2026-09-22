# SCOPING NOTES — desdemonatides-site

Static brand landing page (link-in-bio) for SLF's DesdemonaTides shop at
desdemonatides.com. Scaffolded 2026-09-22. **Local only — nothing public.**

## Decisions

- **D1 — Purpose:** SLF brand landing (link-in-bio) at desdemonatides.com;
  customer-facing.
- **D2 — Launch platforms:** Etsy shop
  (https://www.etsy.com/shop/DesdemonaTides) + Instagram @desdemonatides
  (https://www.instagram.com/desdemonatides/); others pending SLF. Slot for
  more buttons marked with an HTML comment in `index.html`.
- **D3 — Assets pending from SLF/Etsy page:** shop banner (Etsy) and avatar
  (Instagram). Save locations documented in `assets/PLACEHOLDER.md`.
- **D4 — LAUNCH GATE:** SLF sign-off on look/feel BEFORE any DNS / Pages /
  public anything. No GitHub remote, no Pages enable, no DNS edits until D4
  clears.
- **D5 — Accounts:** user holds the Porkbun + Purelymail logins; deploy recipe
  replays shellback-studio-site (extracted-repo + GitHub Pages + Porkbun DNS
  pattern, deployed 2026-09-11).
- **D6 — Follow-up:** slicer subdomain `slice.desdemonatides.com` (CNAME) after
  the page launches — points at the cuff-slicer-app GitHub Pages URL.

## Domain facts

- **Domain:** desdemonatides.com
- **Registrar/DNS:** Porkbun (Porkbun nameservers)
- **Registered:** 2026-06-30 · **Expires:** 2027-06-30 (**confirm auto-renew**
  — launch checklist item 7)
- **DNSSEC:** off

## Process note

Build locally only; no remote, no Pages, no DNS changes until D4 clears. Git
handled by the operator (local commits only at most). The monorepo `.gitignore`
carries `desdemonatides-site/` (mirroring the `shellback-studio-site/` pattern)
so the folder is never accidentally committed to the dev monorepo.

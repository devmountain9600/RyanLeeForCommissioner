# Write In Ryan Lee — Campaign Website

## Project Overview
One-page campaign website for Ryan Lee, a **write-in candidate** for **County Commissioner, District 2, Costilla County, Colorado** (2026 election).
- **Brand**: Mardi Gras colors (purple, green, gold) — a nod to Ryan's Louisiana roots; the office is in Colorado.
- **Logo**: `RyanLeeLogo.jpg` ("Write In ✓ Ryan Lee")
- **Candidate photo**: `RyanLee.jpg`

## Hosting & Services
- **Hosting**: Cloudflare Pages (auto-deploys from GitHub on push to `main`)
- **Repo**: https://github.com/devmountain9600/RyanLeeForCommissioner
- **Domain**: `writeinryanlee.com` (purchased at GoDaddy)
- **DNS**: Cloudflare (nameservers migrated from GoDaddy to Cloudflare)
- **Donations**: GoDaddy PayLink at `https://pay.writeinryanlee.com/donate` (CNAME `pay` → `paylinks.commerce.godaddy.com` in Cloudflare DNS) — same pattern as taylorforsheriff.org.
- **Build**: none — static site, Cloudflare serves repo root as-is

## Deploy Workflow
1. Edit files locally.
2. `git add -A && git commit -m "..." && git push`
3. Cloudflare Pages auto-builds and deploys within ~1 minute.

## Tech Stack
- Plain HTML/CSS, single `index.html` file (everything inline)
- Google Fonts (Oswald + Source Sans 3)
- No build step, no JavaScript framework
- Images stored in the repo root (`RyanLeeLogo.jpg`, `RyanLee.jpg`)

## Content TODO (still placeholder in index.html — marked with [EDIT])
- Ryan's real bio (About section)
- Real campaign priorities (Issues section)
- Contact email / phone / social links
- **Verify with Costilla County Clerk**: exact write-in voting steps + that Ryan filed the Colorado write-in affidavit of intent by the deadline
- **Confirm** the required campaign-finance disclaimer wording

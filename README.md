# Project Excavation

Free LEGO set sorting tracker — dig every brick out of the pile, track progress, stream-friendly.

A sister project to [Project Chrysalis](https://chrysalis.buildbeyondbelief.com) from [Build Beyond Belief](https://buildbeyondbelief.com).

**Live site:** https://excavation.buildbeyondbelief.com

## What it is

Single-page app (`index.html` only). No build step, no backend. Progress saves in the browser.

- Import parts lists (BrickLink paste, Brickset CSV, Rebrickable API)
- Tick off pieces as you find them
- Live stats, pause timer, drop counter, minifig support

## Local use

Open `index.html` in a browser, or:

```bash
python -m http.server 8080
# visit http://localhost:8080
```

## Deploy (GitHub Pages)

1. Push this repo to GitHub (public).
2. **Settings → Pages → Build and deployment**
   - Source: **Deploy from a branch**
   - Branch: **main** / **/ (root)**
3. **Settings → Pages → Custom domain:** `excavation.buildbeyondbelief.com`
4. Wait for DNS check (can take up to 24h; usually minutes).
5. Enable **Enforce HTTPS** once the certificate is issued.

## DNS (subdomain)

At your DNS provider for `buildbeyondbelief.com`, add:

| Type  | Name        | Value              | TTL  |
|-------|-------------|--------------------|------|
| CNAME | `excavation` | `yoans.github.io` | 3600 |

(`yoans` = GitHub username — change if you use a different account.)

GitHub Pages docs: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site

## LEGO disclaimer

Independent fan tool. Not affiliated with the LEGO Group. LEGO® is a trademark of the LEGO Group.

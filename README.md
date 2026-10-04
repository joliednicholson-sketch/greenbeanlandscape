# Green Bean Landscape Designs website

Static website for **greenbeanlandscapedesigns.com**. It's plain HTML and CSS, so there's no build step.

## Files

- `index.html`: page content
- `styles.css`: styling
- `assets/`: logo and project photos
- `CNAME`: tells GitHub Pages to serve the site at greenbeanlandscapedesigns.com
- `.github/workflows/pages.yml`: deploys to GitHub Pages on every push to `main`

## Placeholders to replace

Search `index.html` for these:

- `[YOUR CITY]` / `YOUR CITY, ST`: service area
- `YOUR_FORM_ID`: form service ID so consultation requests reach your inbox
- Gallery: put photos in `assets/gallery/` and replace each placeholder `<figure>` (the comment in the gallery section shows the markup)

## Going live

1. In the GitHub repo, open **Settings → Pages** and set **Source** to **GitHub Actions**.
2. At your domain registrar, add DNS records for `greenbeanlandscapedesigns.com` (on Cloudflare, set each to **DNS only**):
   - Four `A` records for the root domain: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - A `CNAME` record for `www` pointing to `joliednicholson-sketch.github.io`
3. In **Settings → Pages**, enter `greenbeanlandscapedesigns.com` as the custom domain. Once DNS has propagated, turn on **Enforce HTTPS**.

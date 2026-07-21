# Scrupel Website

Marketing/landing site for Scrupel, deployed via GitHub Pages at
[www.scrupel.com](https://www.scrupel.com).

## Structure

Plain static HTML/CSS/JS — no build step, no framework, no dependencies.
Edit `index.html` / `styles.css` directly.

- `index.html` — the whole site (single page for now)
- `styles.css` — brand palette mirrors the Scrupel app's own light/dark
  theme tokens (`App.jsx`'s `LIGHT`/`DARK` objects) so the site and product
  read as one brand
- `favicon.png` — copied from the app's own launcher icon
- `CNAME` — tells GitHub Pages the custom domain (`www.scrupel.com`)

## Deploying

Pages is configured to build from the `main` branch root — pushing to
`main` deploys automatically. No CI config needed for a plain static site.

## Content status

The current copy is a first-draft placeholder (features list, "request
early access" CTA) written to have something real to verify DNS/deploy
against — replace it with real copy/screenshots once the app is further
along. The privacy policy at `/privacy` referenced in `index.html` doesn't
exist yet; the real one currently lives in the main app repo
(`scrupel-app/public/privacypolicy.html`) and should be ported over before
launch.

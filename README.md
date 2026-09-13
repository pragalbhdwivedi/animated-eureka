# BDSPS Competitive Exam Preparation (CEP)

Public information website for the B.D.S. Public School Competitive Exam Preparation programme.

## Public URL

Planned custom domain: `https://cep.bdsps.in/`

The repository intentionally does **not** contain a `CNAME` file yet. Add the custom domain only when DNS is ready.

## Site structure

- `index.html` — public programme overview and contact
- `programme.html` — student/parent-facing explanation of how CEP works
- `pathways.html` — supported exam categories and eligibility notes
- `support.html` — fees, mock tests, document support and transport policy
- `hindi.html` — Hindi programme information
- `strategy.html` — legacy redirect only; no internal strategy content is published
- `styles.css` — responsive visual system
- `script.js` — mobile navigation, reveal effects and copyright year
- `favicon.svg`, `og-card.svg`, `site.webmanifest` — browser/social identity
- `robots.txt`, `sitemap.xml` — search-engine discovery
- `404.html` — custom error page
- `.github/workflows/deploy-pages.yml` — automatic GitHub Pages deployment

The site is dependency-free: no npm, build framework or database is required.

## GitHub Pages setup

The deployment workflow is already included. In the repository, open **Settings → Pages → Build and deployment** and set **Source** to **GitHub Actions**. Future pushes to `main` will then deploy automatically.

## Connecting `cep.bdsps.in` later

1. In DNS for `bdsps.in`, create a `CNAME` record for `cep` pointing to `pragalbhdwivedi.github.io`.
2. In **Repository Settings → Pages**, set the custom domain to `cep.bdsps.in`.
3. Add a repository-root file named `CNAME` containing exactly `cep.bdsps.in`.
4. After GitHub verifies DNS, enable **Enforce HTTPS**.

## Public-content rule

The website is intentionally parent/student facing. Internal preparation strategy, selection thresholds, staffing logic and operational decision rules should not be published here. Current exam dates, application windows and changing eligibility details should be issued as current notices rather than hard-coded into permanent pages.

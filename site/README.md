# Trade Mark Sourcing Ltd. — Website

A fast, responsive, single-page marketing website for Trade Mark Sourcing Ltd., a premium
apparel sourcing partner based in Dhaka, Bangladesh. Built with plain HTML, CSS, and vanilla
JavaScript — no build step required.

## Structure

```
site/
├── index.html        # Full single-page site (all sections)
├── css/styles.css    # Styles + responsive layout
├── js/main.js        # Nav, sticky header, scroll reveal
├── image/            # Site imagery
├── CNAME             # Custom domain for GitHub Pages
├── netlify.toml      # Netlify config + caching/security headers
├── robots.txt        # Crawler directives
└── sitemap.xml       # Sitemap
```

## Preview locally

Any static server works. For example:

```powershell
npx http-server ./site -p 8099
```

Then open http://127.0.0.1:8099

## Deploy to www.trademarksourcing.com

The domain must be pointed at your host. Two easy options:

### Option A — Netlify (drag & drop or CLI)
1. Create a site in Netlify and set the publish directory to this `site/` folder.
2. In Netlify: Domain settings → add custom domain `www.trademarksourcing.com`.
3. At your DNS provider, add a CNAME record:
   - `www` → `<your-site>.netlify.app`
   - (Apex `trademarksourcing.com` → redirect to `www`, or use Netlify DNS.)
4. Netlify provisions HTTPS automatically.

### Option B — GitHub Pages
1. Push the contents of `site/` to a GitHub repo (root of the branch used for Pages).
2. Repo → Settings → Pages → deploy from branch.
3. The included `CNAME` file sets the domain to `www.trademarksourcing.com`.
4. At your DNS provider, add a CNAME record: `www` → `<username>.github.io`.
5. Enable "Enforce HTTPS" once the certificate is issued.

> Note: DNS for trademarksourcing.com must be under your control to point it at the host.
> Publishing here prepares everything; the final go-live step is done at your DNS/host dashboard.

## Content source

Copy and company details are drawn from the Corporate Profile
(`content/TrademarkThreefold_V5.pdf`).
```

# LTI Organic SEO Dashboard

A one-page dashboard for londontradingindex.com with three views:

- **Director**: where the site stands, searches compared with visits, recommendations and decisions needed.
- **Marketing Manager**: main numbers, the 90-day action plan, and search demand charts.
- **SEO Specialist**: the full baseline, page speed, links and detail tables.

Data: Semrush (1 to 2 November 2026), Google PageSpeed Insights (2 November 2026) and an SEO crawler report (2 November 2026). Traffic numbers are Semrush estimates.

## Files

| File | What it does |
|---|---|
| `index.html` | The whole dashboard. Data, styles and charts are all inside this file. |
| `vercel.json` | Vercel settings. Tells search engines not to index the site. |
| `robots.txt` | Asks search engines not to crawl the site. |
| `.gitignore` | Files Git should ignore. |

No build step and no packages are needed.

## Put It on GitHub

```bash
cd lti-seo-dashboard
git init
git add .
git commit -m "Add LTI SEO dashboard"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/lti-seo-dashboard.git
git push -u origin main
```

Create the empty repo on GitHub first (you can make it private), then replace `YOUR-USERNAME`.

## Deploy on Vercel

1. Go to vercel.com and choose **Add New → Project**.
2. Import the `lti-seo-dashboard` repo.
3. Framework preset: **Other**. Leave the build command and output folder empty.
4. Click **Deploy**.

Every push to `main` updates the live site.

## Open a Specific View

Add one of these to the end of the link:

- `#director`
- `#manager`
- `#specialist`

## Update the Numbers

All numbers are in the `const DATA = {...}` line near the bottom of `index.html`. Edit the values, commit and push. The charts and tables update by themselves.

## Privacy

The site is not listed on search engines, but anyone with the link can open it. For password protection, use Vercel's Deployment Protection (paid plans).

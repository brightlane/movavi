# Movavi Video Hub

Independent affiliate SEO site for Movavi video editing software.

**Live site:** https://brightlane.github.io/movavi/

## Setup

1. Upload `build.py` to the root of this repo
2. Create `.github/workflows/deploy.yml` (use the provided `movavi_deploy.yml`)
3. Go to **Settings → Pages → Source → GitHub Actions**
4. Go to **Settings → Secrets → Actions → New repository secret**
   - Name: `ANTHROPIC_API_KEY`
   - Value: your Anthropic API key (enables daily AI blog post)
5. Push to `main` to trigger the first build

## What It Builds

- **875 keyword pages** — core guides, how-tos, comparisons, task guides, platform guides, geo (50 states + 50 cities)
- **30 blog posts** — rotating seed topics, daily AI-generated post via Claude API
- **14 essential pages** — homepage, guides index, blog, FAQ, about, privacy, terms, disclaimer, sitemap, robots.txt, og.svg, llms.txt, RSS

**Total: ~919 pages**

## File Layout

```
repo root/
├── build.py                    ← the build script
└── .github/
    └── workflows/
        └── deploy.yml          ← GitHub Actions (cron 6 AM UTC daily)
```

## Affiliate

All CTAs link to:
`https://www.linkconnector.com/ta.php?lc=007949109434006513&atid=MovaviWebs`

## Verification

Both tags appear in the `<head>` of every page:
```html
<meta name="google-site-verification" content="eWVDN3vbam9nnaZQu7wAQKyfmJJdM7zjI80l4DGeUrQ">
<meta name="msvalidate.01" content="574044E39556B8B8DAAF1D1F233C87B0">
```

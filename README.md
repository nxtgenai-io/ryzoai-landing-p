# RyzoAi — ryzoai.in Deployment Files

## Files in this folder

| File | Purpose |
|------|---------|
| `index.html` | Main landing page (SEO optimized) |
| `404.html` | Custom 404 error page (matches RyzoAi design) |
| `sitemap.xml` | Sitemap for Google indexing |
| `robots.txt` | Tells Google bots to crawl the site |
| `CNAME` | Connects ryzoai.in domain to GitHub Pages |
| `_config.yml` | GitHub Pages configuration |
| `google-site-verification-REPLACE-THIS.html` | RENAME this to your actual GSC verification filename |

## Deploy Steps

### Step 1 — GitHub
1. Create a FREE account at github.com
2. Create new repository → name it `ryzoai` → set Public → Create
3. Upload ALL files in this folder to the repo root

### Step 2 — Enable GitHub Pages
Settings → Pages → Source: Deploy from branch → Branch: main → / (root) → Save

### Step 3 — Connect ryzoai.in domain
Settings → Pages → Custom domain → type `ryzoai.in` → Save → tick Enforce HTTPS

### Step 4 — DNS Records (add at your domain registrar)
| Type | Host | Value |
|------|------|-------|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | nxtgenai-io.github.io |

### Step 5 — Google Search Console
1. Go to search.google.com/search-console
2. Add Property → ryzoai.in
3. Download the HTML verification file → rename it → upload to GitHub repo
4. Sitemaps → Submit: sitemap.xml
5. URL Inspection → https://ryzoai.in → Request Indexing

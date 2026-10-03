# The Huang Family

The official website of the Huang family, hosted on [GitHub Pages](https://pages.github.com).

**Live site:** https://thehuangfamily.org

## Structure

```
.
├── CNAME            # points the site to thehuangfamily.org
├── index.html       # homepage
├── about.html       # our story
├── css/
│   └── style.css    # site styling
└── images/          # drop family photos here
```

## Custom domain DNS (apex: thehuangfamily.org)

Point these at your DNS provider (Cloudflare example values below).

**Apex A records** (one per IP, host = `@` / blank):

| Host | Type | Value |
|------|------|-------|
| @    | A    | 185.199.108.153 |
| @    | A    | 185.199.109.153 |
| @    | A    | 185.199.110.153 |
| @    | A    | 185.199.111.153 |

**www CNAME:**

| Host | Type  | Value |
|------|-------|-------|
| www  | CNAME | thehuangfamily.org |

Optional IPv6 AAAA for the apex: `2606:50c0:8000::153` `2606:50c0:8001::153` `2606:50c0:8002::153` `2606:50c0:8003::153`

After DNS propagates, GitHub will issue an SSL cert for the custom domain (up to ~24h), then enable **Enforce HTTPS**.

## Editing

Edit any `.html` file, commit, push — GitHub rebuilds and republishes automatically. Changes can take up to ~10 minutes to go live.
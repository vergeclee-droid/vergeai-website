# SEO Submission Guide — www.vergeai.net

## ✅ Already done (preparation)
- [x] Self-hosted fonts（Google Fonts replaced with local files — no GFW blocking）
- [x] Updated all URLs to www.vergeai.net（canonical, og:image, hreflang, sitemap, JSON-LD）
- [x] Sitemap ready at https://www.vergeai.net/sitemap.xml
- [x] Robots.txt at https://www.vergeai.net/robots.txt
- [x] Site deployed with SSL ✅

## 📋 Google Search Console

### What I prepared:
- Canonical URLs all pointing to `https://www.vergeai.net/`
- Sitemap updated with correct `www` URLs
- JSON-LD structured data with `www.vergeai.net`

### What you need to do:
1. Go to https://search.google.com/search-console
2. Click **Add property** → Choose **Domain** → Enter `vergeai.net`
3. Google gives you a TXT verification code (format: `google-site-verification=xxxxxxxxx`)
4. **Copy that code to me** — I'll format the exact TXT record for O365 DNS
5. Add the TXT record in O365 Admin → Settings → Domains → `vergeai.net` → DNS records
6. Return to GSC → Click **Verify**
7. Go to **Sitemaps** → Submit `https://www.vergeai.net/sitemap.xml`

## 📋 Baidu（百度站長平台）

### Important finding:
- **ICP filing NOT required** for Baidu organic search indexing
- Your site is hosted on Azure (global), which is acceptable
- Without ICP, you won't get:
  - Baidu "V" Trust Badge
  - Baidu Ads (paid search)
  - Fastest possible load speed in China

### What I prepared:
- Removed Google Fonts（was blocked by GFW ✅）
- Self-hosted all fonts locally ✅
- 简体中文 content already in website ✅
- HTTPS active ✅

### What you need to do (if targeting China):
1. Option A: Just submit to Baidu Webmaster Tools (no ICP needed)
   - Go to https://ziyuan.baidu.com/
   - Add site `www.vergeai.net`
   - Verify via DNS TXT or HTML file
   - Submit sitemap
2. Option B: ICP filing (recommended for better China performance)
   - Requires Chinese business license or partner
   - China mainland hosting (阿里云/腾讯云/百度云)
   - Takes 2-6 weeks
   - Costs ~S$500-1,500 via consultant

## 📋 Bing Webmaster Tools (optional)
- Can import directly from Google Search Console
- Or verify via DNS TXT

## ⚡ Speed checklist
- [x] Self-hosted fonts (no Google Fonts blocking)
- [x] No YouTube/Facebook embeds
- [x] HTTPS active
- [x] Azure CDN (global)
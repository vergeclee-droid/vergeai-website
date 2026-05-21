# Verge AI 官方網站

靜態一頁式公司網站，支援 **EN | 简体 | 繁體** 三語言即時切換。

## 檔案結構

```
vergeai-website/
├── index.html    # 主頁（三語切換，已含 SEO meta）
├── logo.png      # Logo（Hero 用，609×559）
├── logo-nav.png  # Logo（導航欄用，100×100）
├── sitemap.xml   # Sitemap（Google Search Console）
└── robots.txt    # 允許所有爬蟲
```

## SEO 優化內容

- **Meta tags**：language-specific title/description, keywords, author, canonical URL
- **Open Graph**：Facebook/LinkedIn/Twitter 分享 preview（大圖卡）
- **Twitter Card**：summary_large_image
- **hreflang**：en / zh-Hans / zh-Hant / x-default 四組語言標籤
- **JSON-LD Structured Data**：Organization Schema（公司名稱、地址、Logo、成立日期）
- **動態 SEO**：JS 自動切換 `<title>` 同 `<meta name="description">` 跟隨語言選擇
- **Sitemap + Robots**：submit 去 Google Search Console 即可

## 技術規格

- **語言**：HTML + CSS + JS（純靜態，無依賴）
- **三語系統**：`[data-lang]` 屬性 + CSS `display` 切換，零 JS 渲染依賴
- **字型**：Inter + Noto Sans SC/TC（Google Fonts 後備）
- **配色**：白色底色 + #06b6d4（藍色）+ #818cf8（靛紫）+ #a78bfa（淺紫）
- **響應式**：Desktop / Tablet / Mobile
- **特效**：導航欄 scroll 效果、區塊淡入動畫（Intersection Observer）、平滑滾動

## 語言系統

- 🎯 **自動檢測** — 根據瀏覽器語言自動切換（zh-TW/zh-HK → 繁體，zh-CN → 簡體，其餘 → EN）
- 💾 **localStorage 記住選擇** — 關閉分頁後再次訪問保留上次語言
- 🔄 **手動切換** — 導航欄右側 EN / 简体 / 繁體 按鈕

## 頁面結構

| Section | 內容 |
|---------|------|
| Hero | Logo + Tagline（三語）+ CTA 按鈕 |
| About | 公司使命 + 3 張核心價值卡（Private / Real-Time / Ecosystem） |
| VergeOps | 4 個 Use Case（RCA / Smart Ticketing / SLA Guardian / Security Defense），深色背景 |
| Verge Robotics | 2 款機器人產品（Verge Carry 配送 + Verge Scrub 清潔），深色背景 |
| Edge AI Home | Hub + Satellite 產品結構（Home Hub + Smart Mirror + Kitchen Agent + 4 小卡） |
| Technology | 4 格技術亮點（Private LLM / aiDAPTIV+ / Verge Agentic OS / METIS） |
| Contact | 深圳 + 香港地址，hello@vergeai.net |
| Footer | 導航連結 + 版權 |

## 部署方式

將整個 `vergeai-website/` 目錄上傳至網頁伺服器或 CDN（Vercel / Netlify / Cloudflare Pages）即可。

靜態網站，無需後端，無構建步驟。

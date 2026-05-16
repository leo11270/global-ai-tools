# 发布到公网并被搜索收录

## 1) 先发布（推荐 GitHub Pages / Cloudflare Pages / Netlify）
- 站点根目录就是当前文件夹。
- 入口文件：`index.html`

## 2) 发布后立刻改这 3 个地方（把 `example.com` 换成你的真实域名）
- `index.html` 中 `og:url`
- `robots.txt` 中 `Sitemap:`
- `sitemap.xml` 中 `<loc>`

## 3) 提交搜索引擎
- Google Search Console 提交：`https://你的域名/sitemap.xml`
- Bing Webmaster Tools 提交：`https://你的域名/sitemap.xml`

## 4) 注意
- 只有发布到 `https://` 公网域名后，别人和搜索引擎才能访问；`file://` 本地地址不会被收录。

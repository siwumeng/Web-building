全球主流媒体导航 - 部署说明
==========================

说明：
这是一个静态网站包（HTML + CSS + JS），适用于 Vercel / Netlify / GitHub Pages / Cloudflare Pages 等静态托管平台。

文件结构：
- index.html    —— 站点主页面
- style.css     —— 样式文件（黑白极简风）
- media-data.js  —— 媒体数据（可直接扩展）
- deploy_guide.txt —— 简短部署说明

快速部署（Vercel，上传 ZIP）：
1. 登录 https://vercel.com
2. 点击 “New Project” → “Import” → 选择 “Upload”
3. 上传此 ZIP，并点击 Deploy
4. 部署完成后会生成 https://<project-name>.vercel.app 的公网地址

快速部署（GitHub）：
1. 新建 GitHub 仓库，上传此目录所有文件，提交
2. 在 Vercel 点击 “Import Project” 并选择该仓库，Deploy

其他：
- 若要更改数据，请编辑 media-data.js（每个 country 对象下的 outlets 数组）
- 如需接入动态 API 或后台，可把媒体数据替换为远程 JSON 并使用 fetch 加载
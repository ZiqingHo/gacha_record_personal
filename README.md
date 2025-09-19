# 深空抽卡 PWA（GitHub Pages 部署）

## 部署步骤
1. 在 GitHub 新建一个仓库（名字随意）。
2. 把本目录的所有文件 **index.html, sw.js, manifest.webmanifest, icon-192.png, icon-512.png, apple-touch-icon-180.png** 推送到仓库根目录。
3. 打开仓库 -> **Settings** -> **Pages**：
   - **Source** 选择 `Deploy from a branch`
   - **Branch** 选择 `main` 分支 和 `/ (root)` 目录，保存。
4. 大概 1 分钟后，Pages 会生成一个网址，形如 `https://<你的用户名>.github.io/<仓库名>/`。
5. 用 **iPhone 的 Safari** 打开该网址，点击底部 **分享** -> **添加到主屏幕**。

> 说明：GitHub Pages 站点**对外公开**访问。你可以把仓库设为 *Private*，但生成的 Pages 站点依然是公开的；
> 如果你需要访问控制，可以：
> - 用 **Cloudflare Access** 给站点加登录；或
> - 使用 **Vercel / Netlify** 并开启受保护路由；或
> - 自己部署到支持 Basic Auth 的服务器。

## 开发说明
- 首次打开会注册 `sw.js`，缓存静态资源，之后离线可用。
- 数据保存在浏览器的 `localStorage`，不会上传到服务器。
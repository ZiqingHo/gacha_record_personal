# 深空抽卡 PWA

## 部署步骤
1. 在 GitHub 新建一个仓库。
2. 把本目录的所有文件推送到仓库根目录。
3. 打开仓库 -> **Settings** -> **Pages**：
   - **Source** 选择 `Deploy from a branch`
   - **Branch** 选择 `main` 分支 和 `/ (root)` 目录，保存。
4. 大概 1 分钟后，Pages 会生成一个网址，形如 `https://<你的用户名>.github.io/<仓库名>/`。
5. 用 **iPhone 的 Safari** 打开该网址，点击底部 **分享** -> **添加到主屏幕**。

## 开发说明
- 首次打开会注册 `service-worker.js`，缓存静态资源，之后离线可用。
- 数据保存在浏览器的 `localStorage`，不会上传到服务器。

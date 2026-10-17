# 静心木鱼 · 功德 +1

一个黑金风格的电子木鱼单页网页，适配 iPhone、Android 和电脑端。

## 特性

- 敲击木鱼、木槌动画、敲击音效
- 快速连续敲击、浮动「功德 +1」、连击显示
- 今日敲击次数、累计敲击次数，使用浏览器 localStorage 本地保存
- 音效开关、清空记录（二次确认）
- iOS Safari 适配：避免快速双击引起网页放大，避免触摸选择及页面滚动
- 完全独立的 `index.html`，木鱼与木槌素材已嵌入文件，不需要额外图片、字体、音频或第三方 JS

## GitHub Pages 部署

1. 创建一个 GitHub 仓库，上传项目根目录中的 `index.html`（也可以一并上传 `README.md`）。
2. 进入仓库 **Settings → Pages**。
3. 在 **Build and deployment** 中选择 **Deploy from a branch**。
4. Branch 选择 `main`，文件夹选择 `/(root)`，点击保存。
5. 等待 GitHub Pages 完成发布，然后打开 Pages 提供的网址。

> 注意：所有敲击记录只保存在当前浏览器的本地存储中，不会自动在设备之间同步。iOS Safari 的音效会在用户首次主动敲击后解锁。

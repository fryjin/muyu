# 静心木鱼 V2.0 · 重构版

直接上传 `index.html` 到 GitHub 仓库根目录，并在 Settings → Pages 启用 main 分支部署。

## 变更
- 全新独立木鱼与木槌素材（`assets/woodfish.svg` 和 `assets/mallet.svg` 为可编辑设计源）；网页内嵌高精度透明 WebP，避免运动时 SVG 重绘。
- 只对木槌执行 CSS `transform` 动画；不使用持续 `requestAnimationFrame` 循环。
- 触摸按下立即计数，松手播放音效；阻止木鱼区域双击缩放，过滤合成 click。
- 浮字仅复用 6 个动画对象，独立于敲击计数。
- 功德与设置沿用旧键 `zen-woodfish-v1`，同域名/同浏览器可继承旧数据。
- 10 阶当日成就每日按设备本地日期重置，历史累计不清空。

## 测试建议
更新后在 Safari 访问 `?v=20` 以绕过旧 HTML 缓存。建议分别测试慢敲、连续快敲、静音和有声音的表现。

> 提醒：网页不能改变手机物理静音开关，Safari 音频输出也会受设备静音、音量和输出路径影响。

# zibuyuweb

「子不语」系列 iOS 应用的 App Store 上架配套静态页，由 GitHub Pages 托管，无构建、无外部依赖。一个仓服务所有 App，按项目分子目录。

- 首页（项目列表）：<https://miaolegemi9527.github.io/zibuyuweb/>

## 各 App 页面与 App Store Connect 填写用 URL

| App | 隐私政策 URL | 技术支持 URL |
|---|---|---|
| 子不语输入法 | <https://miaolegemi9527.github.io/zibuyuweb/input/privacy/> | <https://miaolegemi9527.github.io/zibuyuweb/input/support/> |
| 子不语照相馆 | <https://miaolegemi9527.github.io/zibuyuweb/camera/privacy/> | <https://miaolegemi9527.github.io/zibuyuweb/camera/support/> |
| 子不语浏览器 | <https://miaolegemi9527.github.io/zibuyuweb/browser/privacy/> | <https://miaolegemi9527.github.io/zibuyuweb/browser/support/> |

用户反馈渠道 = 本仓 GitHub Issues，按 label 分拣：`input` / `camera` / `browser`（各 App 支持页的反馈链接已预挂对应 label）。

## 维护说明

- **子不语输入法**：隐私政策正文与 App 内置 `QQInput/PRIVACY.md` 逐字同源（真源在 App 仓）；改动先改真源，再同步本仓 `input/privacy/index.html` 并更新页面顶部「更新日期」与 English Summary。
- **子不语照相馆**：网页版为完整版；App 内设置页有一段概要（`QQSettingsView.swift` 隐私政策条目），两端口径必须一致，改任一侧需同步另一侧。
- **子不语浏览器**：网页版为完整版与唯一真源；App 内暂无活跃的隐私政策入口（2023 年本地用户协议中「用户数据都存于本地」一句已过时，待 App 侧批次更新）。
- 风格与 App 上架图「墨夜极光」一致：深底 + 极光渐变强调色，样式集中在 `assets/style.css`。
- 纯静态 HTML，相对路径链接；新增 App 时：建 `<slug>/privacy/`、`<slug>/support/` 两个页面 + 首页加卡片 + 建 Issues label，路径口径见上表。

# 通联速记 · QSO Quick Log

业余无线电（Ham Radio）通联快速记录工具，单文件网页应用。打开即用、无需安装、无需注册，数据保存在本机浏览器；在 iPhone 上添加到主屏幕后全屏运行，体验接近原生 App。

**在线地址：<https://xiaoninaoh.github.io/qso-quick-log/>**

## 功能

| 功能 | 说明 |
| --- | --- |
| 快速记录流 | 从「呼号」开始打字，`Enter` 逐项下移，最后一项按 `Enter` 即保存并开始下一条 |
| 自动填充 | 老呼号自动带出上次信息；频率自动换算波段（也认 kHz，如 14074） |
| 信号报告 | 分「我给对方 / 对方给我」记录 R 与 S；S9 后可填 +dB；CW 模式自动出现 T 音调 |
| 电子 QSL | 点记录右侧「QSL」生成电子卡片，可打印存为 PDF；导出后自动打上 QSL ✓ 标签 |
| 数据导出 / 导入 | 支持 ADIF、CSV、JSON；JSON 为完整备份，可跨设备导入合并 |
| 搜索 | 按呼号、QTH、姓名、设备搜索历史通联 |
| 主题 | 自动跟随系统深浅色，也可在设置中手动切换 |
| 时间换算 | 通联时间按 CST 录入，自动换算 UTC |

## 在手机上使用（推荐）

1. 用 Safari 打开在线地址；
2. 点底部「分享」→「添加到主屏幕」；
3. 桌面上出现「通联速记」图标，点开即全屏运行。

## 数据与隐私

- 所有记录仅保存在**本机浏览器**（localStorage），不会上传到任何服务器；
- 请定期导出 ADIF / CSV / JSON 备份，防止清理浏览器数据时丢失；
- 手机 ↔ 电脑同步：任一端导出 JSON 备份，用隔空投送 / 微信传输到另一端，再点「导入」合并。

## 目录结构

```text
.
├── index.html       # 应用本体（HTML / CSS / JS 全部内联，单文件）
├── manifest.json    # PWA 清单，支撑「添加到主屏幕」
├── icon.png         # 180×180，Safari 主屏幕图标
├── icon-192.png     # 192×192，清单图标
├── icon-512.png     # 512×512，清单图标
└── README.md
```

## 部署与更新

纯静态站点，无构建步骤。任意静态托管平台均可：

- 本仓库：推送 `main` 分支后，GitHub Pages 自动更新；
- 其他平台：把 `index.html`、`manifest.json`、图标一并拖入 Netlify Drop / Vercel 等即可。

## 技术说明

- 无框架、无构建工具的单文件 HTML 应用；
- 数据持久化：浏览器 `localStorage`；
- 字体：Google Fonts（Anton / Martian Mono / Inter / Noto Sans SC）；
- PWA 能力：`manifest.json` + `apple-touch-icon`，支持 iOS「添加到主屏幕」全屏模式。

## 版权

© 2026 BI9DAS

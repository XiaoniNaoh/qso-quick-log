# 📻 通联速记 · QSO Quick Log

呼号一输，`Enter` 一路按下去，一条 QSO 就这么记好了——是不是很顺？

这是为业余无线电（Ham Radio）爱好者做的一个**单文件网页小工具**：不用安装、不用注册、不占内存，电脑和手机浏览器打开就能用，还能「添加到主屏幕」变成全屏 App 的感觉。

**在线地址：<https://xiaoninaoh.github.io/qso-quick-log/>**

**作者：BI9DAS** · 个人网站：<https://bioez.xyz>

## 怎么用？

### 🖥️ 电脑（Windows / macOS / Linux）

- 打开网址直接用；Chrome / Edge 地址栏的「安装」按钮，可以把 TA 变成桌面应用；
- 全程键盘流：从呼号开始，`Enter` 一路下移，最后一下保存。

### 📱 iPhone / iPad

1. 用 Safari 打开网址；
2. 分享 →「添加到主屏幕」；
3. 桌面上出现「通联速记」图标，点开即全屏。

### 🤖 安卓

1. 用 Chrome 打开网址；
2. 右上角菜单 →「添加到主屏幕 / 安装应用」。

## 它有多好用？

### ✍️ 记一条通联，快得像说话

- 呼号起头，`Enter` 逐项下移，最后一下保存并自动开新一条；
- 老呼号自动带出上次的信息，不用重复输入；
- 频率自动换算波段，还认 kHz（比如 `14074`）；
- 通联时间按 CST 录入，UTC 自动算好。

### 📊 信号报告，双向都记

- 「我给对方 / 对方给我」的 R 和 S 分开记；
- 满格 S9 还能加 +dB；
- 玩 CW 时自动出现 T 音调字段。

### 🃏 电子 QSL 卡片

- 点一下「QSL」，卡片自动生成，打印或存 PDF 都行；
- 导出后自动盖上 QSL ✓ 的章。

### 💾 数据都是你的

- 导出 **ADIF**（日志软件都认）、**CSV**（Excel / Numbers 直接开）、**JSON**（完整备份）；
- JSON 导出 / 导入 = 换设备不换记忆：隔空投送、微信、网盘随便传；
- 想找某条记录？搜呼号、QTH、姓名、设备都行。

### ⚙️ 按你的习惯来

- 我的呼号、默认频率 / 模式 / 信号报告；
- 设备、天线、功率、QTH、Grid 定位（QSL 卡片上要用）；
- 深色模式自动跟随系统，也能手动切。

## 🔒 数据与隐私

- 记录只存在**你自己的浏览器里**（localStorage），不经过任何服务器；
- 清理浏览器数据 = 记录消失，记得定期导出备份；
- 跨设备同步：一端导 JSON，传到另一端，点「导入」合并。

## 📁 仓库结构

```text
.
├── index.html       # 应用本体（HTML / CSS / JS 全在一页里）
├── manifest.json    # PWA 清单，支撑「安装 / 添加到主屏幕」
├── logo.png         # 项目 logo（1254×1254）
├── icon.png         # 180×180 iOS 主屏幕图标
├── icon-192.png     # 192×192 PWA 图标
├── icon-512.png     # 512×512 PWA 图标
├── LICENSE
├── .gitignore
└── README.md
```

## 🚀 部署与更新

纯静态、零构建：推 `main` 分支，GitHub Pages 自动更新；想换平台，把这几个文件拖进 Netlify Drop / Vercel 也一样跑。

## 🛠️ 技术小抄

- 单文件 HTML / CSS / JS，无框架；
- 存储：浏览器 `localStorage`；
- 字体：Google Fonts（Anton / Martian Mono / Inter / Noto Sans SC）；
- PWA：`manifest.json` + `apple-touch-icon`。

## 🧑‍🚀 关于作者

BI9DAS，业余无线电爱好者一枚。这个工具本来是做给自己通联速记用的，顺手开源出来，希望也能帮到频率上认识的你。

个人网站：<https://bioez.xyz> —— 欢迎来串门。

**73！频率上见。** 📡

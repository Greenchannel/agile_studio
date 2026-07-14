# 🧊 Agile Studio 灵动工作室官网

灵动工作室官方网站，采用了 **液态玻璃（Glassmorphism）** 设计风格。

## ✨ 特性

- **毛玻璃效果** — 所有容器使用 `backdrop-filter: blur()` 实现半透明磨砂玻璃质感
- **动态渐变背景** — 多色渐变背景平滑循环流动，增强视觉层次感
- **顺滑过渡动画** — 所有交互（悬停、切换、加载）均以 `cubic-bezier` 贝塞尔曲线驱动
- **响应式统一** — 全站（主页 + 子页面）共用同一套 CSS 主题，风格一致

## 📁 项目结构

```
agile_studio/
├── index.html                  # 主页
├── error.html                  # 404 页面
├── fav.ico                     # 网站图标
├── agile_logo.webp             # 工作室 LOGO
├── new-shows.webp              # 展示图片
├── css/
│   ├── agile-theme.css         # 主题样式（含液态玻璃效果）
│   ├── tone.css                # ToneCSS 入口
│   └── lib/                    # ToneCSS 核心库
│       ├── core.min.css
│       ├── article.min.css
│       ├── ... (其他 ToneCSS 模块)
│       └── nav.min.css
├── index-shows/                # 子页面
│   ├── activities-history.html # 历史活动
│   ├── gc.html                 # 个人介绍 - _cute486_
│   ├── xpan.html               # 个人介绍 - 小潘
│   ├── xwang.html              # 个人介绍 - 小王
│   ├── ds.html                 # 个人介绍 - DeepSeek
│   └── *.webp                  # 子页面用图片
└── index-download/             # 下载站
    ├── download.html           # 资源下载首页
    ├── wallpaper.html          # 壁纸下载
    └── *.webp                  # 壁纸预览图
```

## 🎨 液态玻璃设计变量

定义在 `:root` 中的 CSS 自定义变量：

| 变量 | 值 | 作用 |
|------|-----|------|
| `--glass-bg` | `rgba(255, 255, 255, 0.12)` | 玻璃基础背景 |
| `--glass-bg-strong` | `rgba(255, 255, 255, 0.18)` | 悬停/强调态背景 |
| `--glass-border` | `1px solid rgba(255, 255, 255, 0.25)` | 玻璃边框 |
| `--glass-blur` | `blur(16px)` | 毛玻璃模糊强度 |
| `--glass-shadow` | `0 8px 32px rgba(0, 0, 0, 0.25)` | 投影阴影 |
| `--glass-transition` | `all 0.4s cubic-bezier(0.25, 0.46, 0.45, 0.94)` | 统一过渡曲线 |

## 🚀 部署

支持 **GitHub Pages** 和 **Cloudflare Pages** 两种部署方式，直接推送仓库即可自动部署。

## 📄 许可证

© AGILE STUDIO 版权所有
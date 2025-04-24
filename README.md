# CloudDeployKit

一个开箱即用的静态站点部署工具，支持 Cloudflare Pages 和 GitHub Pages 双平台部署，适用于个人博客、项目展示、工具页等轻量应用场景。

## 🚀 特性

- ⚡ 一键部署支持 GitHub Pages 与 Cloudflare Pages
- 🧩 提供多种模板（HTML、Vue3 + Vite、React 等）
- 🌍 多语言文档支持（中文 / English）
- 🛠️ 自动化部署配置（GitHub Actions）
- 💡 适合个人项目、小工具、博客展示等使用场景

## 📦 快速开始

### 使用 GitHub Pages 部署

1. Fork 本项目或下载模板至本地
2. 修改 `templates/vanilla-html/` 下的内容
3. 启用 GitHub Pages：
   - 进入仓库 → Settings → Pages
   - Source 选择 `main` 分支和 `templates/vanilla-html` 目录
4. 完成！

### 使用 Cloudflare Pages 部署

1. 在 Cloudflare Pages 创建新项目，选择 GitHub 仓库
2. 设置 Build 配置：
   - Build command: `echo skip`
   - Output folder: `templates/vanilla-html`
3. 保存并部署

---

## 📁 项目结构

```
CloudDeployKit/
├── README.md                # 项目说明
├── LICENSE                  # 开源许可证（MIT）
├── deploy-guide.md          # 手动部署教程
├── .github/
│   └── workflows/
│       └── deploy.yml       # GitHub Actions 自动部署脚本
├── templates/
│   ├── vanilla-html/
│   │   ├── index.html       # 默认 HTML 模板
│   │   └── styles.css       # 简洁样式
│   └── vue-vite/            # Vue3 + Vite 模板
│       ├── index.html
│       ├── vite.config.js
│       ├── package.json
│       └── src/
│           ├── App.vue
│           └── main.js
└── docs/
    └── zh/
        └── index.md         # 中文文档首页
```

## 📜 License

MIT License

---

欢迎 Star ⭐、Fork 🍴、提 Issues 🐞、PR ✨！

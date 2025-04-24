# 📘 deploy-guide.md（部署详细说明）

## 🚀 GitHub Pages 部署教程（图文版）

1. 打开本项目或 Fork 到你自己的 GitHub
2. 进入 `templates/vanilla-html` 文件夹，修改 `index.html` 和 `styles.css`
3. 进入 GitHub 仓库 → `Settings` → `Pages`
4. 配置 Source：
   - 分支选择 `main`
   - 文件夹选择 `templates/vanilla-html`
5. 保存后等待几秒，访问链接就能看到你的网站啦！

📌 示例地址：https://你的用户名.github.io/你的仓库名/


## 🌐 Cloudflare Pages 部署教程

1. 进入 [Cloudflare Pages](https://pages.cloudflare.com/) → `Create a project`
2. 绑定 GitHub 账号，选择本项目
3. Build 设置如下：
   - Build command: `echo skip`
   - Output folder: `templates/vanilla-html`
4. 确认后点击 `Save and Deploy`
5. 部署完成后可以自定义域名或绑定你自己的域名

📌 Cloudflare Pages 免费 CDN、国内访问速度优秀，推荐使用！


## 📝 注意事项

- 修改样式时推荐保留基础布局结构，避免构建失败
- GitHub Pages 支持自定义域名，需设置 CNAME 文件
- Cloudflare Pages 可以通过 dash 页面配置重定向、缓存等

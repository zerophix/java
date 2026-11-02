# Java 项目

一个通过 **GitHub Pages** 部署的纯静态 HTML 页面项目。

## 在线地址

🔗 https://zerophix.github.io/java

## 项目结构

```
.
├── index.html                 # 首页
├── assets/
│   ├── css/
│   │   └── style.css          # 样式
│   └── js/
│       └── main.js            # 脚本
└── .github/
    └── workflows/
        └── pages.yml          # GitHub Pages 自动部署
```

## 本地预览

```bash
# 方式一：用 Python 起本地静态服务器
python3 -m http.server 8080
# 浏览器打开 http://localhost:8080

# 方式二：用 npx serve
npx serve .
```

## 部署方式

项目使用 **GitHub Actions** 自动部署到 GitHub Pages：

1. 将代码推送到 `main` 分支
2. GitHub Actions 自动构建并部署
3. 访问 `https://zerophix.github.io/java`

### 手动触发

在 GitHub 仓库页面 → **Actions** → **Deploy static content to Pages** → **Run workflow** 手动触发一次部署。

> ⚠️ 首次部署需要在 GitHub 仓库 **Settings → Pages → Build and deployment → Source** 选择 **GitHub Actions** 作为部署源。

## 技术栈

- HTML5
- CSS3
- JavaScript
- GitHub Actions + GitHub Pages
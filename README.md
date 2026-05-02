# ✦ Hy01er's Tech Blog

基于 GitHub Pages 的单文件技术博客，支持**专栏分类**和 **Markdown 写作**。

## 特性

- **专栏系统** — 文章按专栏分类（前端/后端/系统设计/AI...），可自定义
- **Markdown 编辑** — marked.js 渲染 + highlight.js 代码语法高亮
- **管理面板** — 密码保护，侧滑抽屉式编辑器
- **标签系统** — 标签云 + 快速筛选
- **全文搜索** — 标题、标签、内容搜索
- **目录生成** — 文章内标题自动生成 TOC
- **阅读时间** — 估算文章阅读时长
- **纯静态部署** — 数据嵌入 HTML，无需服务器/数据库
- **一键发布** — 编辑完成 → 下载 HTML → git push 上线
- **响应式** — 桌面 + 移动端适配

## 使用方法

### 读者
访问 `https://hy01er.github.io` 浏览文章，无需登录。

### 作者（管理员）
1. 打开页面，点击右上角「管理」
2. 首次使用设置管理密码
3. 在管理面板中创建/编辑/删除文章
4. 管理专栏和标签
5. 点击「发布到 GitHub」→ 下载更新后的 `index.html`
6. 提交并推送到仓库

## 技术栈

- 纯原生 HTML/CSS/JS，零框架
- [marked.js](https://github.com/markedjs/marked) — Markdown 渲染
- [highlight.js](https://github.com/highlightjs/highlight.js) — 代码高亮
- Web Crypto API — SHA-256 密码哈希

## 专栏配置

默认四个专栏：🎨 前端 / ⚙️ 后端 / 🏗️ 系统设计 / 🤖 AI & ML

可在管理面板中增删改专栏，每个专栏有图标和名称。

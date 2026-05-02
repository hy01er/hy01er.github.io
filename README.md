# ✦ 星尘日记 · STARDUST JOURNAL

一款**端到端加密**的本地日记 + 技术博客应用，单文件 HTML，无需服务器。

## 特性

- **端到端加密** — PBKDF2-SHA256 (15万次迭代) + AES-256-GCM，数据仅你可读
- **双编辑模式** — 日记(富文本) + 博客(Markdown + 代码高亮)
- **本地存储** — 所有数据加密存储在浏览器 localStorage
- **回收站** — 30 天软删除，可恢复
- **星标收藏** — 标记重要内容
- **标签系统** — 标签云 + 快速筛选
- **迷你日历** — 侧边栏日历，点击日期快速定位
- **搜索** — 全文搜索 + 标签筛选
- **导入/导出** — 加密备份 JSON，支持合并导入
- **统计面板** — 连续写作天数、总字数、博客数
- **自动保存** — 1.5 秒防抖，草稿不丢失
- **键盘快捷键** — Ctrl+S/N/B/F/T
- **响应式** — 桌面 + 移动端适配

## 使用方法

1. 直接浏览器打开 `index.html`
2. 首次使用设置账号密码
3. 开始写日记或博客

## 部署 (GitHub Pages)

1. Fork 或创建仓库 `{username}.github.io`
2. 将 `index.html` 放在仓库根目录
3. 启用 GitHub Pages → 访问 `https://{username}.github.io`

## 技术栈

- 纯原生 HTML/CSS/JS，零框架
- [marked.js](https://github.com/markedjs/marked) — Markdown 渲染
- [highlight.js](https://github.com/highlightjs/highlight.js) — 代码语法高亮
- Web Crypto API — PBKDF2 + AES-256-GCM 加密

## 安全

密码使用 PBKDF2-SHA256 派生加密密钥，数据使用 AES-256-GCM 加密后存储在 localStorage。
服务器端不存储任何数据，所有加解密在浏览器本地完成。

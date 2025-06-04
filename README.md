# simple-md-doc

一个简单的 Markdown 文档浏览器，支持通过 hash 跳转和渲染本地 Markdown 文件。

## 功能

- 支持渲染本地 Markdown 文件为 HTML
- 自动提取 Markdown 第一行作为页面标题
- 支持通过 URL hash 跳转不同文档
- 外部链接自动新标签页打开
- 提供返回首页按钮

## 使用方法

1. 将本项目放置于本地服务器目录下（如使用 VSCode Live Server、http-server 等）。
2. 在项目根目录下放置你的 Markdown 文件（如 `index.md`, `foo.md` 等）。
3. 访问 `index.html`，即可浏览和跳转 Markdown 文档。

## 依赖

- [marked.js](https://github.com/markedjs/marked) 用于 Markdown 解析


# simple-md-doc

一个简单的 Markdown 文档浏览器，支持通过 hash 跳转和渲染本地 Markdown 文件。
> 诞生原因是只需要非常简单地处理Markdown，所以懒得找框架构建

## 功能

- 支持渲染本地 Markdown 文件为 HTML
- 自动提取 Markdown 第一行作为页面标题
- 支持通过 URL hash 跳转不同文档
- 外部链接自动新标签页打开
- 提供返回首页按钮

## 使用方法

0. 仅需复制`index.html`用于你的项目。
1. 将本项目放置于本地服务器目录下（如使用 VSCode Live Server、http-server 等）。
2. 在项目根目录下放置你的 Markdown 文件（如 `index.md`, `foo.md` 等）。
3. 访问 `index.html`，即可浏览和跳转 Markdown 文档。

## 依赖

- [marked.js](https://github.com/markedjs/marked) 用于 Markdown 解析

## 已知问题

- 若使用`CloudFlare Pages`部署时，由于找不到的页面自动返回index，所以无法验证请求的md是否存在（[示例](https://smd.shuvi.moe/#/another)），所以建议使用`CloudFlare Worker`的`static assets`方式部署
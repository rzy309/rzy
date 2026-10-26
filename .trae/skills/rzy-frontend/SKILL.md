---
name: rzy-frontend
description: rzy 项目前端开发规范。当在本仓库编写 HTML/CSS/JS 时自动遵循 rzy_ 前缀、页面注释、原生实现、fetch API 等约束。不要用于后端或非前端任务。
---

# rzy-frontend 项目前端规范

本项目所有前端输出一律遵守以下规则。遇到冲突时以本节为准。

## 命名规范（强制）

- 所有 CSS 类名必须以 `rzy_` 开头（例：`rzy_container`、`rzy_header`）
- 所有 ID 必须以 `rzy_` 开头
- 所有 JS 变量/函数必须以 `rzy_` 开头（例：`rzy_list`、`rzy_fetchData()`）

## HTML 页面注释（强制）

每个 HTML 文件顶部必须包含：

```html
<!-- 姓名：荣子祎，日期：YYYY-MM-DD，功能：功能名称 -->
```

## 技术栈约束（强制）

- 仅使用**原生** HTML / CSS / JavaScript。**禁止**引入任何第三方库或 CDN 资源（如 jQuery、Bootstrap、Tailwind、Vue、React 等）。
- 图标统一使用本仓库 `font/` 目录下的 iconfont 字体图标；未提供 iconfont 时可用内联 SVG 临时替代，但不得使用外部图标库。
- 与服务端通信**必须**使用浏览器原生 `fetch` API。禁止使用 axios / $.ajax 等封装库。

## 导航规范

- 新建的 HTML 练习页面必须加入返回 `index.html` 的超链接（文字可为"返回首页"）。
- `index.html` 导航列表应同步追加新页面链接。

## 与 agents.md 的关系

`agents.md` 是同一项目规则的人类可读版本。本 skill 是规则的可触发执行版。若两者冲突，以本节为高优先级。

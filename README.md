# Aperture Design System — 文档站

为数据密集型界面打造的暗色优先设计语言。谱系：Linear（亮度堆叠、510 字重）+ Vercel（阴影即描边）。

**在线预览**：<https://aperture-design-znl6.zai.site>

## 特点

- **零依赖单文件**：全部内容（令牌、组件、文档、交互、搜索）在 `index.html` 一个文件里，无构建步骤，克隆即用。
- **设计令牌层**：`:root` CSS 变量统一管理表面亮度阶梯、单一强调色、语义色、4px 间距栅格、圆角、动效曲线与字体栈。
- **文档章节**：概览 / 颜色系统 / 字体排版 / 间距系统 / 组件（Buttons、Inputs、Cards、Badges、Toast、Modal、Popover、Tooltip、Tabs、Breadcrumb、Progress、Pagination、Avatar、Alert）/ 图标集 / 动效系统。
- **站内搜索**：自研轻量索引（约 80 行），支持 `/` 或 `Ctrl/⌘+K` 唤起、模糊匹配、↑↓ 选择、Enter 跳转。
- **可访问性**：全局 `:focus-visible` 焦点环、skip link、`aria-live` Toast、`role=tablist` + 方向键、Modal 焦点管理、`prefers-reduced-motion` 适配。
- **移动端**：响应式布局 + 抽屉式侧边栏。

## 使用

直接用浏览器打开 `index.html`，或托管到任意静态服务器：

```bash
# 任选其一
npx serve .
python -m http.server 8080
```

## 结构

```
index.html    # 全部内容：设计令牌 → 样式 → 文档与组件 → 交互脚本
```

## License

MIT

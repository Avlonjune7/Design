# 组件与工具偏好

复用顺序：项目组件与样板 → 已安装组件库 → 最小业务组件。

| 条件 | 选择 |
| --- | --- |
| 新 React 项目尚未选库 | 优先 Astryx；项目样板优先，缺适用样板再选官方模板 |
| 新 Vue 项目尚未选库 | 优先 shadcn-vue CLI |
| 新布局或整体改版有具体设计问题 | Oil UI Pro；明确微调复用现有设计 |
| 原生 Web API、浏览器兼容性或现代实现存在具体疑问 | Modern Web Guidance 按主题检索并读取匹配指南 |
| 用户要求专项审查或出现质量疑点 | 按[网页审查](web-review.md)调用 Vercel 官方 web-design-guidelines |

Astryx 使用项目版本 CLI，已知组件先查 `component <Name> --props`，缺示例再查完整文档。每次仅选能解决当前问题的工具，已有结论足够时直接实现。

---
name: me
description: "个人 UI、浏览器验证、项目初始化、规范整理与开发工具安装偏好。用于 UI 设计与组件选型、线上登录态排查与页面验收、新项目初始化、整理项目规范及安装开发工具。"
---

# me

当前任务有更专业的 skill 时，以专业 skill 为主，me 只补充适用的个人偏好。用户当次要求和项目约定优先。

- 仅允许修改 me 技能。明确要求安装新技能时按原版安装，已有同名技能先复用。

在上述适用场景中，按当前待解决问题读取对应参考，复用已读取且仍有效的指引。UI 任务按设计判断、组件选型、性能或验证问题分别命中对应行。

| 场景 | 参考 |
| --- | --- |
| 工具选型不明确、命令故障或大量输出需要处理 | [CLI 与执行效率](references/cli-efficiency.md) |
| 初始化项目、安装开发工具、部署或整理项目规范 | [项目约定](references/project.md) |
| 前端组件选型、公共组件设计与重构或新项目 UI 初始化 | [组件与工具](references/components.md) |
| 视觉、布局或交互设计需要判断 | [视觉偏好](references/visual-ux.md) |
| 页面加载、请求、资源或渲染性能 | [页面性能](references/performance.md)，React / Next.js 使用 Vercel 官方技能 |
| 项目无可复用方向，或用户要求案例 | [设计参考](references/inspiration.md) |
| 线上登录态排查、浏览器操作、页面验收，或选择脚本与 CI 验证方式 | [验证偏好](references/verification.md)，线上登录态优先 BrowserSkill，本地独立测试优先 Playwright CLI |
| 用户要求网页专项审查，或 UI 出现质量疑点 | [网页审查](references/web-review.md)，使用 Vercel 官方技能 |

用户要求深入讨论或挑战方案时使用 grilling，讨论需文档落地时使用 grill-with-docs，复杂业务概念需梳理时使用 domain-modeling。

引用的外部技能或 CLI 可用时按需使用。缺失时沿用项目现有实现、工具与对应官方资料，讨论与文档按用户要求直接完成。影响交付或验证时说明实际缺口，安装由用户要求或项目依赖决定。

---
name: me
description: "个人开发、CLI 与 UI 偏好。用于开发、调试、重构、构建测试、项目规范、本地文件与数据处理、开发工具安装及 UI 任务。按需选择 CLI 并控制查询和输出量。"
---

# me

用户当次要求和项目约定优先。以响应速度和上下文效率为目标，只读取当前任务相关参考，复用仍有效的已核实信息。工具按需使用，局部改动走最短实现与验证路径。

本地任务优先使用适合任务的现有 CLI，调用前限定查询范围和返回内容。涉及文件检索、结构化数据、Git、数据库、构建测试或工具故障时，读取一次 [CLI 与执行效率](references/cli-efficiency.md)，后续复用。

仅允许修改 me 技能，其他技能保持原样。明确要求安装新技能时按原版安装，已有同名技能先复用。

按任务读取：

| 任务 | 参考 |
| --- | --- |
| 开发、调试、重构、项目规范或额外安装开发工具与 CLI | [项目约定](references/project.md) |
| 前端组件选型、公共组件或新项目 UI 初始化 | [组件与工具](references/components.md) |
| UI 修改或设计，含微调、新页面、布局与交互 | [视觉偏好](references/visual-ux.md) |
| 页面加载、请求、资源或渲染性能 | [页面性能](references/performance.md) |
| 项目无可复用方向，或用户要求案例 | [设计参考](references/inspiration.md) |
| 脚本、CI 或 UI 验证 | [验证偏好](references/verification.md) |
| 用户要求网页专项审查，或 UI 出现质量疑点 | [网页审查](references/web-review.md)，按相关范围检查 |

微调复用现有实现。后端任务读取开发与相关验证参考。用户要求深入讨论或挑战方案时使用 grilling，讨论需文档落地时使用 grill-with-docs，复杂业务概念需梳理时使用 domain-modeling。

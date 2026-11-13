# me

个人跨项目偏好 skill，保留具体工具选择、UI 偏好与专项验证方式，适用于 Codex 与 Claude Code。当前版本 **4.1.0**。项目约定优先，不重复 agent 的通用工作要求。

## 安装与调用

选择当前工具的一种安装位置，克隆整个仓库，保留相对目录：

| 工具 | 用户级目录 | 项目级目录 | 调用示例 |
| --- | --- | --- | --- |
| Codex | `~/.agents/skills/me/` | `.agents/skills/me/` | `$me 按我的规范完成这个功能` |
| Claude Code | `~/.claude/skills/me/` | `.claude/skills/me/` | `/me 按我的规范完成这个功能` |

例如 Codex 用户级安装：

```sh
git clone https://github.com/Avlonjune7/me.git ~/.agents/skills/me
```

Claude Code 使用相同命令并将目标替换为 `~/.claude/skills/me`。技能也可以按项目开发、设计或规范整理任务自动匹配；安装后若未出现，重新开启会话。避免在同一工具的扫描范围安装多个同名副本。

## 结构与读取

```text
me/
├── SKILL.md
├── references/
│   ├── project.md
│   ├── components.md
│   ├── visual-ux.md
│   ├── verification.md
│   ├── inspiration.md
│   └── performance.md
├── README.md
└── CHANGELOG.md
```

[SKILL.md](SKILL.md) 提供核心流程及触发条件，详细规则按任务读取：[项目开发](references/project.md)、[组件与工具](references/components.md)、[视觉与体验](references/visual-ux.md)、[验证与交付](references/verification.md)、[设计参考](references/inspiration.md)、[性能](references/performance.md)。明确微调无需加载所有参考。

README 与 CHANGELOG 仅在维护任务或项目流程需要时读取。该技能不依赖远程页面，不需要脚本、素材、MCP 或特定设计工具；`agents/openai.yaml` 为可选展示元数据。个人设计偏好已由 references 承接，不再加载旧 `~/.codex/design` 副本。

## 编写原则

只保留会改变执行选择的个人偏好与项目约定；Codex、Claude Code 等 agent 已有的通用步骤不在技能中重复展开。影响实际行为的例外仍需明确，例如居中弹窗、组件选型、环境复用及验证范围。此原则不意味着各 agent 的默认行为完全一致。

## 使用边界

按任务读取工具、UI 或专项验证偏好，不在每次交付时加载全部参考。需要明确应用时主动调用。[全局 AGENTS.md](https://github.com/Avlonjune7/codex-global-agent/blob/main/AGENTS.md) 仅保留语言、环境、技能入口与信息读取偏好；本技能不重复通用沟通、授权、安全和开发流程。

要求创建项目 AGENTS.md 时，结合实际技术栈和命令合并规则；一般开发不自动创建规范文件。

## 更新与维护

仅在明确更新技能时同步本地副本，正常任务不联网检查版本。克隆安装可在确认工作区无未提交修改后执行 `git pull --ff-only`；复制安装则同步完整技能目录。

项目代理说明可以引用技能入口，项目 DESIGN.md 继续维护项目自身决定。旧 `~/.codex/design/` 副本和已删除的 DESIGN 文档路径不自动迁移，旧项目引用应单独更新到 SKILL.md。

仅纳入经过验证的跨项目经验；项目特例留在项目中。维护技能时更新相关参考与 CHANGELOG，说明原因、范围及实际同步状态，不在执行文档中重复版本和维护记录。

版本约定：文字澄清递增补丁版本，兼容性新增递增次版本，改变既有规则含义或适用边界递增主版本。

# me

个人跨项目 UI 设计 skill，适用于 Codex 与 Claude Code。当前版本 **3.7.0**。包含条件性的个人工具偏好，用户要求、项目约束与现有技术栈优先。

## 安装与调用

选择当前工具的一种安装位置，克隆整个仓库，保留相对目录：

| 工具 | 用户级目录 | 项目级目录 | 调用示例 |
| --- | --- | --- | --- |
| Codex | `~/.agents/skills/me/` | `.agents/skills/me/` | `$me 优化这个页面` |
| Claude Code | `~/.claude/skills/me/` | `.claude/skills/me/` | `/me 优化这个页面` |

例如 Codex 用户级安装：

```sh
git clone https://github.com/Avlonjune7/me.git ~/.agents/skills/me
```

Claude Code 使用相同命令并将目标替换为 `~/.claude/skills/me`。技能也可以按 UI 任务描述自动匹配；安装后若未出现，重新开启会话。避免在同一工具的扫描范围安装多个同名副本。

## 结构与读取

```text
me/
├── SKILL.md
├── references/
│   ├── components.md
│   ├── visual-ux.md
│   ├── verification.md
│   ├── inspiration.md
│   └── performance.md
├── README.md
└── CHANGELOG.md
```

[SKILL.md](SKILL.md) 提供核心流程及触发条件，详细规则按任务读取：[组件与工具](references/components.md)、[视觉与体验](references/visual-ux.md)、[验证与交付](references/verification.md)、[设计参考](references/inspiration.md)、[性能](references/performance.md)。明确微调无需加载所有参考。

README 与 CHANGELOG 给维护者阅读，运行技能无需加载。该技能不依赖远程页面，不需要脚本、素材、MCP 或特定设计工具；`agents/openai.yaml` 为可选展示元数据。

## 更新与维护

仅在明确更新技能时同步本地副本，正常任务不联网检查版本。克隆安装可在确认工作区无未提交修改后执行 `git pull --ff-only`；复制安装则同步完整技能目录。

项目代理说明可以引用技能入口，项目 DESIGN.md 继续维护项目自身决定。旧 `~/.codex/design/` 副本和已删除的 DESIGN 文档路径不自动迁移，旧项目引用应单独更新到 SKILL.md。

仅纳入经过验证的跨项目经验；项目特例留在项目中。维护技能时更新相关参考与 CHANGELOG，说明原因、范围及实际同步状态，不在执行文档中重复版本和维护记录。

版本约定：文字澄清递增补丁版本，兼容性新增递增次版本，改变既有规则含义或适用边界递增主版本。

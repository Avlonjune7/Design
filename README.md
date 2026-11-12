# me

个人跨项目 UI 设计 skill，不绑定业务、技术栈或视觉风格。当前规范版本 **3.6.2**。

## 安装与调用

将本仓库下载或克隆到用户技能目录 `~/.agents/skills/me/`：

```sh
git clone https://github.com/Avlonjune7/me.git ~/.agents/skills/me
```

安装后在 Codex 中使用 `$me`，例如“用 $me 优化这个页面”。技能也可根据 UI 任务自动匹配；若未显示，重启 Codex。不要同时安装多个同名副本。

## 文件结构

```text
me/
├── SKILL.md
├── references/
│   ├── DESIGN-CORE.md
│   ├── DESIGN.md
│   ├── inspiration.md
│   └── performance.md
├── README.md
└── CHANGELOG.md
```

- [SKILL.md](SKILL.md)：技能入口与适用范围。
- [快速规范](references/DESIGN-CORE.md)：局部明确修改。
- [完整规范](references/DESIGN.md)：新页面与设计决策，按相关章节读取。
- [变更记录](CHANGELOG.md)：版本与历史变更。

`references/` 按任务读取，不要求全部加载。README 与 CHANGELOG 用于仓库说明，不是技能运行时必读文件。此技能只提供设计指引，无需脚本、素材或工具依赖；`agents/openai.yaml` 是可选项。

## 项目接入与维护

用户明确要求、项目约束与现有实现优先。在项目代理说明中引用 `$me` 或本仓库技能入口，保留项目自身决定，不覆盖项目专属 DESIGN.md。

仅明确更新规范时同步安装副本，不在每次任务前联网检查版本。旧 `~/.codex/design/` 副本不自动更新；需要沿用的旧项目引用应单独迁移。

仅纳入经过验证、可跨项目复用的经验；项目特例留在项目内。规则变动同步更新完整规范、快速入口及 CHANGELOG，说明原因、范围与实际同步状态。

版本约定：文字澄清递增补丁版本，兼容性新增递增次版本，改变既有规则含义或适用边界递增主版本。

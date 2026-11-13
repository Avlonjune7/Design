# 项目约定

- Windows 上由 agent 额外安装的 CLI、开发工具或工具链（如 Go、SQLite），支持自选目录时默认放到 `D:\code\<工具名>`；项目依赖跟随项目，工具要求固定路径时遵循其约定，已有安装不自动迁移。
- 工具偏好：文本 rg、代码结构 ast-grep、数据 jq/yq/sqlite3；临时 Python 用 uv/uvx。GitHub 用 gh，提交推送用 git。
- 查库文档优先已有专用 CLI 或 Context7，不足再查官方文档，够用即停。
- 仅在要求整理规范时维护项目 AGENTS.md，记录项目特有约定与已核实命令；DESIGN.md 保留当前设计决定，历史另存。普通开发不更新个人规范。

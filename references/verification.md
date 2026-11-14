# 验证偏好

- 相关工具可用且适合项目时，sh/bash 用 ShellCheck，PowerShell 用 PSScriptAnalyzer，GitHub Actions 用 actionlint。缺失工具是否安装由项目要求和具体验证需求决定。
- 本地页面与独立浏览器测试优先 Playwright CLI，真实登录态操作优先 BrowserSkill。同一页面由一个工具控制，结束时清理本任务会话。
- UI 局部改动从真实入口查看影响区域，交互改动走到操作结果。涉及布局与响应式时覆盖手机和桌面关键断点，公共组件改动抽查代表性使用页面。新增影响、失败、未解决疑点或用户要求触发扩大验证。

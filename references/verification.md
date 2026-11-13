# 验证偏好

- 相关工具可用且适合项目时，sh/bash 用 ShellCheck，PowerShell 用 PSScriptAnalyzer，GitHub Actions 用 actionlint。缺失工具是否安装由项目要求和具体验证需求决定。
- 本地页面与独立浏览器测试优先 Playwright CLI，真实登录态操作优先 BrowserSkill。同一页面由一个工具控制，结束时清理本任务会话。
- UI 局部改动查看影响区域，公共组件抽查使用页面。布局与响应式覆盖手机和桌面，主要交互从真实入口走到结果。

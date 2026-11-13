# 验证偏好

- sh/bash 用 ShellCheck，PowerShell 用 PSScriptAnalyzer，GitHub Actions 用 actionlint。
- 网页交互优先现有 Playwright CLI；需要登录态时复用对应浏览器会话。
- UI 局部改动查看影响区域，公共组件抽查使用页面；布局与响应式覆盖手机和桌面，主要交互从真实入口走到结果。

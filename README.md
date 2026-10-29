# 入画AI工作台 · 官方下载

本地优先的入画应用总启动台与个人工作台，用项目空间整理入口、便签与下一步，连接工具、看板、画布和工坊。

先行版永久免费，非开源。此仓库仅提供公开发行文件和说明，不包含工作台的私有源码或用户数据；第三方组件遵循各自许可证。

## v1.0.0 下载

[完整发行说明与校验文件](https://github.com/zhangolio/ruhua-ai-releases/releases/tag/v1.0.0)

发行状态以 Release 的实际公开状态为准；草稿阶段下载暂不可用。

| 平台 | 下载 | 使用方式 |
| --- | --- | --- |
| Windows x64 | [便携 ZIP](https://github.com/zhangolio/ruhua-ai-releases/releases/download/v1.0.0/Ruhua-AI_1.0.0_windows-x64-portable.zip) | 完整解压到可写独立目录，打开其中的「入画AI.exe」，不需要安装器；系统需有 WebView2 |
| macOS Apple Silicon / Intel | [Universal DMG](https://github.com/zhangolio/ruhua-ai-releases/releases/download/v1.0.0/Ruhua-AI_1.0.0_universal.dmg) | 将应用放入应用程序目录，不要长期从 DMG 内运行 |

工作台不捆绑独立看板、画布、工坊或付费模型服务。项目助理需自行安装 Node.js 22+、Codex CLI 并登录自己的账户，使用自己的模型额度；免费工作台功能不要求登录工作台账号。

## 更新与信任边界

- 应用内更新经用户确认，使用工作台专用公钥验证更新包。Windows 继续在当前便携根更新受管文件，不转换为 NSIS 或另装第二套程序。
- 旧内部测试版首次接入前请导出个人备份，再手动安装本版；保留原项目、工具链和系列应用等业务目录，不承诺旧测试包能识别首发新签名。
- 每版提供 `SHA256SUMS.txt`、更新包 `.sig` 与 `latest.json`。`.app.tar.gz` 是 Mac 自动更新制品，普通用户安装请选 DMG。
- Windows 暂无 Authenticode，Mac 为 ad-hoc 签名、未获 Apple Developer ID / 公证，首次打开可能收到系统安全提醒。更新完整性验签不等于操作系统发布者认证，请勿关闭系统整体安全防护。
- 本版两端由 GitHub 原生 runner 构建并验证制品；负责人接受未进行新版 Windows 实机 GUI、干净系统及真实便携升级/回滚测试。Windows 便携版暂不提供 Agent 系统桌面回复通知。

GitHub 自动显示的 `Source code` 下载只是这个发行仓库说明文件的快照，不是工作台源码。

官网：[ruhuaai.com](https://ruhuaai.com/) · 安全问题见 [SECURITY.md](SECURITY.md)。发现来源、校验和或签名异常时请停止安装并联系作者。


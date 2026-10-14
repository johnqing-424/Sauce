# last30days：模型主导，Skill 辅助

普通 `$last30days AI圈的热点` 现在直接由 Codex 选择方向、搜索、读取原文、
比较资源和判断价值。Skill 提供可选的检索适配器、证据校验、存储和预算工具。
研究不再以安装 Go、编译来源工具、修复浏览器或首次配置为前置条件。
明确的配置、诊断、原有命令和 `intelligence` 闭环仍可单独使用。

**已经安装过的用户：** [下载小更新包（约 23 KB）](https://github.com/johnqing-424/Sauce/raw/refs/heads/codex/last30days-intelligence-installer/installers/last30days-model-led-update.zip)。
完整解压，双击 `Update-Windows.cmd`。看到 `updated` 或 `already_updated` 后，
打开本机 Codex 新会话，输入原来的自然语言请求：

```text
$last30days AI圈的热点
```

小更新只替换四个说明/辅助文件，备份旧文件；现有检索实现、X 连接修补、
Go 工具、Clash 私人配置和数据库保留。未知本地修改不会被覆盖。
已有 Python 或 uv 缓存解释器可使用；更新器不会下载软件或读取 Cookie。

**首次安装：** [下载完整 Windows 包（约 16 MB）](https://github.com/johnqing-424/Sauce/raw/refs/heads/codex/last30days-intelligence-installer/installers/last30days-intelligence-model-led-windows.zip)，
解压双击 `Install-Windows.cmd`。需要 Python 3.12+。
安装位置为 `%USERPROFILE%\.agents\skills\last30days`，安装后打开本机新会话。
完整包适用于首次安装；已安装用户优先用小包以保留本地代码修补。
旧五文件联网修复包和旧完整安装包不要再覆盖新版入口。

[阅读相同普通命令的真实研究答复](examples/model-led-research/AI圈热点-实跑.md)

实跑使用了真实原生工具：5 次查询、13 次读取尝试。模型筛选三项近期发现，
读取原始公告和论文实验条件，指出价格口径、LLM 轨迹回放及未公开评测资料等
限制。所有入选原文日期都在窗口内。未声明独立复现实验或全 AI 圈热度排名。

- 原生检索阶段约 **2 分 25 秒**。
- 从读取 Skill 到研究答复保存/登记约 **7 分 23 秒**。
- 额外测试审计归档结束共 **12 分 40 秒**；该额外工作不计为普通研究响应。

这些是云端实际测量，不是 Windows 性能保证。默认研究账本阶段为 6 分钟、
18 次查询/读取；Agent 必须在检查点停止新检索，账本不能强制打断 Codex 推理
或已经运行的工具。

[查看修改、真实材料与测试范围](examples/model-led-research/实跑与验收说明.md)

独立审查及最终 255 项相关回归通过。首次完整回归中的格式和计时失败、修正
及复测范围如实保留；本次不宣称最终版本已有完全绿色的完整回归。
小包及完整包分别做云端便携安装验证；新版 Windows 实机和机器人发送未验证。
安装或更新不会启用定时任务或发送消息。

源码提交 `ba08ab1a28900507a2dfb7bc301927ab320c18e5`，独立分支
`codex/model-led-research`，基线仍为上游 3.27.2 的
`267d50f7fcbab8a6457a93ad6ca15cbc199f633c`。
源码补丁、SHA256 和旧版验证记录在 `installers/` 与 `examples/`。

# last30days 自主溯源情报系统：研究质量更新

[下载 Windows 质量更新包（约 16 MB）](https://github.com/johnqing-424/Sauce/raw/refs/heads/codex/last30days-intelligence-installer/installers/last30days-intelligence-quality-windows.zip)

已经安装过的用户也用这个完整更新包。它会备份旧 Skill，保留用户目录里的
Clash 代理配置、数据库和报告。安装不会启用定时任务或发送消息。

1. 下载并完整解压 ZIP。
2. 双击 `Install-Windows.cmd`。需要 Python 3.12+。
3. 出现 `installed` 或 `already_installed` 后，在本机 Codex 新会话中输入：

```text
$last30days intelligence discover AI
请自主选择不同探索方向，筛选 3 项值得实验的资源。
每项说明新意、用途、限制和下一步验证，引用实际原文；至少深挖一层有效关联。用中文。
```

Skill 安装到 `%USERPROFILE%\.agents\skills\last30days`。
如果之前已看到 `external_trace_verified`，继续使用现有网络配置；不要再次运行
旧五文件修复包来覆盖质量更新文件。源码补丁和 SHA256 校验文件在 `installers/`。

这次修复针对实际本机会话：个人主页被打成高价值情报、GitHub 导航混入证据、
预算被早到的候选耗尽，以及分析只有模板。新流程先收集并审阅候选，再公平分配
溯源预算，要求六项带原文引用的 Agent 分析；新 A 提醒需完成审阅后才允许入队。
元数据和主页作为发现入口，科学创新未知时明确写未知。

[查看真实检索与研究质量验证](examples/intelligence-quality/研究效果验证.md)

- [Laya-MLX：独立移植、Mac 环境限制及单机测量边界](examples/intelligence-quality/laya.md)
- [Strands Decider：决策模型及训练数据可重建限制](examples/intelligence-quality/strands.md)
- [Simreal-MLBench：开放协议及商业运行平台边界](examples/intelligence-quality/simreal.md)

报告来自授权 GitHub MCP 的真实公开原文，包含 22 处逐字匹配引用。三项入库仍是
三项；重复检查保留已验证引用的分析。旧误判中的真实个人主页已重取元数据并
正确暂存，不按高价值发现推送。这些事实不等于复现了作者实验。

最终完整回归：6580 项通过、11 项跳过、205 个 subtests 通过。未重测覆盖率。
ZIP、隔离安装、重复安装、旧版备份、私人配置/数据库保留，以及无系统时区库
时的启动均通过。测试中模拟发送与真实外部检索分别记录；真实机器人收件尚未验证。
先前完整回归的短时限测试失败已定位到测试准备/模拟范围，并修正测试，产品
超时和子进程清理规则保留。详细验证记录见示例目录的 verification.json。

当前云端 CLI 的上游候选收集被网络策略拒绝，因此这次真实检索使用已经授权的
MCP。不能据此宣称新版在 Windows 上的自主发现质量已经验证；需要安装后实跑。
旧版 Windows 安装/联网成功依据用户提供的实机输出，新版未替用户执行本机安装。

定时 CLI 可收集、溯源和保存，深入语义分析需要 Agent 参与；缺少审阅不会生成新
A 提醒。默认 A/B 阈值为 65/60；旧私人配置的显式阈值保留。评分仍是启发式代理，
尚未证明可以客观衡量科学突破。下一阶段优先补充后台 Agent 调度和语义价值校准。

源码基线为 267d50f7fcbab8a6457a93ad6ca15cbc199f633c，上游版本 3.27.2，
本次未合并后续上游版本。质量更新源码提交 2f498f844f21c560e52d0d69f9bfdc4ff2cb5483，在独立分支上开发。
恢复版和网络修复历史仍保留在旧包/补丁及 Clash 说明中。

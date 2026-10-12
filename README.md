# last30days 自主溯源情报系统：Windows 安装包

[下载 Clash / Mihomo 联网修复包（约 25 KB）](https://github.com/johnqing-424/Sauce/raw/refs/heads/codex/last30days-intelligence-installer/installers/last30days-clash-repair.zip)

如果已经安装成功，但 GitHub 因 `198.18.*` 非公开地址而失败：保持 Clash 开启，
解压修复包，双击 `Repair-Clash.cmd`。它会备份受支持的文件、验证本机代理、保存
Skill 私有配置并自动执行真实 GitHub 溯源。看到 `external_trace_verified` 才表示
本机取到了当前证据；旧报告不能使失败刷新显示成功。具体恢复步骤见
[Clash 修复说明](installers/Clash-修复说明.md)。

[下载 Windows 安装包](https://github.com/johnqing-424/Sauce/raw/refs/heads/codex/last30days-intelligence-installer/installers/last30days-intelligence-windows.zip)

1. 下载并完整解压 ZIP。
2. 双击 `Install-Windows.cmd`。需要 Python 3.12+；已有 uv 时可通过 uv 准备 Python。
3. 出现 `installed` 或 `already_installed` 后，在本机 Codex 新会话中输入：

```text
$last30days intelligence trace https://github.com/mvanhorn/last30days-skill
```

Skill 安装到当前 Windows 用户的 `%USERPROFILE%\.agents\skills\last30days`。
已有 Skill 会自动备份。安装包附官方 tzdata 时区数据；安装不会启用定时任务或发送消息。

此包包含基于 last30days-skill 的自主发现、资源溯源、证据图、SQLite 去重和通知接口。
恢复源码提交为 `fbb6861`；原基线为 `267d50f7fcbab8a6457a93ad6ca15cbc199f633c`。
本次 Clash 兼容修复对应源码提交 `2f2107e`，完整源码补丁包含两阶段修改。
通知模块部分丢失记录按原契约重建，不能视为原提交 `34fc4bb` 的逐字节副本。
源码补丁与 SHA256 校验文件在 `installers/`。

恢复版完整回归：6378 项通过，11 项跳过，覆盖率 84.08%。ZIP 校验、隔离安装、
重复安装与缺少系统时区数据库时的启动已验证。Windows 安装与本机 Skill 加载已经
由用户实机确认。修复后的 Windows 实机输出也确认代理配置成功并取得 4 份资源、
4 条证据，状态 `external_trace_verified`；部分关联资料仍有 HTTP 403 或预算限制。
此结论依据用户提供的实机终端结果，云端未独立读取 Windows 报告文件。
真实消息收件仍未验证。
本次代理修复定向回归 241 项通过，独立复查的 110 项代理/修复/来源检查通过。
最终完整回归 6409 项通过、11 项跳过、205 个 subtests 通过；没有重新测量覆盖率。
修改后的真实云端 GitHub 测试取回 4 份资源、4 条证据；API 被既定云端策略拒绝，
报告保留来源未知状态。这不等于 Windows Clash 联网成功。

修复包仅更新五个版本匹配的公开文件；保留 TLS、地址与托管网络策略限制，
不改变 Windows/Clash 设置，不读取订阅或浏览器 Cookie，不启用任务或发送消息。

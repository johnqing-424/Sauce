# last30days 自主溯源情报系统：Windows 安装包

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
通知模块部分丢失记录按原契约重建，不能视为原提交 `34fc4bb` 的逐字节副本。
源码补丁与 SHA256 校验文件在 `installers/`。

恢复版完整回归：6378 项通过，11 项跳过，覆盖率 84.08%。ZIP 校验、隔离安装、
重复安装与缺少系统时区数据库时的启动已验证；Windows 实机安装和真实收件尚未验证。

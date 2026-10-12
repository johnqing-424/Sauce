# Clash 本机联网修复

适用于已经安装 last30days 情报 MVP、使用 Clash / Clash Verge / Mihomo，
且 GitHub 因 `198.18.*` 非公开地址而无法溯源的 Windows 电脑。

1. 保持 Clash 开启。
2. 完整解压此 ZIP，双击 `Repair-Clash.cmd`。
3. 等待三个步骤结束。出现 `external_trace_verified` 表示真实 GitHub 证据已经
   取回；`source_failures` 会保留其他未成功来源，不能当作全部资源已验证。
4. 在本机 Codex 输入 `$last30days intelligence discover robotics`，或描述领域。

修复器需要 Python 3.12+。它仅替换支持版本中的五个公开 Skill 文件，校验 SHA256
和 Python 语法；不同或自定义版本会拒绝覆盖。原文件备份在用户 Skill 目录旁的
`.last30days-network-backup-日期-随机值`。磁盘写入失败时会恢复已替换文件。
已有 SQLite、报告、通知凭据和其他设置保留。代理配置的旧 JSON 另有私有备份。

程序读取 Windows 注册表的代理端口提示，并最多尝试四个数字回环候选，包括常见
7897/7890。只有实际 GitHub HTTPS 成功才写 `local_proxy_url`。自定义端口可从终端
运行 `Repair-Clash.cmd --proxy http://127.0.0.1:实际端口`，无需提供代理订阅或密码。
配置写入 `LAST30DAYS_INTEL_CONFIG` 指定文件，或当前用户
`%USERPROFILE%\.config\last30days\intelligence.json`；此用户文件会被以后调用自动加载。

仅支持数字回环 HTTP/mixed 代理，不支持 SOCKS、代理认证或远程代理。仅已明确列出
的公共平台通过代理解析；未知网站仍可能因 Fake-IP 被拒绝。源站 TLS 检查保留；
证据会明确记录地址解析由可信本机代理承担，不能验证代理远端地址。修复不会绕过
托管云端网络策略、关闭地址检查、更改 Clash 设置或启用系统代理。

不发送消息、不启用定时任务。真实推送仍需你的消息目标和凭据。

如需恢复：关闭运行中的研究任务，将文件备份中的五个文件复制回原 Skill 目录；
若存在配置备份，把它复制回原配置文件。没有旧配置备份时，可从用户 JSON 中删除
`local_proxy_url` 或设为 `null`。不要把私人配置内容发到公开仓库。

发布前验证包括模拟 Fake-IP/代理测试、证书与跳转限制、真实临时文件备份/回滚及
修复 ZIP 完整性。云端不能连接你的 Clash；Windows 实际联网结论以步骤三输出为准。

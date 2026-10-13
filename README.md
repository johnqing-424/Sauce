# last30days：Codex 原生研究能力优先更新

[下载 Windows 更新包（约 16 MB）](https://github.com/johnqing-424/Sauce/raw/refs/heads/codex/last30days-intelligence-installer/installers/last30days-intelligence-native-windows.zip)

这次更新修复了“在别的 Codex 会话里研究效果明显变差”的流程问题：
Skill 现在优先让 Codex 使用已连接的搜索、GitHub 和网页工具来发现候选、读原文、
比较已有方法，再交给 Python 校验证据、追踪关系、去重入库和生成中文简报。
原 last30days 的平台发现能力保留。

已经安装过的用户也使用这个完整更新包。

1. 下载并完整解压 ZIP。
2. 双击里面的 `Install-Windows.cmd`。需要 Python 3.12+。
3. 出现 `installed` 或 `already_installed` 后，在本机 Codex **新会话**输入：

```text
$last30days intelligence discover AI
```

安装位置为 `%USERPROFILE%\.agents\skills\last30days`。更新会备份旧 Skill，保留
用户目录中的 Clash 配置、数据库和报告。已有联网配置可继续使用；不要再用旧的
五文件联网修复包覆盖新版。安装不会启用定时任务或发送消息。

新版要求先扩展候选，再筛选值得实验的资源；每项需读取至少一层有效关联，
说明发现、新意、用途、限制和下一步验证，并引用实际取得的原文。
比较用的背景资料不再混入原始来源或抬高分数。用户无需手写分析 JSON。
如果会话缺少相应工具或检索受限，报告会说明缺口；不同会话的连接权限和工具
仍可能不同，不能保证所有环境都有相同的检索覆盖。

403 的原因需要看具体响应。Python 的匿名 GitHub API 请求与 Codex 已授权的
GitHub 连接使用不同的认证和网络路径；一个失败不代表另一个不可用。新版记录
可核验的配额信息，不把所有 403 都解释为凭据错误。网络地址拦截也与 HTTP 403
分别报告，现有 TLS 和地址检查保留。

[查看真实检索、失败记录与修复验证](examples/intelligence-native/验证说明.md)

- [中文研究简报](examples/intelligence-native/研究简报.md)
- [KVShareArena：缓存复用评测及可复现性限制](examples/intelligence-native/kvshare.md)
- [SkillsBench：技能评测和具体任务检查，作为背景资源暂存](examples/intelligence-native/skillsbench.md)
- [OriginBlame：数据来源定位与模型遗忘的边界，作为旧资源暂存](examples/intelligence-native/originblame.md)

实际 Codex 原生检索得到 20 个候选。初次提交暴露的导入和分析引用问题已经修复；
同一批真实原文重放后生成 3 份报告、18 项分析、24 处逐字匹配引用。
重复运行仍为 3 个事件、3 个修订，没有通知记录。
两项较旧资源按 `hold` 保存，未包装成近期突破。材料分数仍是启发式代理，
科学创新和作者实验的正确性需要独立验证。

完整回归为 6601 项通过、11 项跳过、205 个 subtests 通过。
ZIP 文件完整性、隔离安装、重复安装、旧版备份、私人配置/数据库保留、
无系统时区库时的启动及安装包内的真实材料重放均通过。
这些检查在 Linux 云端完成；**本次新版 Windows 实机执行、真实机器人发送尚未验证**。
新检索与保存材料重放的结果分别记录，不将重放宣称为新一轮外部搜索。

源码提交：`8b122d47e60e2889080bd1c3393e0487fe0b9eac`，分支
`codex/intelligence-native-discovery`。基线为
`267d50f7fcbab8a6457a93ad6ca15cbc199f633c`（上游 3.27.2）。
源码补丁与 SHA256 校验在 `installers/`；旧安装包和历史验证仍保留。
原有定时 CLI 可以收集、追踪和保存；深入语义研究仍需 Agent 运行环境，
本次没有启用无人值守调度。

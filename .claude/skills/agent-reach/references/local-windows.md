# Sauce 项目 Windows 运行与报告交付

仅适用于 `E:\Sauce` 项目及其子目录中的本地对话。Skill 位于
`E:\Sauce\.agents\skills\agent-reach`，安装位置是 `E:\Sauce\Agent-Reach`。
不要把本项目配置、盘符、代理或 Chrome 会话推广到其他项目、用户级目录或云端。

## 运行入口

使用完整路径；本项目没有向用户 PATH 或 PowerShell profile 注册命令。

```powershell
& 'E:\Sauce\Agent-Reach\bin\agent-reach.exe' doctor --json
& 'E:\Sauce\Agent-Reach\bin\mcporter.exe' --config 'E:\Sauce\Agent-Reach\config\mcporter.json' call exa.web_search_exa query='检索问题' numResults=5
& 'E:\Sauce\Agent-Reach\bin\opencli.exe' reddit search '检索问题' -f json --window background --site-session ephemeral --keep-tab false
& 'E:\Sauce\Agent-Reach\bin\bili.exe' search '检索问题' --type video -n 5 --json
& 'E:\Sauce\Agent-Reach\bin\gh.exe' search repos '检索问题' --limit 5
& 'E:\Sauce\Agent-Reach\bin\opencli.exe' boss search '检索问题' --city 北京 --limit 15 -f json --window background
& 'E:\Sauce\Agent-Reach\bin\opencli.exe' boss detail '<security_id>' -f json --window background
```

Boss直聘优先用 OpenCLI 的 `boss` 适配器，复用用户日常 Chrome 的登录态（2026-10-28
验证 `whoami` 为 geek 已登录，`search` 和 `detail` 返回完整职位与 JD）。只做只读命令；
greet/send/exchange/batchgreet 等写操作需用户明确要求。Doctor 的 Boss 检查只看
boss-agent-cli + CDP 9222，显示 off 不代表 OpenCLI 路线不可用。

项目 Exa 配置在 `E:\Sauce\Agent-Reach\config\mcporter.json`。使用明确的 `--config`
避免工作目录影响配置选择；不要覆盖用户级或其他项目配置。其他 mcporter
服务器仍按用户或项目自己的配置调用。Exa 限额耗尽时转向可用的搜索/官网阅读渠道并记录
覆盖限制，不自动重复配置或升级。

原生 `.exe` 启动器会选择本套 Python/Node 依赖、处理 UTF-8，并在未设置代理时使用
现有 Clash `http://127.0.0.1:7897`。Chrome 和 Clash 需运行；只有实际内容读取失败且
确认登录有帮助时才请用户登录。不要要求已经登录的用户重复交出 Cookie。

## 已验证的后端与回退

- X、Reddit、小红书优先使用 OpenCLI 已连接的 Chrome 会话。Doctor 的 warn/null 可能
  表示未进行实时登录验证；用一次实际只读命令判断，不能仅凭该状态重装。
- 本机 Jina Reader 返回 HTTP 401。已知网页可用公开网页读取工具，或创建自己的
  OpenCLI 后台 browser session，先 `open` 再 `extract`，结束后 `close`。
- 本机 YouTube 匿名 yt-dlp 被阻止。优先 OpenCLI 的 `youtube video` 与
  `youtube transcript`；先查看对应 `--help`，返回值是记录数组。
- 小红书搜索可用，`note` 可能拒绝导航。保留搜索返回的完整签名 URL，使用自己的
  后台 browser session 打开，再读取
  `E:\Sauce\Agent-Reach\.runtime\xhs-note-extract.js` 并执行其只读提取。
  使用正文前确认 `loginWall/securityBlock/notFound` 为 false，标题与正文非空。
- 安装包含已验证的 OpenCLI 小红书、YouTube 和 Reddit search 适配修复；重新安装会覆盖它们。
  Reddit search 改为解析 `/search/` 网页（JSON 接口返回 403），原文件为
  `.runtime/checks/reddit-search-1.8.8-original.js`。
- OpenCLI doctor 显示 `Extension: not connected` 而 Chrome 已打开时，先运行
  `opencli daemon restart`，扩展会自动重连。
  普通研究任务不要顺便升级。关闭自己创建的标签，不影响用户原有标签。

## 报告交付

用户提出研究、调研或报告需求时，完成采集、源头核实和分析后，交付可打开的文档。
格式未指定时默认 Markdown，并在最终回复提供文件链接和重点结论。简单事实查询、
只要链接或明确要求简短聊天答复时，按用户要求，不强制生成文件。

用户指定 Word/PDF 等格式时，继续使用当前环境可用的对应文档技能和工具。
Agent-Reach 的“只负责获取内容”是职责划分，不能作为拒绝或停止文档交付的理由；
不要要求用户再发一次指令才开始写报告。

报告保存到用户指定位置，否则保存到当前对话的可写目录；命名包含主题和日期。
临时采集数据放 `C:\Users\ACER\.agent-reach\research\` 等缓存位置，与交付物分开。
正文说明检索时间范围、核心结论和直接来源，区分事实与推断，标明影响结论的采集限制。
不要把摘要、标题或厂商跑分当作未核实的事实。保存后确认文件存在且内容可读取。

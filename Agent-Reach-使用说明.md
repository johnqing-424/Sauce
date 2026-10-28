# Agent-Reach 本机安装与使用

安装日期：2026-10-14。

Git 仓库根目录是 `E:\Sauce`，项目源码和独立运行环境位于其 `Agent-Reach` 子目录。
根目录的 `AGENTS.md`、`CLAUDE.md` 和两套项目 Skill 都由同一个 Git 仓库直接管理。

Agent-Reach 版本为 1.5.0，上游源码基于提交
`94f06c1969dfc1834001269d79d3ad0972d9dee6`。OpenCLI 为 1.8.8，
mcporter 为 0.14.3，GitHub CLI 为 2.102.0。

Codex Skill 已注册到 `E:\Sauce\.agents\skills\agent-reach`，仅在 Sauce 项目使用。
Claude Code 的项目 Skill 位于 `E:\Sauce\.claude\skills\agent-reach`。
账号配置使用各工具的默认用户目录；
程序、Python 虚拟环境和 Node 工具均位于上述 E 盘安装目录。

## 已完成的实际验收

| 渠道 | 已验证的能力 |
|---|---|
| X / Twitter | Chrome 登录态搜索，返回真实推文及来源链接 |
| Reddit | 搜索返回 3 个帖子；读取帖子及评论，返回 91 条记录 |
| 小红书 | 搜索返回 3 条笔记；浏览器备用路线读取标题、作者、正文和互动数据，样例正文 472 字 |
| YouTube | Chrome 路线读取视频信息和 2,955 段英文字幕 |
| Exa | MCP 语义搜索实际返回文档来源 |
| GitHub | CLI 已授权 johnqing-424，仓库 API 读取成功 |
| B站 | 无需登录的视频搜索返回结果 |
| RSS / Atom | 解析仓库动态订阅源，返回 20 条记录 |
| 网页正文 | OpenCLI 浏览器提取已通过 |

验收数据保存在 `E:\Sauce\Agent-Reach\.runtime\checks`。

## 在 Codex 中使用

在 Sauce 项目中新建对话即可使用 `$agent-reach`，例如：

```text
$agent-reach 调研最近一周 AI Agent 的重要进展，结合官网、GitHub、X、Reddit、B站和小红书，追踪原始来源，交叉核验后输出完整研究报告，并附来源链接。
```

使用时保持 Chrome、OpenCLI 扩展和 Clash 运行。已验证的本机代理为
`http://127.0.0.1:7897`，启动器会为工具进程设置代理。

PowerShell 中可以直接调用本机入口：

```powershell
& 'E:\Sauce\Agent-Reach\bin\agent-reach.exe' doctor --json
& 'E:\Sauce\Agent-Reach\bin\opencli.exe' reddit search 'OpenAI Codex' --limit 5 -f json
& 'E:\Sauce\Agent-Reach\bin\mcporter.exe' --config 'E:\Sauce\Agent-Reach\config\mcporter.json' call exa.web_search_exa query='AI Agent' numResults=5
```

## 本机修补与已知限制

Windows 入口使用原生 `.exe` 启动器，通过参数数组调用工具，已验证 `%`、`&`
和完整 URL 参数可以保留。入口使用上述完整路径，不向用户 PATH 或 PowerShell
profile 自动加载。2026-10-15 已撤回用户级通用配置，保留项目内运行和报告交付。

小红书搜索已应用 [OpenCLI 上游修复](https://github.com/jackwener/OpenCLI/commit/0f8fd4470793e141e7df2146a2008dbbca830db8)，
修正透明重复筛选控件导致的误判。YouTube 字幕适配器已修正冗余主页导航。
原始适配器备份位于 `.runtime/checks`；重新安装 OpenCLI 会替换这些文件，
更新后需要重新验证。

小红书标准 `note` 命令当前仍会拒绝详情页导航，正文使用已验证的浏览器备用路线。
对应操作已写入 `E:\Sauce\AGENTS.md`，并保存了上游只读正文提取脚本。

当前网络出口被 Jina 拒绝匿名读取；匿名 yt-dlp 访问 YouTube 也被要求登录。
本机已采用 Chrome 读取网页和 YouTube 的路线。

`doctor` 会保守地显示部分已登录渠道为 `warn`，也可能只根据工具配置显示 `ok`。
实际可用性以本次保存的搜索、正文和字幕验收结果为准。

参考：[项目安装说明](https://github.com/Panniantong/Agent-Reach/blob/main/docs/install.md)、
[OpenAI 官方 Skill 文档](https://learn.chatgpt.com/docs/build-skills)。

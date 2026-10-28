# Local Agent Reach installation

Agent Reach is installed at `E:\Sauce\Agent-Reach`. Its project-scoped Skill is
registered at `E:\Sauce\.agents\skills\agent-reach\SKILL.md`.
Use it only in the Sauce project and its subdirectories. Read its
`references/local-windows.md` for this project's runtime and report delivery.
Do not register the skill, launchers, or report rules at user scope.

## Skill 双副本同步规则（Codex 与 Claude Code 共同遵守）

本项目的 Skill 有两份副本：Codex 读取 `E:\Sauce\.agents\skills\`，Claude Code 读取
`E:\Sauce\.claude\skills\`。两份必须始终逐字节一致。

- 修改、新增或删除任一副本中的 Skill 文件后，在同一次任务内把相同改动同步到另一份副本。
- 同步后逐个文件比对两侧（含新增和删除的文件），确认完全一致后再结束任务，并在回复中说明已同步。
- 发现两侧不一致而不确定哪份更新时，先列出差异并询问用户，不要自行覆盖。
- 本 `AGENTS.md` 是两边共用的规则源；`CLAUDE.md` 只通过 `@AGENTS.md` 引用它，规则只改这里。

Use the launchers in `E:\Sauce\Agent-Reach\bin` from PowerShell, for example:

```powershell
& 'E:\Sauce\Agent-Reach\bin\agent-reach.exe' doctor --json
& 'E:\Sauce\Agent-Reach\bin\mcporter.exe' --config 'E:\Sauce\Agent-Reach\config\mcporter.json' call exa.web_search_exa query='query' numResults=5
& 'E:\Sauce\Agent-Reach\bin\opencli.exe' reddit search 'query' -f yaml
```

The launchers select this installation's Python and Node tools and use the
existing local Clash proxy at `http://127.0.0.1:7897` when no proxy environment
variables are already set. Keep Clash running for external sites and Chrome
open for the OpenCLI browser session.

For X, Reddit and Xiaohongshu, prefer the configured OpenCLI browser session.
Validate each platform with an actual read-only command; a Doctor warning can
mean that credentials were intentionally not tested. Preserve complete URLs
from platform search results. Follow the upstream Skill's credential rules.

Prefer OpenCLI for YouTube metadata and transcripts on this machine. The
anonymous yt-dlp route was blocked by YouTube, while the Chrome route returned
video metadata and 2,955 English subtitle segments.

Known working fallbacks on this installation:

- Jina Reader returns HTTP 401 for this network exit. Read webpages with an
  owned OpenCLI browser session: `browser <session> open <url> --window background`,
  then `browser <session> extract`, then `browser <session> close`.
- The Xiaohongshu `note` adapter can reject detail-page navigation even though
  the same signed URL works in the browser. Open its full URL in an owned
  browser session, then evaluate the upstream read-only note extractor saved at
  `E:\Sauce\Agent-Reach\.runtime\xhs-note-extract.js`. Verify `loginWall`,
  `securityBlock` and `notFound` before using the returned `title` and `desc`.
  Release the session with `browser <session> close` afterwards.

OpenCLI 1.8.8 has three verified local repairs: Xiaohongshu search uses the
upstream fix from commit `0f8fd4470793e141e7df2146a2008dbbca830db8`; the YouTube
transcript adapter skips redundant homepage pre-navigation; Reddit search parses
the `/search/` web page because `/search.json` and `/by_id/*.json` now return
HTTP 403 (verified 2026-10-28). Originals are in
`.runtime/checks/`. An OpenCLI reinstall replaces these adapter files, so verify
the repairs again when updating. Installed tool entry points are native `.exe`
launchers; use them to preserve signed URL query parameters.

Do not log cookies or tokens. Save credentials through the tool's explicit
configuration commands. Keep reports and diagnostics free of credentials.

For research/report requests in this project, finish gathering, verification,
analysis, and document delivery. Default to a sourced Markdown report in the
requested location or this chat's writable project directory, unless the user
requests another format or a short chat answer. Use the available document
tools for Word/PDF. Collection-cache rules do not prohibit requested reports.

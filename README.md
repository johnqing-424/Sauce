# Sauce

Agent-Reach 源码与本项目的 Codex、Claude Code 配置工作区。Git 仓库根目录是
`E:\Sauce`，源码保存在 `Agent-Reach/`。

## 项目文件

- [AGENTS.md](AGENTS.md)：Codex 与 Claude Code 共用的项目规则。
- [CLAUDE.md](CLAUDE.md)：通过 `@AGENTS.md` 引用共用规则。
- [.agents/skills/](.agents/skills/) 与 [.claude/skills/](.claude/skills/)：两套内容一致的项目技能。
- [Agent-Reach/](Agent-Reach/)：源码、测试、上游文档和许可证。
- [本机安装与使用说明](Agent-Reach-使用说明.md)：Windows 运行环境与工具入口。

Git 操作在仓库根目录进行。Agent-Reach 的安装、构建和测试在 `Agent-Reach/`
目录进行；GitHub Actions 已配置相同的工作目录。

研究报告放在 `reports/`，运行环境、下载工具、凭据及缓存通过 `.gitignore`
排除。它们保留在本机，不作为项目源码提交。

Agent-Reach 的上游来源和署名保留在其文档中，代码遵循 [MIT 许可证](LICENSE)。

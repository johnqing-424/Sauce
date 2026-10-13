# strands-labs/strands-decider

Generated: 2026-10-13T01:11:43.340341+00:00
Value proxy: 60.75/100 · Delivery tier: B
Verification: primary_material_retrieved; experiments_not_independently_verified

## Discovery

Strands Decider 提供选择与评分的决策模型及可靠性分数。最值得试的是把不确定决策交回人或较大模型，而不是把置信度直接当真实性。

## Three source roles

Origin status: primary_resource_verified
Earliest retrieved dated record: https://github.com/strands-labs/strands-decider (2026-09-29T16:36:38Z); global earliest is unknown.
Creator-direct records: https://github.com/strands-labs/strands-decider
Underlying resources: https://github.com/strands-labs/strands-decider

## Claims and facts

- [unverified] Original observation has no claim text.
- [primary_document_confirmed] Primary repository retrieved: strands-labs/strands-decider

## Verifiable evidence

### repository: strands-labs

https://github.com/strands-labs/strands-decider
Published: 2026-09-29T16:36:38Z; version: unknown
Retrieved: 2026-10-12T08:22:32+00:00; location: text:chars:239-639; SHA256: aeda3dc07320b1745d021d9153dded1f948097be7b7972afebaf0484f167c5f2
Status: primary_document_retrieved; freshness: host_observed_snapshot

> <div align="center">
>   <div>
>     <a href="https://strandsagents.com">
>       <picture>
>         <source media="(prefers-color-scheme: dark)" srcset="https://strandsagents.com/latest/assets/wordmark-github-dark.svg">
>         <img src="https://strandsagents.com/latest/assets/wordmark-github-light.svg" alt="Strands" width="320">
>       </picture>
>     </a>
>   </div>
>
>   <h1>Strands Decider</h1>
>
>   <h2>A sm
Host-reported retrieval: github.fetch (authorized MCP); HTTP status unknown; CLI transport/DNS/TLS not independently verified.
Host-reported retrieval: github.fetch (authorized MCP); HTTP status unknown; CLI transport/DNS/TLS not independently verified.

### documentation: unknown

https://github.com/strands-labs/strands-decider/blob/main/evaluation/results.md
Published: unknown; version: unknown
Retrieved: 2026-10-12T08:22:32+00:00; location: text:chars:0-399; SHA256: 3c353cf34ea9d348f5ff950e6ed4698f84cf4b2fbed4b4f05e7def82c0f17fa9
Status: document_retrieved; freshness: host_observed_snapshot

> # Results
>
> The measurements of v1 (the released model), the Gemma 4 v1 models, v21, v19 and the versions
> before them: the seeds and release checks of v1, the Gemma 4 v1 models and v21, the AWS retrain, the summary by version,
> calibration, and accuracy and latency on a Mac. [README.md](README.md) says how to run them, and
> [jevbench.md](jevbench.md) has the external benchmark. Paths are relative to
Host-reported retrieval: github.fetch (authorized MCP); HTTP status unknown; CLI transport/DNS/TLS not independently verified.

### repository: unknown

https://github.com/strands-agents/harness-sdk
Published: unknown; version: unknown
Retrieved: 2026-10-13T01:04:47.508868+00:00; location: text:chars:0-400; SHA256: f15717bcaf1a02195fec34812271f298355dea11799228e2e071321056629c31
Status: document_retrieved; freshness: historical_not_revalidated

> Strands Agents
> A model-driven approach to building AI agents in just a few lines of code.
> Documentation
> ◆ Samples
> ◆ MCP Server
> ◆ Discord
> Strands Agents is an open-source SDK for building and running AI agents in Python and TypeScript. Choose Strands when you would otherwise write your own agent loop: it runs in your process with no hosted control plane, and it covers the jobs a hand-rolled loop gr

## Value and uncertainty

作者声称在未见过的短分类任务上，置信度至少 0.9 的回答约有 95% 正确。若能在目标分布复现，可靠性分数可用于拒答或升级路由；目前只是作者评测。
可先调查 CPU 路径，用固定标签任务测试分类、工具路由与拒答。CPU 文档使它比仅限 MLX 的实现更值得在你的电脑上调查；Windows 兼容性尚未验证。

- No independent replication or experimental fact verification was performed.
- Earliest public record is scoped to retrieved records; global priority is unknown.
- Novelty, originality and practical value are heuristic proxies, not proved breakthroughs.
- Some linked resources could not be retrieved; the evidence chain is partial.
- Agent assessment is an evidence-linked interpretation, not independent fact or experiment verification.
- 评测文件说明训练数据构建代码尚未全部进入 main，现阶段无法从 main 重建该训练集。可靠性是否能迁移到你的领域、误差成本和硬件性能均未知。

## Evidence-linked Agent assessment

AI interpretation; not independent verification.

### Finding

Strands Decider 提供选择与评分的决策模型及可靠性分数。最值得试的是把不确定决策交回人或较大模型，而不是把置信度直接当真实性。

https://github.com/strands-labs/strands-decider
Location: text:chars:1557-1632; SHA256: aeda3dc07320b1745d021d9153dded1f948097be7b7972afebaf0484f167c5f2
> a decision model picks between sets of options and
> rates things on a scale.

### New

关联评测记录说明版本调整了训练数据混合等设置，属于可追踪的具体版本变化；相对全部先前研究的创新程度仍未知。

https://github.com/strands-labs/strands-decider/blob/main/evaluation/results.md
Location: text:chars:679-738; SHA256: 3c353cf34ea9d348f5ff950e6ed4698f84cf4b2fbed4b4f05e7def82c0f17fa9
> **A balanced data mix** of 246,678 rows, about twice v21's:

### Why it matters

作者声称在未见过的短分类任务上，置信度至少 0.9 的回答约有 95% 正确。若能在目标分布复现，可靠性分数可用于拒答或升级路由；目前只是作者评测。

https://github.com/strands-labs/strands-decider
Location: text:chars:2451-2523; SHA256: aeda3dc07320b1745d021d9153dded1f948097be7b7972afebaf0484f167c5f2
> answers at a confidence of 0.9 or more are right
>   about 95% of the time

### Application potential

可先调查 CPU 路径，用固定标签任务测试分类、工具路由与拒答。CPU 文档使它比仅限 MLX 的实现更值得在你的电脑上调查；Windows 兼容性尚未验证。

https://github.com/strands-labs/strands-decider
Location: text:chars:3041-3098; SHA256: aeda3dc07320b1745d021d9153dded1f948097be7b7972afebaf0484f167c5f2
> The `cuda`, `mps` and `cpu` extras name the other devices

### Limitations

评测文件说明训练数据构建代码尚未全部进入 main，现阶段无法从 main 重建该训练集。可靠性是否能迁移到你的领域、误差成本和硬件性能均未知。

https://github.com/strands-labs/strands-decider/blob/main/evaluation/results.md
Location: text:chars:2078-2126; SHA256: 3c353cf34ea9d348f5ff950e6ed4698f84cf4b2fbed4b4f05e7def82c0f17fa9
> the training
> data cannot be rebuilt from `main`.

### Next steps

建立自己的保留测试集，记录各置信度区间的正确率、拒答率和延迟，再与生成式路由比较；先核对当前发布版本和训练数据可重建程度。

https://github.com/strands-labs/strands-decider
Location: text:chars:2451-2523; SHA256: aeda3dc07320b1745d021d9153dded1f948097be7b7972afebaf0484f167c5f2
> answers at a confidence of 0.9 or more are right
>   about 95% of the time

https://github.com/strands-labs/strands-decider/blob/main/evaluation/results.md
Location: text:chars:2078-2126; SHA256: 3c353cf34ea9d348f5ff950e6ed4698f84cf4b2fbed4b4f05e7def82c0f17fa9
> the training
> data cannot be rebuilt from `main`.

## Observed relationship chain

- https://github.com/strands-labs/strands-decider → [readme] https://github.com/strands-labs/strands-decider/blob/main/README.md (host:paired_snapshot_url; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [references] https://strandsagents.com/ (host:text:L3; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [references] https://strandsagents.com/latest/assets/wordmark-github-dark.svg (host:text:L5; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [references] https://strandsagents.com/latest/assets/wordmark-github-light.svg (host:text:L6; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [references] https://github.com/strands-labs/strands-decider/graphs/commit-activity (host:text:L16; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [references] https://img.shields.io/github/commit-activity/m/strands-labs/strands-decider (host:text:L16; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [references] https://github.com/strands-labs/strands-decider/issues (host:text:L17; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [references] https://img.shields.io/github/issues/strands-labs/strands-decider (host:text:L17; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [references] https://github.com/strands-labs/strands-decider/pulls (host:text:L18; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [references] https://img.shields.io/github/issues-pr/strands-labs/strands-decider (host:text:L18; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [references] https://discord.gg/Wa4CQrxsP (host:text:L19; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [references] https://img.shields.io/badge/Discord-Join-5865F2?logo=discord&logoColor=white (host:text:L19; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [code] https://github.com/strands-agents/sdk-python (host:text:L32; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [documentation] https://github.com/strands-labs/strands-decider/blob/main/evaluation/results.md (host:text:L39; target retrieved: True)
- https://github.com/strands-labs/strands-decider → [documentation] https://github.com/strands-labs/strands-decider/blob/main/docs/inference.md (host:text:L53; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [documentation] https://github.com/strands-labs/strands-decider/blob/main/docs/vision.md (host:text:L188; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [documentation] https://github.com/strands-labs/strands-decider/blob/main/docs/naming.md (host:text:L205; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [references] https://huggingface.co/StrandsAgents (host:text:L207; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [references] https://huggingface.co/amazon (host:text:L209; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [references] https://huggingface.co/StrandsAgents/strands-decider-E2B-gemma4-v1-2610 (host:text:L219; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [references] https://huggingface.co/StrandsAgents/strands-decider-E4B-gemma4-v1-2610 (host:text:L220; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [references] https://huggingface.co/StrandsAgents/strands-decider-12B-gemma4-v1-2610 (host:text:L221; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [references] https://huggingface.co/StrandsAgents/strands-decider-26B-A4B-gemma4-v1-2610 (host:text:L222; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [code] https://github.com/strands-labs/strands-decider (host:text:L238; target retrieved: True)
- https://github.com/strands-labs/strands-decider → [documentation] https://github.com/strands-labs/strands-decider/blob/main/data/sources.md (host:text:L266; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [documentation] https://github.com/strands-labs/strands-decider/blob/main/README.md (host:text:L279; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [references] https://huggingface.co/Qwen (host:text:L284; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [documentation] https://github.com/strands-labs/strands-decider/blob/main/docs/architecture.md (host:text:L310; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [documentation] https://github.com/strands-labs/strands-decider/blob/main/evaluation/README.md (host:text:L320; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [documentation] https://github.com/strands-labs/strands-decider/blob/main/evaluation/jevbench.md (host:text:L321; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [documentation] https://github.com/strands-labs/strands-decider/blob/main/examples/strands/README.md (host:text:L369; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [documentation] https://github.com/strands-labs/strands-decider/blob/main/training/README.md (host:text:L376; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [documentation] https://github.com/strands-labs/strands-decider/blob/main/training/aws/README.md (host:text:L381; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [documentation] https://github.com/strands-labs/strands-decider/blob/main/data/README.md (host:text:L389; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [documentation] https://github.com/strands-labs/strands-decider/blob/main/research/README.md (host:text:L399; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [documentation] https://github.com/strands-labs/strands-decider/blob/main/research/history.md (host:text:L400; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [documentation] https://github.com/strands-labs/strands-decider/blob/main/CONTRIBUTING.md (host:text:L401; target retrieved: False)
- https://github.com/strands-labs/strands-decider → [documentation] https://github.com/strands-labs/strands-decider/blob/main/LICENSE (host:text:L409; target retrieved: False)
- https://github.com/strands-labs/strands-decider/blob/main/evaluation/results.md → [documentation] https://github.com/strands-labs/strands-decider/blob/main/evaluation/README.md (host:text:L5; target retrieved: False)
- https://github.com/strands-labs/strands-decider/blob/main/evaluation/results.md → [documentation] https://github.com/strands-labs/strands-decider/blob/main/evaluation/jevbench.md (host:text:L6; target retrieved: False)
- https://github.com/strands-labs/strands-decider/blob/main/evaluation/results.md → [documentation] https://github.com/strands-labs/strands-decider/blob/main/docs/naming.md (host:text:L11; target retrieved: False)
- https://github.com/strands-labs/strands-decider/blob/main/evaluation/results.md → [documentation] https://github.com/strands-labs/strands-decider/blob/main/docs/vision.md (host:text:L72; target retrieved: False)
- https://github.com/strands-labs/strands-decider/blob/main/evaluation/results.md → [documentation] https://github.com/strands-labs/strands-decider/blob/main/data/sources.md (host:text:L85; target retrieved: False)
- https://github.com/strands-labs/strands-decider/blob/main/evaluation/results.md → [documentation] https://github.com/strands-labs/strands-decider/blob/main/docs/inference.md (host:text:L192; target retrieved: False)
- https://github.com/strands-labs/strands-decider/blob/main/evaluation/results.md → [documentation] https://github.com/strands-labs/strands-decider/blob/main/configs/experiments/v21b.yaml (host:text:L197; target retrieved: False)
- https://github.com/strands-labs/strands-decider/blob/main/evaluation/results.md → [documentation] https://github.com/strands-labs/strands-decider/blob/main/training/aws/README.md (host:text:L253; target retrieved: False)
- https://github.com/strands-labs/strands-decider/blob/main/evaluation/results.md → [documentation] https://github.com/strands-labs/strands-decider/blob/main/evaluation/results.md (host:text:L287; target retrieved: True)
- https://github.com/strands-labs/strands-decider/blob/main/evaluation/results.md → [documentation] https://github.com/strands-labs/strands-decider/blob/main/research/history.md (host:text:L297; target retrieved: False)
- https://github.com/strands-labs/strands-decider/blob/main/evaluation/results.md → [documentation] https://github.com/strands-labs/strands-decider/blob/main/research/preregistrations/PREREGISTRATION-v20.md (host:text:L299; target retrieved: False)
- https://github.com/strands-labs/strands-decider/blob/main/evaluation/results.md → [references] https://benchmarkheaven.com/jev-models (host:text:L319; target retrieved: False)
- https://github.com/strands-labs/strands-decider/blob/main/evaluation/results.md → [documentation] https://github.com/strands-labs/strands-decider/blob/main/docs/architecture.md (host:text:L406; target retrieved: False)
- https://github.com/strands-labs/strands-decider/blob/main/evaluation/results.md → [documentation] https://github.com/strands-labs/strands-decider/blob/main/research/preregistrations/PREREGISTRATION-v19-calmix.md (host:text:L419; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://strandsagents.com/ (html:repository-readme/line 3, a[1]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [code] https://github.com/strands-agents/harness-sdk (html:repository-readme/line 12, a[2]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://github.com/strands-agents/harness-sdk/graphs/commit-activity (html:repository-readme/line 21, a[4]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://github.com/strands-agents/harness-sdk/issues (html:repository-readme/line 22, a[5]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://github.com/strands-agents/harness-sdk/pulls (html:repository-readme/line 23, a[6]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [documentation] https://github.com/strands-agents/harness-sdk/blob/main/LICENSE.APACHE (html:repository-readme/line 24, a[7]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://pypi.org/project/strands-harness/ (html:repository-readme/line 25, a[8]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://www.npmjs.com/package/@strands-agents/harness (html:repository-readme/line 26, a[9]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://www.npmjs.com/package/@strands-agents/cli (html:repository-readme/line 27, a[10]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://pypi.org/project/strands-agents/ (html:repository-readme/line 28, a[11]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://www.npmjs.com/package/@strands-agents/sdk (html:repository-readme/line 29, a[12]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [code] https://github.com/strands-agents/samples (html:repository-readme/line 33, a[14]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [documentation] https://github.com/strands-agents/harness-sdk/tree/main/strands-mcp (html:repository-readme/line 34, a[15]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://discord.gg/strands (html:repository-readme/line 35, a[16]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://strandsagents.com/docs/user-guide/concepts/agents/agent-loop/ (html:repository-readme/line 38, a[17]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://strandsagents.com/docs/user-guide/concepts/tools/ (html:repository-readme/line 38, a[18]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://strandsagents.com/docs/user-guide/concepts/agents/structured-output/ (html:repository-readme/line 38, a[19]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://strandsagents.com/docs/user-guide/concepts/tools/mcp-tools/ (html:repository-readme/line 38, a[20]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://strandsagents.com/docs/user-guide/concepts/multi-agent/multi-agent-patterns/ (html:repository-readme/line 38, a[21]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://strandsagents.com/docs/user-guide/concepts/memory/overview/ (html:repository-readme/line 38, a[22]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://strandsagents.com/docs/user-guide/concepts/agents/session-management/ (html:repository-readme/line 38, a[23]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://strandsagents.com/docs/user-guide/concepts/model-providers/ (html:repository-readme/line 38, a[24]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://strandsagents.com/docs/user-guide/concepts/streaming/ (html:repository-readme/line 38, a[25]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://strandsagents.com/docs/user-guide/safety-security/guardrails/ (html:repository-readme/line 38, a[26]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://strandsagents.com/docs/user-guide/observability-evaluation/observability/ (html:repository-readme/line 38, a[27]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://strandsagents.com/docs/user-guide/evals-sdk/quickstart/ (html:repository-readme/line 38, a[28]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [documentation] https://github.com/strands-agents/harness-sdk/blob/main/.agents/skills/strands (html:repository-readme/line 39, a[29]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [documentation] https://github.com/strands-agents/harness-sdk/blob/main/harness-py (html:repository-readme/line 50, a[30]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://strandsagents.com/docs/user-guide/harness/ (html:repository-readme/line 51, a[32]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [documentation] https://github.com/strands-agents/harness-sdk/blob/main/harness-ts (html:repository-readme/line 54, a[33]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [documentation] https://github.com/strands-agents/harness-sdk/blob/main/strands-cli (html:repository-readme/line 58, a[36]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [documentation] https://github.com/strands-agents/harness-sdk/blob/main/strands-py (html:repository-readme/line 62, a[38]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [release] https://github.com/strands-agents/harness-sdk/releases?q=python%2F&expanded=false (html:repository-readme/line 63, a[40]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [documentation] https://github.com/strands-agents/harness-sdk/blob/main/strands-ts (html:repository-readme/line 66, a[41]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [release] https://github.com/strands-agents/harness-sdk/releases?q=typescript%2F&expanded=false (html:repository-readme/line 67, a[43]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [documentation] https://github.com/strands-agents/harness-sdk/blob/main/strands-mcp (html:repository-readme/line 70, a[44]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://pypi.org/project/strands-agents-mcp-server/ (html:repository-readme/line 71, a[45]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [documentation] https://github.com/strands-agents/harness-sdk/blob/main/site (html:repository-readme/line 74, a[46]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [documentation] https://github.com/strands-agents/harness-sdk/blob/main/team (html:repository-readme/line 78, a[48]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [documentation] https://github.com/strands-agents/harness-sdk/blob/main/test-infra (html:repository-readme/line 82, a[49]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://strandsagents.com/docs/user-guide/harness/quickstart/ (html:repository-readme/line 97, a[54]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://strandsagents.com/docs/user-guide/harness/reference/configuration/ (html:repository-readme/line 116, a[59]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://strandsagents.com/docs/user-guide/quickstart/overview/ (html:repository-readme/line 117, a[60]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://strandsagents.com/docs/user-guide/sdk/bidi/ (html:repository-readme/line 153, a[73]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://strandsagents.com/docs/examples/ (html:repository-readme/line 154, a[74]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://strandsagents.com/docs/api/python/strands.agent.agent/ (html:repository-readme/line 155, a[75]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://strandsagents.com/docs/api/typescript/ (html:repository-readme/line 155, a[76]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://strandsagents.com/docs/user-guide/deploy/operating-agents-in-production/ (html:repository-readme/line 156, a[77]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [documentation] https://github.com/strands-agents/harness-sdk/blob/main/CONTRIBUTING.md (html:repository-readme/line 182, a[81]/@href; target retrieved: False)
- https://github.com/strands-agents/harness-sdk → [references] https://discord.com/invite/strands (html:repository-readme/line 191, a[83]/@href; target retrieved: False)

## Partial coverage

- https://github.com/strands-labs/strands-decider/blob/main/README.md: budget_exhausted (call budget exhausted)

## Next directions

建立自己的保留测试集，记录各置信度区间的正确率、拒答率和延迟，再与生成式路由比较；先核对当前发布版本和训练数据可重建程度。

- https://github.com/strands-labs/strands-decider/blob/main/evaluation/README.md: documentation
- https://github.com/strands-labs/strands-decider/blob/main/evaluation/jevbench.md: documentation
- https://github.com/strands-labs/strands-decider/blob/main/docs/naming.md: documentation
- https://github.com/strands-labs/strands-decider/blob/main/docs/vision.md: documentation
- https://github.com/strands-labs/strands-decider/blob/main/data/sources.md: documentation
- https://github.com/strands-labs/strands-decider/blob/main/docs/inference.md: documentation
- https://github.com/strands-labs/strands-decider/blob/main/configs/experiments/v21b.yaml: documentation
- https://github.com/strands-labs/strands-decider/blob/main/training/aws/README.md: documentation
- https://github.com/strands-labs/strands-decider/blob/main/research/history.md: documentation
- https://github.com/strands-labs/strands-decider/blob/main/research/preregistrations/PREREGISTRATION-v20.md: documentation
- https://benchmarkheaven.com/jev-models: references
- https://github.com/strands-labs/strands-decider/blob/main/docs/architecture.md: documentation
- https://github.com/strands-labs/strands-decider/blob/main/research/preregistrations/PREREGISTRATION-v19-calmix.md: documentation
- https://github.com/strands-labs/strands-decider/blob/main/README.md: budget_limit
- https://github.com/strands-labs/strands-decider/blob/main/README.md: budget_limit
- https://github.com/strands-labs/strands-decider/blob/main/docs/vision.md: budget_limit
- https://github.com/strands-agents/sdk-python: budget_limit
- https://github.com/strands-labs/strands-decider/blob/main/docs/naming.md: budget_limit
- https://github.com/strands-labs/strands-decider/graphs/commit-activity: budget_limit
- https://github.com/strands-labs/strands-decider/blob/main/data/sources.md: budget_limit
- https://github.com/strands-labs/strands-decider/blob/main/docs/inference.md: budget_limit
- https://github.com/strands-labs/strands-decider/blob/main/training/aws/README.md: budget_limit
- https://github.com/strands-labs/strands-decider/blob/main/CONTRIBUTING.md: budget_limit
- https://img.shields.io/github/issues-pr/strands-labs/strands-decider: budget_limit
- https://discord.gg/Wa4CQrxsP: budget_limit
- https://strandsagents.com/latest/assets/wordmark-github-dark.svg: budget_limit
- https://github.com/strands-labs/strands-decider/blob/main/docs/architecture.md: budget_limit
- https://github.com/strands-labs/strands-decider/blob/main/evaluation/README.md: budget_limit
- https://github.com/strands-labs/strands-decider/blob/main/examples/strands/README.md: budget_limit
- https://github.com/strands-labs/strands-decider/blob/main/data/README.md: budget_limit
- https://github.com/strands-labs/strands-decider/blob/main/research/README.md: budget_limit
- https://github.com/strands-labs/strands-decider/blob/main/LICENSE: budget_limit
- https://huggingface.co/amazon: budget_limit
- https://huggingface.co/StrandsAgents/strands-decider-E2B-gemma4-v1-2610: budget_limit
- https://huggingface.co/StrandsAgents/strands-decider-E4B-gemma4-v1-2610: budget_limit
- https://huggingface.co/StrandsAgents/strands-decider-12B-gemma4-v1-2610: budget_limit
- https://huggingface.co/StrandsAgents/strands-decider-26B-A4B-gemma4-v1-2610: budget_limit
- https://img.shields.io/badge/Discord-Join-5865F2?logo=discord&logoColor=white: budget_limit
- https://github.com/strands-labs/strands-decider/pulls: budget_limit
- https://huggingface.co/Qwen: budget_limit
- https://img.shields.io/github/commit-activity/m/strands-labs/strands-decider: budget_limit
- https://github.com/strands-labs/strands-decider/issues: budget_limit
- https://github.com/strands-labs/strands-decider/blob/main/evaluation/jevbench.md: budget_limit
- https://huggingface.co/StrandsAgents: budget_limit
- https://github.com/strands-labs/strands-decider/blob/main/training/README.md: budget_limit
- https://img.shields.io/github/issues/strands-labs/strands-decider: budget_limit
- https://strandsagents.com/: budget_limit
- https://strandsagents.com/latest/assets/wordmark-github-light.svg: budget_limit
- https://github.com/strands-labs/strands-decider/blob/main/research/history.md: budget_limit

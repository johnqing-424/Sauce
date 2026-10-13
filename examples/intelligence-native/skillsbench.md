# benchflow-ai/skillsbench

Generated: 2026-10-13T08:53:26.467467+00:00
Value proxy: 57.75/100 · Delivery tier: hold
Verification: primary_material_retrieved; experiments_not_independently_verified

## Discovery

文档和任务源确认：SkillsBench 将 Agent Skills 包用于实际产出任务，可选择 with-skill/no-skill 评测。已读到 offer-letter 的 task.md 和确定性 verifier，不能据此推定所有任务或模型效果。

## Three source roles

Origin status: primary_resource_verified
Earliest retrieved dated record: https://github.com/benchflow-ai/skillsbench (2025-12-29T05:04:57Z); global earliest is unknown.
Creator-direct records: https://github.com/benchflow-ai/skillsbench
Underlying resources: https://github.com/benchflow-ai/skillsbench

## Claims and facts

- [author_claim] SkillsBench
- [primary_document_confirmed] Primary repository retrieved: benchflow-ai/skillsbench

## Verifiable evidence

### repository: benchflow-ai

https://github.com/benchflow-ai/skillsbench
Published: 2025-12-29T05:04:57Z; version: unknown
Retrieved: 2026-10-13T03:42:45.045Z; location: text:chars:140-540; SHA256: 77686a4cc0d50370e9763c83dffaec8b3f46db18825e4b11814e13d1b9797500
Status: primary_document_retrieved; freshness: host_observed_snapshot

> # SkillsBench
>
> [![Discord](https://img.shields.io/badge/Discord-Join-7289da?logo=discord&logoColor=white)](https://discord.gg/G9dg3EfSva)
> [![GitHub](https://img.shields.io/github/stars/benchflow-ai/skillsbench?style=social)](https://github.com/benchflow-ai/skillsbench)
> [![WeChat](https://img.shields.io/badge/WeChat-Join-07C160?logo=wechat&logoColor=white)](docs/wechat-qr.jpg)
> [![Hugging Face Datas
Host-reported retrieval: mcp__codex_apps__github_fetch; HTTP status unknown; CLI transport/DNS/TLS not independently verified.
Host-reported retrieval: mcp__codex_apps__github_fetch_file; HTTP status unknown; CLI transport/DNS/TLS not independently verified.

### documentation: unknown

https://github.com/benchflow-ai/skillsbench/blob/main/CONTRIBUTING.md
Published: unknown; version: unknown
Retrieved: 2026-10-13T03:45:16.619Z; location: text:chars:0-400; SHA256: b9c44c4853135a82f5a59e4adbfd25571820fd906ca974ef6052efe15ca805a4
Status: document_retrieved; freshness: host_observed_snapshot

> # Contributing to SkillsBench
>
> SkillsBench evaluates how well AI agents use reusable skills to complete real
> tasks. We need contributors to add diverse, challenging, well-tested task
> packages.
>
> **Links**: [Website](https://www.skillsbench.ai) · [GitHub](https://github.com/benchflow-ai/skillsbench) · [BenchFlow CLI](https://github.com/benchflow-ai/benchflow) · [Discord](https://discord.gg/G9dg3EfSv
Host-reported retrieval: mcp__codex_apps__github_fetch_file; HTTP status unknown; CLI transport/DNS/TLS not independently verified.

### documentation: unknown

https://github.com/benchflow-ai/skillsbench/blob/main/README.md
Published: unknown; version: unknown
Retrieved: 2026-10-13T03:42:45.045Z; location: text:chars:0-400; SHA256: da52e1ecd8c992e9125ec46b6237bd14d4c4b6a5ca7be896e2a06c97be1d79eb
Status: document_retrieved; freshness: host_observed_snapshot

> # SkillsBench
>
> [![Discord](https://img.shields.io/badge/Discord-Join-7289da?logo=discord&logoColor=white)](https://discord.gg/G9dg3EfSva)
> [![GitHub](https://img.shields.io/github/stars/benchflow-ai/skillsbench?style=social)](https://github.com/benchflow-ai/skillsbench)
> [![WeChat](https://img.shields.io/badge/WeChat-Join-07C160?logo=wechat&logoColor=white)](docs/wechat-qr.jpg)
> [![Hugging Face Datas
Host-reported retrieval: mcp__codex_apps__github_fetch_file; HTTP status unknown; CLI transport/DNS/TLS not independently verified.

## Value and uncertainty

AI 推断：为企业技能或文档工作流建立回归评测时，测试结果和轨迹比 README 宣称更可操作；其贡献流程要求先跑 oracle，再比较是否加载技能，有助于定位技能增益。
AI 应用假设：优先采用无需外部凭据的 tasks，以容器化 offer-letter 任务验证 DOCX 占位符、嵌套表格和条件段落，再扩展至自己的工作流。Agent 运行仍可能需要模型 API 或本地模型。

- No independent replication or experimental fact verification was performed.
- Earliest public record is scoped to retrieved records; global priority is unknown.
- Novelty, originality and practical value are heuristic proxies, not proved breakthroughs.
- Agent assessment is an evidence-linked interpretation, not independent fact or experiment verification.
- 代码阅读限制：该实例大量断言采用输出文本包含检查，不足以证明版式或所有字段的正确位置；conditional 检查只覆盖当前输入的 Yes 分支。只读取1个任务，未跑 oracle/模型，也未核查全量87任务。

## Evidence-linked Agent assessment

AI interpretation; not independent verification.

### Application potential

AI 应用假设：优先采用无需外部凭据的 tasks，以容器化 offer-letter 任务验证 DOCX 占位符、嵌套表格和条件段落，再扩展至自己的工作流。Agent 运行仍可能需要模型 API 或本地模型。

https://github.com/benchflow-ai/skillsbench/blob/main/README.md
Location: text:chars:2897-2977; SHA256: da52e1ecd8c992e9125ec46b6237bd14d4c4b6a5ca7be896e2a06c97be1d79eb
> Default runnable tasks live under `tasks/` and run with no external
> credentials.

### Finding

文档和任务源确认：SkillsBench 将 Agent Skills 包用于实际产出任务，可选择 with-skill/no-skill 评测。已读到 offer-letter 的 task.md 和确定性 verifier，不能据此推定所有任务或模型效果。

https://github.com/benchflow-ai/skillsbench/blob/main/README.md
Location: text:chars:905-964; SHA256: da52e1ecd8c992e9125ec46b6237bd14d4c4b6a5ca7be896e2a06c97be1d79eb
> SkillsBench measures how effectively agents leverage skills

### Limitations

代码阅读限制：该实例大量断言采用输出文本包含检查，不足以证明版式或所有字段的正确位置；conditional 检查只覆盖当前输入的 Yes 分支。只读取1个任务，未跑 oracle/模型，也未核查全量87任务。

https://github.com/benchflow-ai/skillsbench/blob/main/tasks/offer-letter-generator/verifier/test_outputs.py
Location: text:chars:2974-3001; SHA256: 913b9a3ebe579aed9c8f876dededea4d6a957eca9fbd0d9e8f043719cfb8cf05
> assert expected in all_text

https://github.com/benchflow-ai/skillsbench/blob/main/tasks/offer-letter-generator/verifier/test_outputs.py
Location: text:chars:4089-4144; SHA256: 913b9a3ebe579aed9c8f876dededea4d6a957eca9fbd0d9e8f043719cfb8cf05
> # Content should be present (RELOCATION_PACKAGE is Yes)

### New

AI 比较判断：已读取 AgentBench 的多环境通用代理基准；SkillsBench 的具体差异是技能包注入和成对技能条件。贡献文档称当前为 1.2，但同页 CLI 注释仍提 1.1，版本口径需核实。全球首创未知，未声称最近30天新发布。

https://github.com/THUDM/AgentBench/blob/main/README.md
Location: text:chars:4718-4756; SHA256: 1b7d1f1cd7a74ac9497c639324ec342dd3f8769e9c0c4cd2cd92a4eb6740ac98
> It encompasses 8 distinct environments

https://github.com/benchflow-ai/skillsbench/blob/main/CONTRIBUTING.md
Location: text:chars:650-692; SHA256: b9c44c4853135a82f5a59e4adbfd25571820fd906ca974ef6052efe15ca805a4
> The current release is **SkillsBench 1.2**

### Next steps

下一步测试：固定同一模型、输入和沙箱，对 easy offer-letter 任务做多次 with-skill/no-skill，保存耗时与轨迹；增加 RELOCATION_PACKAGE=No 和错位字段输入，验证 verifier 是否能识别。

https://github.com/benchflow-ai/skillsbench/blob/main/tasks/offer-letter-generator/task.md
Location: text:chars:96-144; SHA256: a3ce086d3b605fcb45cfe553b31ce45071d95047ba839c6a67add358a40cb772
> difficulty: easy
>   category: office-white-collar

### Why it matters

AI 推断：为企业技能或文档工作流建立回归评测时，测试结果和轨迹比 README 宣称更可操作；其贡献流程要求先跑 oracle，再比较是否加载技能，有助于定位技能增益。

https://github.com/benchflow-ai/skillsbench/blob/main/CONTRIBUTING.md
Location: text:chars:1674-1720; SHA256: b9c44c4853135a82f5a59e4adbfd25571820fd906ca974ef6052efe15ca805a4
> Run at least one agent with and without skills

## Observed relationship chain

- https://github.com/benchflow-ai/skillsbench → [readme] https://github.com/benchflow-ai/skillsbench/blob/main/README.md (host:paired_snapshot_url; target retrieved: True)
- https://github.com/benchflow-ai/skillsbench → [references] https://img.shields.io/badge/Discord-Join-7289da?logo=discord&logoColor=white (host:text:L3; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench → [references] https://discord.gg/G9dg3EfSva (host:text:L3; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench → [references] https://img.shields.io/github/stars/benchflow-ai/skillsbench?style=social (host:text:L4; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench → [code] https://github.com/benchflow-ai/skillsbench (host:text:L4; target retrieved: True)
- https://github.com/benchflow-ai/skillsbench → [references] https://img.shields.io/badge/WeChat-Join-07C160?logo=wechat&logoColor=white (host:text:L5; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench → [references] https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Dataset-yellow (host:text:L6; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench → [references] https://huggingface.co/datasets/benchflow/skillsbench (host:text:L6; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench → [references] https://www.skillsbench.ai/ (host:text:L10; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench → [documentation] https://github.com/benchflow-ai/skillsbench/blob/main/CONTRIBUTING.md (host:text:L10; target retrieved: True)
- https://github.com/benchflow-ai/skillsbench → [code] https://github.com/benchflow-ai/benchflow (host:text:L10; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench → [code] https://github.com/benchflow-ai/skillsbench.git (host:text:L24; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench → [references] https://modal.com/ (host:text:L46; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench → [documentation] https://github.com/benchflow-ai/skillsbench/blob/main/tasks-extra/mhc-layer-impl (host:text:L53; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench → [documentation] https://github.com/benchflow-ai/skillsbench/blob/main/experiments/run_experiment.ipynb (host:text:L80; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench → [references] https://direnv.net/ (host:text:L86; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench → [documentation] https://github.com/benchflow-ai/skillsbench/blob/main/docs/wechat-qr.jpg (host:text:L111; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench → [documentation] https://github.com/benchflow-ai/skillsbench/blob/main/LICENSE (host:text:L116; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/CONTRIBUTING.md → [references] https://www.skillsbench.ai/ (host:text:L7; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/CONTRIBUTING.md → [code] https://github.com/benchflow-ai/skillsbench (host:text:L7; target retrieved: True)
- https://github.com/benchflow-ai/skillsbench/blob/main/CONTRIBUTING.md → [code] https://github.com/benchflow-ai/benchflow (host:text:L7; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/CONTRIBUTING.md → [references] https://discord.gg/G9dg3EfSva (host:text:L7; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/CONTRIBUTING.md → [code] https://github.com/benchflow-ai/skillsbench.git (host:text:L34; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/CONTRIBUTING.md → [documentation] https://github.com/benchflow-ai/skillsbench/blob/main/CONTRIBUTING.md (host:text:L68; target retrieved: True)
- https://github.com/benchflow-ai/skillsbench/blob/main/CONTRIBUTING.md → [documentation] https://github.com/benchflow-ai/skillsbench/blob/main/tasks/ (host:text:L70; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/CONTRIBUTING.md → [references] https://discord.com/channels/1348543112661962792/1473432026899157162 (host:text:L73; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/CONTRIBUTING.md → [references] https://github.com/benchflow-ai/skillsbench/discussions (host:text:L74; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/CONTRIBUTING.md → [documentation] https://github.com/benchflow-ai/skillsbench/blob/main/taxonomy.yaml (host:text:L152; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/CONTRIBUTING.md → [documentation] https://github.com/benchflow-ai/skillsbench/blob/main/taxonomy.md (host:text:L153; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/CONTRIBUTING.md → [documentation] https://github.com/benchflow-ai/skillsbench/blob/main/.github/scripts/lint_taxonomy.py (host:text:L156; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/CONTRIBUTING.md → [documentation] https://github.com/benchflow-ai/skillsbench/blob/main/.agents/skills/task-review/ (host:text:L283; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/README.md → [references] https://img.shields.io/badge/Discord-Join-7289da?logo=discord&logoColor=white (host:text:L3; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/README.md → [references] https://discord.gg/G9dg3EfSva (host:text:L3; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/README.md → [references] https://img.shields.io/github/stars/benchflow-ai/skillsbench?style=social (host:text:L4; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/README.md → [code] https://github.com/benchflow-ai/skillsbench (host:text:L4; target retrieved: True)
- https://github.com/benchflow-ai/skillsbench/blob/main/README.md → [references] https://img.shields.io/badge/WeChat-Join-07C160?logo=wechat&logoColor=white (host:text:L5; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/README.md → [references] https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Dataset-yellow (host:text:L6; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/README.md → [references] https://huggingface.co/datasets/benchflow/skillsbench (host:text:L6; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/README.md → [references] https://www.skillsbench.ai/ (host:text:L10; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/README.md → [documentation] https://github.com/benchflow-ai/skillsbench/blob/main/CONTRIBUTING.md (host:text:L10; target retrieved: True)
- https://github.com/benchflow-ai/skillsbench/blob/main/README.md → [code] https://github.com/benchflow-ai/benchflow (host:text:L10; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/README.md → [code] https://github.com/benchflow-ai/skillsbench.git (host:text:L24; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/README.md → [references] https://modal.com/ (host:text:L46; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/README.md → [documentation] https://github.com/benchflow-ai/skillsbench/blob/main/tasks-extra/mhc-layer-impl (host:text:L53; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/README.md → [documentation] https://github.com/benchflow-ai/skillsbench/blob/main/experiments/run_experiment.ipynb (host:text:L80; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/README.md → [references] https://direnv.net/ (host:text:L86; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/README.md → [documentation] https://github.com/benchflow-ai/skillsbench/blob/main/docs/wechat-qr.jpg (host:text:L111; target retrieved: False)
- https://github.com/benchflow-ai/skillsbench/blob/main/README.md → [documentation] https://github.com/benchflow-ai/skillsbench/blob/main/LICENSE (host:text:L116; target retrieved: False)

## Next directions

下一步测试：固定同一模型、输入和沙箱，对 easy offer-letter 任务做多次 with-skill/no-skill，保存耗时与轨迹；增加 RELOCATION_PACKAGE=No 和错位字段输入，验证 verifier 是否能识别。

- https://www.skillsbench.ai/: references
- https://github.com/benchflow-ai/benchflow: code
- https://discord.gg/G9dg3EfSva: references
- https://github.com/benchflow-ai/skillsbench.git: code
- https://github.com/benchflow-ai/skillsbench/blob/main/tasks/: documentation
- https://discord.com/channels/1348543112661962792/1473432026899157162: references
- https://github.com/benchflow-ai/skillsbench/discussions: references
- https://github.com/benchflow-ai/skillsbench/blob/main/taxonomy.yaml: documentation
- https://github.com/benchflow-ai/skillsbench/blob/main/taxonomy.md: documentation
- https://github.com/benchflow-ai/skillsbench/blob/main/.github/scripts/lint_taxonomy.py: documentation
- https://github.com/benchflow-ai/skillsbench/blob/main/.agents/skills/task-review/: documentation
- https://img.shields.io/badge/Discord-Join-7289da?logo=discord&logoColor=white: references
- https://discord.gg/G9dg3EfSva: references
- https://img.shields.io/github/stars/benchflow-ai/skillsbench?style=social: references
- https://img.shields.io/badge/WeChat-Join-07C160?logo=wechat&logoColor=white: references
- https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Dataset-yellow: references
- https://huggingface.co/datasets/benchflow/skillsbench: references
- https://www.skillsbench.ai/: references
- https://github.com/benchflow-ai/benchflow: code
- https://github.com/benchflow-ai/skillsbench.git: code
- https://modal.com/: references
- https://github.com/benchflow-ai/skillsbench/blob/main/tasks-extra/mhc-layer-impl: documentation
- https://github.com/benchflow-ai/skillsbench/blob/main/experiments/run_experiment.ipynb: documentation
- https://direnv.net/: references
- https://github.com/benchflow-ai/skillsbench/blob/main/docs/wechat-qr.jpg: documentation
- https://github.com/benchflow-ai/skillsbench/blob/main/LICENSE: documentation
- https://github.com/benchflow-ai/benchflow: host_material_required
- https://github.com/benchflow-ai/skillsbench/blob/main/tasks-extra/mhc-layer-impl: host_material_required
- https://github.com/benchflow-ai/skillsbench/blob/main/experiments/run_experiment.ipynb: host_material_required
- https://github.com/benchflow-ai/skillsbench/blob/main/docs/wechat-qr.jpg: host_material_required
- https://github.com/benchflow-ai/skillsbench/blob/main/LICENSE: host_material_required
- https://img.shields.io/badge/Discord-Join-7289da?logo=discord&logoColor=white: host_material_required
- https://discord.gg/G9dg3EfSva: host_material_required
- https://img.shields.io/github/stars/benchflow-ai/skillsbench?style=social: host_material_required
- https://img.shields.io/badge/WeChat-Join-07C160?logo=wechat&logoColor=white: host_material_required
- https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Dataset-yellow: host_material_required
- https://huggingface.co/datasets/benchflow/skillsbench: host_material_required
- https://www.skillsbench.ai/: host_material_required
- https://modal.com/: host_material_required
- https://direnv.net/: host_material_required

# xishi404/KVShare-Arena

Generated: 2026-10-13T08:53:26.716757+00:00
Value proxy: 60.75/100 · Delivery tier: B
Verification: primary_material_retrieved; experiments_not_independently_verified

## Discovery

文档确认：KVShareArena 是将跨上下文、跨模型检查点评测统一到问题、模型、质量和成本口径的可复用资源。论文 v2 与仓库均为 2026-09-27 的主机报告记录，落在窗口；未复现实验。

## Three source roles

Origin status: primary_resource_verified
Earliest retrieved dated record: https://github.com/xishi404/KVShare-Arena (2026-09-27T19:17:12Z); global earliest is unknown.
Creator-direct records: https://github.com/xishi404/KVShare-Arena
Underlying resources: https://github.com/xishi404/KVShare-Arena

## Claims and facts

- [author_claim] KVShareArena
- [primary_document_confirmed] Primary repository retrieved: xishi404/KVShare-Arena

## Verifiable evidence

### repository: xishi404

https://github.com/xishi404/KVShare-Arena
Published: 2026-09-27T19:17:12Z; version: unknown
Retrieved: 2026-10-13T03:44:40.954Z; location: text:chars:47-447; SHA256: 3983ddd84221321bd2dcfbcf19ef1b9498cba8f7010a894f5a6313456fc271a3
Status: primary_document_retrieved; freshness: host_observed_snapshot

> # KVShareArena
>
> A benchmark and open evaluation framework for KV-cache reuse when the preceding text or the LLM that
> wrote the cache changes.
>
> **[Leaderboard](https://xishi404.github.io/KVShare-Arena/)** ·
> **[Paper (arXiv:2609.10266)](https://arxiv.org/abs/2609.10266)** ·
> [Benchmark settings](docs/benchmark.md) · [Question sets](data/queryset/README.md) ·
> [Add a method](CONTRIBUTING.md)
>
> Reusing K
Host-reported retrieval: mcp__codex_apps__github_fetch; HTTP status unknown; CLI transport/DNS/TLS not independently verified.
Host-reported retrieval: mcp__codex_apps__github_fetch_file; HTTP status unknown; CLI transport/DNS/TLS not independently verified.

### paper: unknown

https://arxiv.org/abs/2609.10266
Published: unknown; version: unknown
Retrieved: 2026-10-13T03:42:45.222Z; location: text:chars:979-1379; SHA256: e347fb287a8a27ccad642495d84e7f06955c83745f281c0ddb4665dedb846993
Status: document_retrieved; freshness: host_observed_snapshot

> Reusing key-value (KV) caches speeds up LLM inference by avoiding repeated computation on shared text.
> L17: Standard prefix caching reuses a KV cache only when the LLM is the same and all preceding text is identical, but real workloads often break both conditions: RAG systems place different documents before the same one, agents with different system prompts read the same file or tool output, mult
Host-reported retrieval: mcp__codex_apps__search_service_web_run; HTTP status unknown; CLI transport/DNS/TLS not independently verified.

### documentation: unknown

https://github.com/xishi404/KVShare-Arena/blob/main/docs/benchmark.md
Published: unknown; version: unknown
Retrieved: 2026-10-13T03:45:16.506Z; location: text:chars:0-400; SHA256: 8fdce0e1d3ee201d0b84245b9aae30984d68a65b1a5264f5f0a2e3adb62106b0
Status: document_retrieved; freshness: host_observed_snapshot

> # Benchmark settings
>
> ## Two kinds of change
>
> **Context change (cross-context reuse).** Each source is cached separately and the caches are combined
> in a new prompt, so a cached block is reused after different preceding text. Position alignment moves a
> cache to its new positions without recomputing any token; it does not add the missing context.
>
> **Checkpoint change (cross-checkpoint reuse).** A c
Host-reported retrieval: mcp__codex_apps__github_fetch_file; HTTP status unknown; CLI transport/DNS/TLS not independently verified.

### documentation: unknown

https://github.com/xishi404/KVShare-Arena/blob/main/data/queryset/README.md
Published: unknown; version: unknown
Retrieved: 2026-10-13T03:45:16.505Z; location: text:chars:0-400; SHA256: acc79489dea4713493af2c8260a4e9394eca27e1ee00f9d910513083f3842b27
Status: document_retrieved; freshness: host_observed_snapshot

> # Frozen evaluation inputs
>
> | File | Contents |
> | --- | --- |
> | `qasper_n1000.jsonl.gz` | 1,000 Qasper questions (scientific-paper QA) |
> | `multifieldqa_en_n150.jsonl.gz` | 150 MultiFieldQA-en questions (single-document QA) |
> | `hotpotqa_n1000.jsonl.gz` | 1,000 HotpotQA questions (multi-hop QA) |
> | `agent_reports/` | Frozen question-blind reports for the first 100 HotpotQA questions, with token id
Host-reported retrieval: mcp__codex_apps__github_fetch_file; HTTP status unknown; CLI transport/DNS/TLS not independently verified.

### documentation: unknown

https://github.com/xishi404/KVShare-Arena/blob/main/README.md
Published: unknown; version: unknown
Retrieved: 2026-10-13T03:44:40.955Z; location: text:chars:0-400; SHA256: abff189f782b93838cc2c2a2ff3c442468fc2794a34c03a1b2e91ceb75b513b7
Status: document_retrieved; freshness: host_observed_snapshot

> # KVShareArena
>
> A benchmark and open evaluation framework for KV-cache reuse when the preceding text or the LLM that
> wrote the cache changes.
>
> **[Leaderboard](https://xishi404.github.io/KVShare-Arena/)** ·
> **[Paper (arXiv:2609.10266)](https://arxiv.org/abs/2609.10266)** ·
> [Benchmark settings](docs/benchmark.md) · [Question sets](data/queryset/README.md) ·
> [Add a method](CONTRIBUTING.md)
>
> Reusing K
Host-reported retrieval: mcp__codex_apps__github_fetch_file; HTTP status unknown; CLI transport/DNS/TLS not independently verified.

## Value and uncertainty

AI 推断：真实 RAG/多代理常打破完全相同前缀，若只看命中率或 TTFT 会遗漏答案退化。该资源提供 F1/PGR 与成本定义，适合判断缓存优化是否可接受。
AI 应用假设：团队可先在 CPU 校验冻结题集并为自有输出评分，再接入自己的缓存方法，而不用先下载全部 GPU 模型。数据有独立上游许可，代码 Apache-2.0 不能替代数据条款。

- No independent replication or experimental fact verification was performed.
- Earliest public record is scoped to retrieved records; global priority is unknown.
- Novelty, originality and practical value are heuristic proxies, not proved breakthroughs.
- Agent assessment is an evidence-linked interpretation, not independent fact or experiment verification.
- 文档确认：已发表方法的专属实现和逐题输出不在包内，主要提供 position-alignment 示例；生成仍需 CUDA、模型和依赖。作者报告不是复现证明，排行榜结果无法全部独立重跑。

## Evidence-linked Agent assessment

AI interpretation; not independent verification.

### Application potential

AI 应用假设：团队可先在 CPU 校验冻结题集并为自有输出评分，再接入自己的缓存方法，而不用先下载全部 GPU 模型。数据有独立上游许可，代码 Apache-2.0 不能替代数据条款。

https://github.com/xishi404/KVShare-Arena/blob/main/README.md
Location: text:chars:2311-2371; SHA256: abff189f782b93838cc2c2a2ff3c442468fc2794a34c03a1b2e91ceb75b513b7
> These commands need no installation, GPU, or network access:

https://github.com/xishi404/KVShare-Arena/blob/main/data/queryset/README.md
Location: text:chars:2704-2754; SHA256: acc79489dea4713493af2c8260a4e9394eca27e1ee00f9d910513083f3842b27
> the
> Apache-2.0 code license does not replace them.

### Finding

文档确认：KVShareArena 是将跨上下文、跨模型检查点评测统一到问题、模型、质量和成本口径的可复用资源。论文 v2 与仓库均为 2026-09-27 的主机报告记录，落在窗口；未复现实验。

https://github.com/xishi404/KVShare-Arena/blob/main/README.md
Location: text:chars:16-76; SHA256: abff189f782b93838cc2c2a2ff3c442468fc2794a34c03a1b2e91ceb75b513b7
> A benchmark and open evaluation framework for KV-cache reuse

### Limitations

文档确认：已发表方法的专属实现和逐题输出不在包内，主要提供 position-alignment 示例；生成仍需 CUDA、模型和依赖。作者报告不是复现证明，排行榜结果无法全部独立重跑。

https://github.com/xishi404/KVShare-Arena/blob/main/docs/benchmark.md
Location: text:chars:2886-2980; SHA256: 8fdce0e1d3ee201d0b84245b9aae30984d68a65b1a5264f5f0a2e3adb62106b0
> Method-specific code for the evaluated methods and their
> per-question outputs are not included

### New

AI 比较判断：相对已读取的 LMCache 缓存管理能力，增量在横向质量/成本评测，而非首次实现非前缀复用。跨版本权重和上下文变化均被明确区分；全球科学首创未知。

https://github.com/xishi404/KVShare-Arena/blob/main/docs/benchmark.md
Location: text:chars:449-487; SHA256: 8fdce0e1d3ee201d0b84245b9aae30984d68a65b1a5264f5f0a2e3adb62106b0
> another version with different weights

https://github.com/LMCache/LMCache/blob/dev/README.md
Location: text:chars:6801-6838; SHA256: 60b8409940e9fd6abf7ed04ac984cad5200b1b5fb428f138684038091c0f4dae
> Extend KV reuse beyond prefix caching

### Next steps

下一步测试：先校验输入校验和和 100 题示例，再在同一后端加入自有方法，与 position alignment 做成对 bootstrap，分别记录缓存构建一次性成本与每请求 TTFT。跨零区间只表示未检测到差异。

https://github.com/xishi404/KVShare-Arena/blob/main/docs/benchmark.md
Location: text:chars:2615-2680; SHA256: 8fdce0e1d3ee201d0b84245b9aae30984d68a65b1a5264f5f0a2e3adb62106b0
> An interval containing zero means that no difference was detected

### Why it matters

AI 推断：真实 RAG/多代理常打破完全相同前缀，若只看命中率或 TTFT 会遗漏答案退化。该资源提供 F1/PGR 与成本定义，适合判断缓存优化是否可接受。

https://github.com/xishi404/KVShare-Arena/blob/main/docs/benchmark.md
Location: text:chars:1252-1314; SHA256: 8fdce0e1d3ee201d0b84245b9aae30984d68a65b1a5264f5f0a2e3adb62106b0
> Answers are scored with the official LongBench token-level F1.

## Observed relationship chain

- https://github.com/xishi404/KVShare-Arena → [readme] https://github.com/xishi404/KVShare-Arena/blob/main/README.md (host:paired_snapshot_url; target retrieved: True)
- https://github.com/xishi404/KVShare-Arena → [references] https://xishi404.github.io/KVShare-Arena/ (host:text:L6; target retrieved: False)
- https://github.com/xishi404/KVShare-Arena → [paper] https://arxiv.org/abs/2609.10266 (host:text:L7; target retrieved: True)
- https://github.com/xishi404/KVShare-Arena → [documentation] https://github.com/xishi404/KVShare-Arena/blob/main/docs/benchmark.md (host:text:L8; target retrieved: True)
- https://github.com/xishi404/KVShare-Arena → [documentation] https://github.com/xishi404/KVShare-Arena/blob/main/data/queryset/README.md (host:text:L8; target retrieved: True)
- https://github.com/xishi404/KVShare-Arena → [documentation] https://github.com/xishi404/KVShare-Arena/blob/main/CONTRIBUTING.md (host:text:L9; target retrieved: False)
- https://github.com/xishi404/KVShare-Arena/blob/main/data/queryset/README.md → [code] https://github.com/THUDM/LongBench (host:text:L48; target retrieved: False)
- https://github.com/xishi404/KVShare-Arena/blob/main/data/queryset/README.md → [references] https://allenai.org/data/qasper (host:text:L51; target retrieved: False)
- https://github.com/xishi404/KVShare-Arena/blob/main/data/queryset/README.md → [references] https://hotpotqa.github.io/ (host:text:L53; target retrieved: False)
- https://github.com/xishi404/KVShare-Arena/blob/main/README.md → [references] https://xishi404.github.io/KVShare-Arena/ (host:text:L6; target retrieved: False)
- https://github.com/xishi404/KVShare-Arena/blob/main/README.md → [paper] https://arxiv.org/abs/2609.10266 (host:text:L7; target retrieved: True)
- https://github.com/xishi404/KVShare-Arena/blob/main/README.md → [documentation] https://github.com/xishi404/KVShare-Arena/blob/main/docs/benchmark.md (host:text:L8; target retrieved: True)
- https://github.com/xishi404/KVShare-Arena/blob/main/README.md → [documentation] https://github.com/xishi404/KVShare-Arena/blob/main/data/queryset/README.md (host:text:L8; target retrieved: True)
- https://github.com/xishi404/KVShare-Arena/blob/main/README.md → [documentation] https://github.com/xishi404/KVShare-Arena/blob/main/CONTRIBUTING.md (host:text:L9; target retrieved: False)

## Next directions

下一步测试：先校验输入校验和和 100 题示例，再在同一后端加入自有方法，与 position alignment 做成对 bootstrap，分别记录缓存构建一次性成本与每请求 TTFT。跨零区间只表示未检测到差异。

- https://github.com/THUDM/LongBench: code
- https://allenai.org/data/qasper: references
- https://hotpotqa.github.io/: references
- https://xishi404.github.io/KVShare-Arena/: references
- https://github.com/xishi404/KVShare-Arena/blob/main/CONTRIBUTING.md: documentation
- https://github.com/xishi404/KVShare-Arena/blob/main/CONTRIBUTING.md: host_material_required
- https://xishi404.github.io/KVShare-Arena/: host_material_required

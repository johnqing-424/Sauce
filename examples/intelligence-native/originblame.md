# tzbkk/originblame

Generated: 2026-10-13T08:53:26.580354+00:00
Value proxy: 57.75/100 · Delivery tier: hold
Verification: primary_material_retrieved; experiments_not_independently_verified

## Discovery

文档确认：OriginBlame 记录训练数据的作者、来源、记录和 token 关联，并生成撤销/遗忘集合。它要求采集阶段记录来源。最后相关论文修订与仓库推送均在8月，此处是有用旧资源，不能作为最近30天的新突破。

## Three source roles

Origin status: primary_resource_verified
Earliest retrieved dated record: https://github.com/tzbkk/originblame (2026-04-01T16:43:01Z); global earliest is unknown.
Creator-direct records: https://github.com/tzbkk/originblame
Underlying resources: https://github.com/tzbkk/originblame

## Claims and facts

- [author_claim] OriginBlame
- [primary_document_confirmed] Primary repository retrieved: tzbkk/originblame

## Verifiable evidence

### repository: tzbkk

https://github.com/tzbkk/originblame
Published: 2026-04-01T16:43:01Z; version: unknown
Retrieved: 2026-10-13T03:42:45.125Z; location: text:chars:104-504; SHA256: a9646d7c348fae3c5f6bd59959939f153dddb4139292111f1dabca0d4a476965
Status: primary_document_retrieved; freshness: host_observed_snapshot

> # OriginBlame
>
> **Record- and token-level data provenance for AI training datasets.**
>
> When a data contributor requests removal, model trainers face a practical gap: unlearning algorithms require a forget set, yet no tool can locate which training records belong to a given author. Existing provenance systems operate at file or dataset level, forcing catastrophic over-deletion. We present `ob`, a re
Host-reported retrieval: mcp__codex_apps__github_fetch; HTTP status unknown; CLI transport/DNS/TLS not independently verified.
Host-reported retrieval: mcp__codex_apps__github_fetch_file; HTTP status unknown; CLI transport/DNS/TLS not independently verified.

### paper: unknown

https://arxiv.org/abs/2607.13037
Published: unknown; version: unknown
Retrieved: 2026-10-13T03:43:45.675Z; location: text:chars:966-1366; SHA256: bb4f68ff6f2f9f80e4b7f0e746b610f8dbe9be37134b81e1e7e0194234531545
Status: document_retrieved; freshness: host_observed_snapshot

> When a data contributor requests removal, model trainers face a practical gap: unlearning algorithms require a forget set, yet no tool can locate which training records belong to a given author. Existing provenance systems operate at file or dataset level, forcing catastrophic over-deletion.
> L17: We present ob, a record- and token-level data provenance system that propagates author identity throug
Host-reported retrieval: mcp__codex_apps__search_service_web_run; HTTP status unknown; CLI transport/DNS/TLS not independently verified.

### documentation: unknown

https://github.com/tzbkk/originblame/blob/master/README.md
Published: unknown; version: unknown
Retrieved: 2026-10-13T03:42:45.204Z; location: text:chars:0-400; SHA256: a7095083cc705c45da0c276c7e5143e11ef3cf6eb15c34285fbfbbdc386026b5
Status: document_retrieved; freshness: host_observed_snapshot

> # OriginBlame
>
> **Record- and token-level data provenance for AI training datasets.**
>
> When a data contributor requests removal, model trainers face a practical gap: unlearning algorithms require a forget set, yet no tool can locate which training records belong to a given author. Existing provenance systems operate at file or dataset level, forcing catastrophic over-deletion. We present `ob`, a re
Host-reported retrieval: mcp__codex_apps__github_fetch_file; HTTP status unknown; CLI transport/DNS/TLS not independently verified.

## Value and uncertainty

AI 推断：撤回某个贡献者的数据需要可精确定位的 forget set；这可减少整文件/整数据集删除的旁损。作者论文给出实验规模与吞吐代价，但本轮未复现这些数字。
AI 应用假设：新建数据管线可在采集与 tokenization 时持续登记来源，导出 bitmask 供下游删除/遗忘算法使用；已有无来源数据无法靠该记录机制自动回溯真实作者。

- No independent replication or experimental fact verification was performed.
- Earliest public record is scoped to retrieved records; global priority is unknown.
- Novelty, originality and practical value are heuristic proxies, not proved breakthroughs.
- Agent assessment is an evidence-linked interpretation, not independent fact or experiment verification.
- 文档确认：作者声明 seed42 单次实验，遗忘后仍有较高 extraction，retain-PPL 优势未在 retain ROUGE-L 复现；来源定位不能保证模型擦除。按文档路径读取 pipeline_v2/summary.json 返回404，原始汇总未核验。

## Evidence-linked Agent assessment

AI interpretation; not independent verification.

### Application potential

AI 应用假设：新建数据管线可在采集与 tokenization 时持续登记来源，导出 bitmask 供下游删除/遗忘算法使用；已有无来源数据无法靠该记录机制自动回溯真实作者。

https://github.com/tzbkk/rust-originblame/blob/master/README.md
Location: text:chars:6491-6537; SHA256: 12c937f8f343150c5b5eb2ae305a4368feaed92607fca5ae7075357e54f87fd4
> ob generate-set --tokenizer gpt2 -o forget.bin

https://github.com/tzbkk/originblame/blob/master/README.md
Location: text:chars:1344-1401; SHA256: a7095083cc705c45da0c276c7e5143e11ef3cf6eb15c34285fbfbbdc386026b5
> OriginBlame tracks provenance at **data collection time**

### Finding

文档确认：OriginBlame 记录训练数据的作者、来源、记录和 token 关联，并生成撤销/遗忘集合。它要求采集阶段记录来源。最后相关论文修订与仓库推送均在8月，此处是有用旧资源，不能作为最近30天的新突破。

https://github.com/tzbkk/originblame/blob/master/README.md
Location: text:chars:15-84; SHA256: a7095083cc705c45da0c276c7e5143e11ef3cf6eb15c34285fbfbbdc386026b5
> **Record- and token-level data provenance for AI training datasets.**

### Limitations

文档确认：作者声明 seed42 单次实验，遗忘后仍有较高 extraction，retain-PPL 优势未在 retain ROUGE-L 复现；来源定位不能保证模型擦除。按文档路径读取 pipeline_v2/summary.json 返回404，原始汇总未核验。

https://github.com/tzbkk/originblame/blob/master/README.md
Location: text:chars:12305-12334; SHA256: a7095083cc705c45da0c276c7e5143e11ef3cf6eb15c34285fbfbbdc386026b5
> Single-run results (seed 42);

https://github.com/tzbkk/originblame/blob/master/benchmarks/README.md
Location: text:chars:17026-17093; SHA256: 61bd6e15d4a7bd98a7a8ffd69597ff384bbc416827adade9f108631dea265397
> pointing at the source is necessary but not sufficient for erasure.

### New

AI 判断：主要能力是 token/record 级确定性定位，而非自动证明或完成模型遗忘。读到了独立 Rust 实现的安装/API说明与双向项目链接；未读到可独立核验的全部先行系统，科学创新程度未知。

https://github.com/tzbkk/rust-originblame/blob/master/README.md
Location: text:chars:6543-6604; SHA256: 12c937f8f343150c5b5eb2ae305a4368feaed92607fca5ae7075357e54f87fd4
> The token-index operates independently of the document-index.

### Next steps

下一步测试：先用自有1000条可追踪样本跑 hash-only 流程，核验撤销精度、吞吐与错误归因；编辑部分记录后测 reconcile 恢复率。多seed遗忘和直接抽取评测留给后续 GPU 阶段。

https://github.com/tzbkk/originblame/blob/master/benchmarks/README.md
Location: text:chars:3410-3464; SHA256: 61bd6e15d4a7bd98a7a8ffd69597ff384bbc416827adade9f108631dea265397
> **Hash-only** (fast): Uses exact SHA-256 hash matching

### Why it matters

AI 推断：撤回某个贡献者的数据需要可精确定位的 forget set；这可减少整文件/整数据集删除的旁损。作者论文给出实验规模与吞吐代价，但本轮未复现这些数字。

https://arxiv.org/abs/2607.13037
Location: text:chars:1398-1478; SHA256: bb4f68ff6f2f9f80e4b7f0e746b610f8dbe9be37134b81e1e7e0194234531545
> resolves revocation requests into precise forget sets via deterministic queries.

## Observed relationship chain

- https://github.com/tzbkk/originblame → [readme] https://github.com/tzbkk/originblame/blob/master/README.md (host:paired_snapshot_url; target retrieved: True)
- https://github.com/tzbkk/originblame → [code] https://github.com/tzbkk/rust-originblame (host:text:L9; target retrieved: False)
- https://github.com/tzbkk/originblame → [paper] https://arxiv.org/abs/2607.13037 (host:text:L57; target retrieved: True)
- https://github.com/tzbkk/originblame → [references] https://dumps.wikimedia.org/zhwiki/20260401/ (host:text:L66; target retrieved: False)
- https://github.com/tzbkk/originblame → [references] https://mirrors.ustc.edu.cn/linux.git (host:text:L68; target retrieved: False)
- https://github.com/tzbkk/originblame/blob/master/README.md → [code] https://github.com/tzbkk/rust-originblame (host:text:L9; target retrieved: False)
- https://github.com/tzbkk/originblame/blob/master/README.md → [paper] https://arxiv.org/abs/2607.13037 (host:text:L57; target retrieved: True)
- https://github.com/tzbkk/originblame/blob/master/README.md → [references] https://dumps.wikimedia.org/zhwiki/20260401/ (host:text:L66; target retrieved: False)
- https://github.com/tzbkk/originblame/blob/master/README.md → [references] https://mirrors.ustc.edu.cn/linux.git (host:text:L68; target retrieved: False)

## Next directions

下一步测试：先用自有1000条可追踪样本跑 hash-only 流程，核验撤销精度、吞吐与错误归因；编辑部分记录后测 reconcile 恢复率。多seed遗忘和直接抽取评测留给后续 GPU 阶段。

- https://github.com/tzbkk/rust-originblame: code
- https://dumps.wikimedia.org/zhwiki/20260401/: references
- https://mirrors.ustc.edu.cn/linux.git: references
- https://github.com/tzbkk/rust-originblame: host_material_required
- https://dumps.wikimedia.org/zhwiki/20260401/: host_material_required
- https://mirrors.ustc.edu.cn/linux.git: host_material_required

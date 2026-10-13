# mizorewww/laya-mlx

Generated: 2026-10-13T01:15:07.158136+00:00
Value proxy: 60.75/100 · Delivery tier: B
Verification: primary_material_retrieved; experiments_not_independently_verified

## Discovery

Laya-MLX 把用于选择和评分的 Laya 决策模型移植到 Apple Silicon 本地运行。它值得作为 Agent 路由实验候选，不应当作新的基础模型突破。

## Three source roles

Origin status: primary_resource_verified
Earliest retrieved dated record: https://github.com/mizorewww/laya-mlx (2026-09-19T13:50:26Z); global earliest is unknown.
Creator-direct records: https://github.com/mizorewww/laya-mlx
Underlying resources: https://github.com/mizorewww/laya-mlx

## Claims and facts

- [unverified] Original observation has no claim text.
- [primary_document_confirmed] Primary repository retrieved: mizorewww/laya-mlx

## Verifiable evidence

### repository: mizorewww

https://github.com/mizorewww/laya-mlx
Published: 2026-09-19T13:50:26Z; version: unknown
Retrieved: 2026-10-12T08:22:32+00:00; location: text:chars:174-574; SHA256: a9c91b1e932847e15468af3f8b36a989519d58b050a07a50c60e45783b5ed679
Status: primary_document_retrieved; freshness: host_observed_snapshot

> # Laya-MLX
>
> ![Laya MLX playing Snake — actual decisions, original speed](https://raw.githubusercontent.com/mizorewww/laya-mlx/main/docs/assets/snake-demo.gif)
>
> **Open-weight typed decisions, running natively on Apple Silicon.**
>
> **13.4 ms** median end-to-end for a short English typed decision. **7.4 ms** with the multilingual checkpoint. **0 output tokens.** Local MLX inference, with no PyTorch, T
Host-reported retrieval: github.fetch (authorized MCP); HTTP status unknown; CLI transport/DNS/TLS not independently verified.
Host-reported retrieval: github.fetch (authorized MCP); HTTP status unknown; CLI transport/DNS/TLS not independently verified.

### documentation: unknown

https://github.com/mizorewww/laya-mlx/blob/main/BENCHMARKS.md
Published: unknown; version: unknown
Retrieved: 2026-10-12T08:22:32+00:00; location: text:chars:0-400; SHA256: af468244a62d940abe822afe6a9ddb824fe0207ea65df426c829e372aebfee05
Status: document_retrieved; freshness: host_observed_snapshot

> # Local benchmarks
>
> Measured on **Apple M3 Max**, 40-core GPU, **128 GiB unified memory**, macOS-27.2-arm64-64bit, Python 3.12.13.
>
> These are local measurements of the native MLX port and the pinned upstream PyTorch runtime on the same Mac. They are not comparisons with the upstream T4 or third-party API figures.
>
> ## Method
>
> - Each checkpoint/backend runs in a fresh process, sequentially, with 5 w
Host-reported retrieval: github.fetch (authorized MCP); HTTP status unknown; CLI transport/DNS/TLS not independently verified.

### repository: NandhaKishorM

https://github.com/NandhaKishorM/laya
Published: unknown; version: unknown
Retrieved: 2026-10-13T01:04:41.498509+00:00; location: text:chars:0-400; SHA256: 10d54e7442a9c651cafa8938f9c6bd9bd04fefd265339b7e141e5846d9c1dc88
Status: document_retrieved; freshness: historical_not_revalidated

> Multilingual, non-autoregressive System 1 decision engine. Typed decisions over 100+ languages in a single forward pass — 33 ms — trained with reinforcement learning against strictly proper scoring rules (RLCD), with a router that picks the right checkpoint per request.
> Installation
> python -m pip install laya
> With uv, run uv add laya in a uv project or uv pip install laya in a virtual environment.

## Value and uncertainty

受控选项的分类或评分可能用本地决策模型替代部分生成式调用，减少网络依赖；这是假设，不能把单机测量推成普遍性能优势。
可在 Apple Silicon 上试验工具选择、分类和评分。你的 Windows 电脑不能直接照用这个 MLX 运行环境，需要另一个后端或相应硬件。

- No independent replication or experimental fact verification was performed.
- Earliest public record is scoped to retrieved records; global priority is unknown.
- Novelty, originality and practical value are heuristic proxies, not proved breakthroughs.
- Some linked resources could not be retrieved; the evidence chain is partial.
- Agent assessment is an evidence-linked interpretation, not independent fact or experiment verification.
- 性能数字来自作者的一台开发机，未独立复现；不能跨设备推广，也不能证明生产稳定性。当前追踪仍有失败或未探索的上游链接。

## Evidence-linked Agent assessment

AI interpretation; not independent verification.

### Application potential

可在 Apple Silicon 上试验工具选择、分类和评分。你的 Windows 电脑不能直接照用这个 MLX 运行环境，需要另一个后端或相应硬件。

https://github.com/mizorewww/laya-mlx
Location: text:chars:1831-1870; SHA256: a9c91b1e932847e15468af3f8b36a989519d58b050a07a50c60e45783b5ed679
> Apple Silicon, Python 3.11+, macOS 14+.

### Finding

Laya-MLX 把用于选择和评分的 Laya 决策模型移植到 Apple Silicon 本地运行。它值得作为 Agent 路由实验候选，不应当作新的基础模型突破。

https://github.com/mizorewww/laya-mlx
Location: text:chars:5823-5935; SHA256: a9c91b1e932847e15468af3f8b36a989519d58b050a07a50c60e45783b5ed679
> This repository provides inference and conversion; RLCD training and fine-tuning remain in the upstream project.

### Limitations

性能数字来自作者的一台开发机，未独立复现；不能跨设备推广，也不能证明生产稳定性。当前追踪仍有失败或未探索的上游链接。

https://github.com/mizorewww/laya-mlx/blob/main/BENCHMARKS.md
Location: text:chars:1885-2046; SHA256: af468244a62d940abe822afe6a9ddb824fe0207ea65df426c829e372aebfee05
> This is one development machine and one run of each configuration, with normal OS activity. No claim of cross-device performance or production endurance is made.

### New

这里新增的是 MLX 推理与权重转换实现；原模型训练方法仍来自上游，作者也明确说明这是独立移植。与此前工具的系统比较尚未完成。

https://github.com/mizorewww/laya-mlx
Location: text:chars:5936-6006; SHA256: a9c91b1e932847e15468af3f8b36a989519d58b050a07a50c60e45783b5ed679
> It is an independent port, not an official Convai Innovations release.

### Next steps

有合适 Mac 时，按原文条件比较 MLX 与上游 PyTorch 的同任务正确率及延迟，并单列冷启动、批处理和内存；Windows 上先调查可用的 CPU 决策模型实现。

https://github.com/mizorewww/laya-mlx/blob/main/BENCHMARKS.md
Location: text:chars:241-314; SHA256: af468244a62d940abe822afe6a9ddb824fe0207ea65df426c829e372aebfee05
> They are not comparisons with the upstream T4 or third-party API figures.

https://github.com/mizorewww/laya-mlx
Location: text:chars:1831-1870; SHA256: a9c91b1e932847e15468af3f8b36a989519d58b050a07a50c60e45783b5ed679
> Apple Silicon, Python 3.11+, macOS 14+.

### Why it matters

受控选项的分类或评分可能用本地决策模型替代部分生成式调用，减少网络依赖；这是假设，不能把单机测量推成普遍性能优势。

https://github.com/mizorewww/laya-mlx
Location: text:chars:1871-1939; SHA256: a9c91b1e932847e15468af3f8b36a989519d58b050a07a50c60e45783b5ed679
> First load downloads the checkpoint; later inference is fully local.

https://github.com/mizorewww/laya-mlx/blob/main/BENCHMARKS.md
Location: text:chars:241-314; SHA256: af468244a62d940abe822afe6a9ddb824fe0207ea65df426c829e372aebfee05
> They are not comparisons with the upstream T4 or third-party API figures.

## Observed relationship chain

- https://github.com/mizorewww/laya-mlx → [readme] https://github.com/mizorewww/laya-mlx/blob/main/README.md (host:paired_snapshot_url; target retrieved: False)
- https://github.com/mizorewww/laya-mlx → [references] https://raw.githubusercontent.com/mizorewww/laya-mlx/main/docs/assets/snake-demo.gif (host:text:L3; target retrieved: False)
- https://github.com/mizorewww/laya-mlx → [documentation] https://github.com/mizorewww/laya-mlx/blob/main/README.zh-CN.md (host:text:L9; target retrieved: False)
- https://github.com/mizorewww/laya-mlx → [documentation] https://github.com/mizorewww/laya-mlx/blob/main/BENCHMARKS.md (host:text:L9; target retrieved: True)
- https://github.com/mizorewww/laya-mlx → [documentation] https://github.com/mizorewww/laya-mlx/blob/main/docs/SNAKE_DEMO.md (host:text:L9; target retrieved: False)
- https://github.com/mizorewww/laya-mlx → [references] https://huggingface.co/aac6fef/laya-mlx (host:text:L9; target retrieved: False)
- https://github.com/mizorewww/laya-mlx → [documentation] https://github.com/mizorewww/laya-mlx/blob/main/docs/assets/snake-demo.mp4 (host:text:L11; target retrieved: False)
- https://github.com/mizorewww/laya-mlx → [documentation] https://github.com/mizorewww/laya-mlx/blob/main/docs/SNAKE_BENCHMARKS.md (host:text:L11; target retrieved: False)
- https://github.com/mizorewww/laya-mlx → [documentation] https://github.com/mizorewww/laya-mlx/blob/main/docs/SNAKE_OPTIMIZATION.md (host:text:L48; target retrieved: False)
- https://github.com/mizorewww/laya-mlx → [references] https://huggingface.co/aac6fef/laya-multilingual-mlx (host:text:L92; target retrieved: False)
- https://github.com/mizorewww/laya-mlx → [references] https://huggingface.co/aac6fef/laya-typed-decisions-mlx (host:text:L93; target retrieved: False)
- https://github.com/mizorewww/laya-mlx → [documentation] https://github.com/mizorewww/laya-mlx/blob/main/benchmarks/results/hub-publication.json (host:text:L95; target retrieved: False)
- https://github.com/mizorewww/laya-mlx → [code] https://github.com/mizorewww/laya-mlx.git (host:text:L106; target retrieved: False)
- https://github.com/mizorewww/laya-mlx → [references] https://github.com/NandhaKishorM/laya/commit/1adc59f7e371deb601fcfa18a14e25db238addcc (host:text:L212; target retrieved: False)
- https://github.com/mizorewww/laya-mlx → [documentation] https://github.com/mizorewww/laya-mlx/blob/main/benchmarks/results/upstream-v041-validation.json (host:text:L298; target retrieved: False)
- https://github.com/mizorewww/laya-mlx → [documentation] https://github.com/mizorewww/laya-mlx/blob/main/benchmarks/results (host:text:L362; target retrieved: False)
- https://github.com/mizorewww/laya-mlx → [documentation] https://github.com/mizorewww/laya-mlx/blob/main/docs/PERFORMANCE_RESEARCH.md (host:text:L370; target retrieved: False)
- https://github.com/mizorewww/laya-mlx → [documentation] https://github.com/mizorewww/laya-mlx/blob/main/docs/MATH_10X_RESEARCH.md (host:text:L371; target retrieved: False)
- https://github.com/mizorewww/laya-mlx → [documentation] https://github.com/mizorewww/laya-mlx/blob/main/docs/ENGINEERING_10X_RESEARCH.md (host:text:L372; target retrieved: False)
- https://github.com/mizorewww/laya-mlx → [documentation] https://github.com/mizorewww/laya-mlx/blob/main/experiments (host:text:L374; target retrieved: False)
- https://github.com/mizorewww/laya-mlx → [documentation] https://github.com/mizorewww/laya-mlx/blob/main/LICENSE (host:text:L389; target retrieved: False)
- https://github.com/mizorewww/laya-mlx → [documentation] https://github.com/mizorewww/laya-mlx/blob/main/NOTICE (host:text:L389; target retrieved: False)
- https://github.com/mizorewww/laya-mlx → [code] https://github.com/NandhaKishorM/laya (host:text:L389; target retrieved: False)
- https://github.com/mizorewww/laya-mlx/blob/main/BENCHMARKS.md → [documentation] https://github.com/mizorewww/laya-mlx/blob/main/benchmarks/latency.png (host:text:L19; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://colab.research.google.com/drive/15d4Yv__KHeHjshVb-6PRTfqVllxih2S3?usp=sharing (html:repository-readme/line 9, a[1]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://pypi.org/project/laya/ (html:repository-readme/line 10, a[2]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://nandhakishorm.github.io/laya/ (html:repository-readme/line 11, a[3]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://huggingface.co/convaiinnovations/laya (html:repository-readme/line 12, a[4]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://huggingface.co/convaiinnovations/laya-multilingual (html:repository-readme/line 13, a[5]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://huggingface.co/spaces/convaiinnovations/laya-demo (html:repository-readme/line 14, a[6]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://dev.to/nandakishor_m_6cc0adfde9f/i-built-non-autoregressive-decision-models-a-year-ago-then-a-frontier-lab-called-it-a-18me (html:repository-readme/line 15, a[7]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://www.buymeacoffee.com/nandakishorm (html:repository-readme/line 16, a[8]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://opensource.org/licenses/Apache-2.0 (html:repository-readme/line 17, a[9]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [code] https://github.com/NandhaKishorM/laya (html:repository-readme/line 19, a[10]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://docs.astral.sh/uv/ (html:repository-readme/line 21, a[11]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/tree/main/laya-ts/ (html:repository-readme/line 23, a[13]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/blob/main/research/scripts/bench_long_context.py (html:repository-readme/line 24, a[14]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://raw.githubusercontent.com/NandhaKishorM/laya/main/assets/long_context_8192.png (html:repository-readme/line 26, a[15]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/blob/main/notebooks/laya_finetune_typed_decisions_2xT4_kaggle.ipynb (html:repository-readme/line 86, a[20]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/blob/main/notebooks/laya_finetune_typed_decisions_mps.py (html:repository-readme/line 86, a[21]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://nandhakishorm.github.io/laya/hooks/ (html:repository-readme/line 88, a[25]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://nandhakishorm.github.io/laya/structured/ (html:repository-readme/line 88, a[26]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://nandhakishorm.github.io/laya/docker/ (html:repository-readme/line 88, a[27]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://nandhakishorm.github.io/laya/langchain/ (html:repository-readme/line 88, a[28]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://nandhakishorm.github.io/laya/reference/ (html:repository-readme/line 88, a[29]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [release] https://github.com/NandhaKishorM/laya/releases (html:repository-readme/line 109, a[31]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://raw.githubusercontent.com/NandhaKishorM/laya/main/assets/laya_vs_jev_full.png (html:repository-readme/line 112, a[32]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://huggingface.co/convaiinnovations/laya-typed-decisions (html:repository-readme/line 142, a[35]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/blob/main/examples/README.md (html:repository-readme/line 164, a[37]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/blob/main/LOCAL_SETUP.md (html:repository-readme/line 168, a[38]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/blob/main/BENCHMARKS.md (html:repository-readme/line 172, a[39]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/blob/main/research/README.md (html:repository-readme/line 176, a[40]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://pytorch.org/get-started/locally/ (html:repository-readme/line 183, a[42]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://docs.pytorch.org/docs/2.14/notes/get_start_xpu.html (html:repository-readme/line 202, a[43]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://docs.astral.sh/uv/guides/integration/pytorch/ (html:repository-readme/line 223, a[45]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://github.com/NandhaKishorM/laya/issues/123 (html:repository-readme/line 243, a[47]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://github.com/NandhaKishorM/laya/pull/195 (html:repository-readme/line 244, a[48]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/blob/main/sdk/typescript/README.md (html:repository-readme/line 447, a[57]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/blob/main/docs/typescript-sdk.md (html:repository-readme/line 473, a[59]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/blob/main/docs/docker.md (html:repository-readme/line 477, a[61]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/blob/main/docs/hooks/lifecycle.md (html:repository-readme/line 672, a[67]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [code] https://github.com/getmissionctrl/hs-jev (html:repository-readme/line 831, a[73]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [code] https://github.com/marcreichel/laya-php (html:repository-readme/line 833, a[74]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://github.com/NandhaKishorM/laya/issues/394 (html:repository-readme/line 893, a[77]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [code] https://github.com/tile-ai/tilelang (html:repository-readme/line 1056, a[84]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/blob/main/docs/compile-and-fast-path.md (html:repository-readme/line 1095, a[88]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/blob/main/docs/langchain.md (html:repository-readme/line 1143, a[93]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/blob/main/docs/hooks/index.md (html:repository-readme/line 1203, a[95]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/tree/main/examples/hooks/ (html:repository-readme/line 1203, a[96]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/blob/main/docs/structured.md (html:repository-readme/line 1239, a[98]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://github.com/NandhaKishorM/laya/issues/131 (html:repository-readme/line 1434, a[105]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [paper] https://arxiv.org/abs/2212.10947 (html:repository-readme/line 1479, a[107]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://modelcontextprotocol.io/ (html:repository-readme/line 1529, a[109]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/blob/main/docs/cli-mcp.md (html:repository-readme/line 1540, a[110]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/blob/main/laya/serve.py (html:repository-readme/line 1558, a[111]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/blob/main/docs/evals.md (html:repository-readme/line 1636, a[116]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/blob/main/research/benchmarks/feishu_zh/README.md (html:repository-readme/line 1639, a[118]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/blob/main/research/benchmarks/feishu_zh/README.zh-CN.md (html:repository-readme/line 1639, a[119]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/blob/main/research/benchmarks/zh_short_commands/README.md (html:repository-readme/line 1639, a[120]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/blob/main/research/benchmarks/zh_short_commands/README.zh-CN.md (html:repository-readme/line 1639, a[121]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://raw.githubusercontent.com/NandhaKishorM/laya/main/assets/laya_benchmark.png (html:repository-readme/line 1642, a[123]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/blob/main/research/scripts/laya_benchmark_colab.ipynb (html:repository-readme/line 1646, a[124]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [code] https://github.com/AbdelStark/jev-benchmarks (html:repository-readme/line 1681, a[126]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [code] https://github.com/nibzard/decision-model-benchmark (html:repository-readme/line 1682, a[127]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://github.com/NandhaKishorM/laya/issues/377 (html:repository-readme/line 1955, a[139]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/blob/main/research/benchmarks/tournament/README.md (html:repository-readme/line 2019, a[141]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://github.com/NandhaKishorM/laya/issues/102 (html:repository-readme/line 2066, a[142]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://github.com/NandhaKishorM/laya/issues/156 (html:repository-readme/line 2090, a[143]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [code] https://github.com/F0Rextasy/omp-laya-judge (html:repository-readme/line 2107, a[145]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [code] https://github.com/can1357/oh-my-pi (html:repository-readme/line 2107, a[146]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [code] https://github.com/Ashfaqbs/laya-adk-toolkit (html:repository-readme/line 2108, a[147]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://google.github.io/adk-docs/ (html:repository-readme/line 2108, a[148]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [code] https://github.com/zzhdbw/laya-Ascend (html:repository-readme/line 2109, a[149]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [code] https://github.com/tc3oliver/laya-apple (html:repository-readme/line 2110, a[150]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [code] https://github.com/bladedevoff/stuntd (html:repository-readme/line 2111, a[151]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [documentation] https://github.com/NandhaKishorM/laya/blob/main/docs/finetune_browser_agent.md (html:repository-readme/line 2156, a[160]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [code] https://github.com/browser-use/jev-ultrafast (html:repository-readme/line 2158, a[161]/@href; target retrieved: False)
- https://github.com/NandhaKishorM/laya → [references] https://huggingface.co/cklxx/laya-browser (html:repository-readme/line 2161, a[162]/@href; target retrieved: False)

## Partial coverage

- https://github.com/mizorewww/laya-mlx/blob/main/README.md: budget_exhausted (call budget exhausted)

## Next directions

有合适 Mac 时，按原文条件比较 MLX 与上游 PyTorch 的同任务正确率及延迟，并单列冷启动、批处理和内存；Windows 上先调查可用的 CPU 决策模型实现。

- https://github.com/mizorewww/laya-mlx/blob/main/benchmarks/latency.png: documentation
- https://github.com/mizorewww/laya-mlx/blob/main/README.md: budget_limit
- https://github.com/NandhaKishorM/laya: budget_limit
- https://github.com/mizorewww/laya-mlx/blob/main/docs/SNAKE_DEMO.md: budget_limit
- https://github.com/mizorewww/laya-mlx/blob/main/README.zh-CN.md: budget_limit
- https://github.com/mizorewww/laya-mlx/blob/main/docs/SNAKE_BENCHMARKS.md: budget_limit
- https://github.com/mizorewww/laya-mlx/blob/main/LICENSE: budget_limit
- https://github.com/mizorewww/laya-mlx/blob/main/benchmarks/results/hub-publication.json: budget_limit
- https://github.com/mizorewww/laya-mlx/blob/main/docs/assets/snake-demo.mp4: budget_limit
- https://github.com/mizorewww/laya-mlx/blob/main/docs/PERFORMANCE_RESEARCH.md: budget_limit
- https://github.com/mizorewww/laya-mlx/blob/main/docs/SNAKE_OPTIMIZATION.md: budget_limit
- https://github.com/mizorewww/laya-mlx/blob/main/NOTICE: budget_limit
- https://huggingface.co/aac6fef/laya-typed-decisions-mlx: budget_limit
- https://huggingface.co/aac6fef/laya-mlx: budget_limit
- https://github.com/NandhaKishorM/laya/commit/1adc59f7e371deb601fcfa18a14e25db238addcc: budget_limit
- https://github.com/mizorewww/laya-mlx/blob/main/benchmarks/results/upstream-v041-validation.json: budget_limit
- https://github.com/mizorewww/laya-mlx/blob/main/benchmarks/results: budget_limit
- https://raw.githubusercontent.com/mizorewww/laya-mlx/main/docs/assets/snake-demo.gif: budget_limit
- https://github.com/mizorewww/laya-mlx/blob/main/docs/MATH_10X_RESEARCH.md: budget_limit
- https://github.com/mizorewww/laya-mlx/blob/main/docs/ENGINEERING_10X_RESEARCH.md: budget_limit
- https://github.com/mizorewww/laya-mlx/blob/main/experiments: budget_limit
- https://huggingface.co/aac6fef/laya-multilingual-mlx: budget_limit

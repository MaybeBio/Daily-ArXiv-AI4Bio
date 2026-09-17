# AI4Bio Daily ArXiv Papers
The project automatically fetches the latest papers from arXiv based on keywords related to computational biology.

`Each topic below shows only papers from the last 7 days (a recent view)`. The complete archive — including everything shown here — is stored under `papers/`, one folder per topic and one file per month. Papers are not duplicated: the links below are the same entries kept in `papers/`. Click the archive link under each topic to browse the full history.

Papers are accumulated over time (never removed) and deduplicated by arXiv id.

Last update: 2026-09-18


<!-- MANUAL:START -->
> ⚠️ Add your own notes here. This block is preserved across automatic updates.

|产物|内容 |数据来源|是否累积|
|--|--|--|--|
|README|近 7 天文献（每个 topic 一个表格）|从 archive 里读 recent_rows_for_topic(days=7)|滚动 7 天窗口|
|每日 Issue|当天这次运行新抓到且去重后新增的文献（现在显示全部）|new_papers_by_topic|快照，每天一份|
|archive (papers/) |全部历史文献，按 topic/月归档|每次运行 append |永久积累，只增不减|


- [x] Adapted and Modified from [DailyArXiv](https://github.com/zezhishao/DailyArXiv)

> 🌟 Todo
> - [ ] 整体workflow可再修改调整：https://github.com/Vincentqyw/cv-arxiv-daily、YuzeHao2023
> 
> - [ ] 后续需要修改+调整+范围收缩/新增 Topic：
>     - [ ] 新增收束 DNA、ZF：MD
>     - [ ] 新增收束 IDR、interaction、ensemble
>
> - [ ] post-processing善后：
>   - [ ] 如何批阅、整理每篇文献，也就是如何承接下游阅读流，zotero-MCP？
>      
> - [ ] 需要新增功能：翻译、Agent总结，对高通量paper先人工降噪一部分，参考: https://github.com/RainerSeventeen/paper-tracker
>
> - [ ] 能否用上GitHub pages
> - [ ] JasonEtco/create-an-issue@v2 的workflow warning：Node.js 20 is deprecated

Also refer to: https://www.arxivdaily.com/
<!-- MANUAL:END -->

## Intrinsically Disordered Proteins (IDR)

No new papers in the last 7 days.

Archive: [papers/IDR/](papers/IDR/)

## Protein-DNA Modeling & Simulation (PDA)

No new papers in the last 7 days.

Archive: [papers/PDA/](papers/PDA/)

## Protein Structure Deep Learning (PSA)

| **Title** | **Date** | **Abstract** | **Comment** |
| --- | --- | --- | --- |
| **[OpenAI4S: Code as Action, Science as Sessions](https://arxiv.org/abs/2609.15096v1)** | 2026-09-14 | <details><summary>Show</summary><p>AI co-scientists could accelerate computational research, but over a long-running study the workflow also has to stay inspectable, resumable and reproducible, which requires persistent computational state and provenance. Here we present OpenAI4S, an open-source scientific research agent built around the principle of \emph{Code as Action, Science as Sessions}. OpenAI4S combines a persistent computing runtime with research-session management: orchestration is handled through structured tool calls, while scientific actions are represented as complete code cells executed in persistent Python and R kernels. An append-only Action Ledger, per-cell execution records, versioned artifacts, environment records, and workspace checkpoints preserve how results were produced and support session recovery, branching, and extension. Configurable sandboxing, permission controls, and code and trajectory screening provide complementary safeguards. We evaluate OpenAI4S on 36 research scenarios spanning retrosynthesis, molecular dynamics, protein binder design, protein mutation, catalyst screening, and mineral spectroscopy, measuring scientific task accuracy, workflow completeness, and reproducibility of the resulting repositories. OpenAI4S achieves an overall score of 7.83, compared with 5.7--6.4 for a general-purpose coding harness evaluated with three frontier models, with the largest gains on long-horizon and computation-intensive workflows. These results suggest that integrating persistent execution with session-level provenance can improve the reliability of AI-assisted scientific workflows. Environment specification and full rerunnability remain weak for every evaluated system, ours included, so reproducibility is still an open problem for scientific agents. The system is available under the MIT license at \href{https://github.com/PKU-YuanGroup/OpenAI4S}{github.com/PKU-YuanGroup/OpenAI4S}.</p></details> |  |
| **[Ensemble-Conditioned Molecular Design](https://arxiv.org/abs/2609.15077v1)** | 2026-09-14 | <details><summary>Show</summary><p>Molecular design is typically approached as a problem of finding molecules which can adopt a single bioactive conformation. In reality, molecules occupy a distribution over conformations, and many of the properties which determine whether a candidate is viable depend on that distribution rather than on any single conformer. We reframe molecular design as an optimisation of both the modes and properties of molecules' conformational ensembles, where modes can be represented as shapes, pharmacophore profiles or protein pockets, and properties are aggregate scalars computed over the whole distribution. To realise this we introduce ensemble-conditioned guidance, a framework which conditions 3D molecular generative models on both axes simultaneously. Mode conditions are composed adaptively at inference by combining the vector fields produced under each condition. Conditions may be targeted or avoided, mixed across modalities and combined in arbitrary numbers, allowing a wide range of design tasks to be expressed with a single trained model. We introduce adaptive symmetry learning to allow conditions from different reference frames to be composed, and extend our generative framework to enable flexible-size generation. We evaluate on new benchmarks for multi-mode conditioning and ensemble property optimisation, and apply the framework to two practical drug discovery tasks, dual-target binder design and active-state-selective agonist design, where in both cases conditioning on the additional state improves the desired outcome over single-state conditioning.</p></details> | <details><summary>Code ...</summary><p>Code available at: https://github.com/rssrwn/ensemble-cond-design datasets and checkpoints available at: https://zenodo.org/records/22485204</p></details> |

Archive: [papers/PSA/](papers/PSA/)


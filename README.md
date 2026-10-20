# AI4Bio Daily ArXiv Papers
The project automatically fetches the latest papers from arXiv based on keywords related to computational biology.

`Each topic below shows only papers from the last 7 days (a recent view)`. The complete archive — including everything shown here — is stored under `papers/`, one folder per topic and one file per month. Papers are not duplicated: the links below are the same entries kept in `papers/`. Click the archive link under each topic to browse the full history.

Papers are accumulated over time (never removed) and deduplicated by arXiv id.

Last update: 2026-10-21


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
| **[ProtGlycanDock: Towards Accurate Protein-Glycan Docking with Tailored Dataset, Benchmark and Model](https://arxiv.org/abs/2610.26009v1)** | 2026-10-19 | <details><summary>Show</summary><p>Performing accurate protein-glycan docking is critical to understanding protein-glycan interactions which govern many biological processes. However, this important task is hampered by the lack of tailored datasets, benchmarks and models for protein-glycan docking. To fill this blank, we first curate a standard benchmark ProtGlycanDock for training and evaluating protein-glycan docking models under both protein and glycan generalization settings. On this benchmark, we evaluate ten models in three categories, physics-based docking methods, machine-learning-based docking models and molecular structure prediction models. To obtain more precise binding poses, we further propose two finetuning techniques to inject the knowledge of glycan conformations into a general-purpose molecular structure prediction model. These two techniques respectively augment model inputs with glycan topological features and refine glycan binding pose with a glycan energy loss. Benchmark results show the superiority of AlphaFold 3 among existing methods, and the two proposed finetuning techniques can be well combined to achieve a state-of-the-art model for protein-glycan docking. Also, we perform stratified benchmark analysis and case studies to better understand the strengths and weaknesses of current models, providing insights for future model improvements. We maintain datasets at https://huggingface.co/datasets/ProtGlycanDock/ProtGlycanDock and source codes at https://github.com/kasawa1234/ProtGlycanDock</p></details> | <details><summary>Accep...</summary><p>Accepted by NeurIPS 2026 Evaluations and Datasets Track. Datasets and source codes are released</p></details> |

Archive: [papers/PSA/](papers/PSA/)


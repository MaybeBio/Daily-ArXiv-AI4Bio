# AI4Bio Daily ArXiv Papers
The project automatically fetches the latest papers from arXiv based on keywords related to computational biology.

`Each topic below shows only papers from the last 7 days (a recent view)`. The complete archive — including everything shown here — is stored under `papers/`, one folder per topic and one file per month. Papers are not duplicated: the links below are the same entries kept in `papers/`. Click the archive link under each topic to browse the full history.

Papers are accumulated over time (never removed) and deduplicated by arXiv id.

Last update: 2026-10-02


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
| **[Computational Insights into Mechanostability and Dissociation Dynamics of the Dengue Virus Envelope Protein Ectodomain Dimer Across pH and Temperature Gradients](https://arxiv.org/abs/2609.40151v1)** | 2026-09-30 | <details><summary>Show</summary><p>Dengue virus (DENV) is an enveloped flavivirus of major public health importance. Its envelope (E) protein mediates viral entry through homodimer dissociation and subsequent membrane fusion, making it one of the principal targets for antiviral strategies. To investigate the molecular determinants of this process, we performed steered molecular dynamics (SMD) simulations of the E protein ectodomain (ecE) dimer from DENV-2 and DENV-3 under variable pH and temperature conditions. Force-extension analyses revealed a highly stable interface for both serotypes, with rupture forces exceeding 1000 pN. pH and temperature had modest effects on overall mechanical resistance. However, DENV-3 displayed a distinct sensitivity to thermal stress compared to DENV-2. We identified a robust, asymmetric dissociation pathway across all conditions, characterized by a metastable intermediate state involving partial dimer opening and exposure of the fusion loop (FL). This intermediate exposes an immunodominant epitope and persists under physiological conditions, suggesting it as a viable target for therapeutic intervention. The primary contributions to the interfacial interaction network were found to arise from van der Waals interactions, followed by hydrogen bonds, salt bridges, and pi-cation interactions. DENV-3 exhibited a slightly greater contribution from polar interactions involving domains EDI, EDII, and EDIII. Furthermore, pairwise occupancy analysis identified pH-sensitive contacts that are disrupted under acidic conditions, particularly in DENV-3, providing mechanistic insight into the early stages of ecE dissociation. Together, these findings provide structural insights into the dissociation mechanism, identifying key metastable states and pH-sensitive interactions that could be exploited to develop antivirals that stabilize the dimer and prevent viral fusion.</p></details> | <details><summary>28 pa...</summary><p>28 pages, 5 figures, 7 supplementary figures. Supporting Information included</p></details> |
| **[CellMSA: Context Modeling for Single-Cell Representation Learning](https://arxiv.org/abs/2609.38908v1)** | 2026-09-30 | <details><summary>Show</summary><p>Single-cell transcriptomics enables profiling of cellular states at unprecedented resolution, but its high dimensionality, sparsity, and technical batch effects pose significant challenges for representation learning. Existing single-cell foundation models typically encode each cell independently or only model cells from the same batch for denoising, thereby underutilizing the rich relational information across batches and cell types to model gene expression patterns. We argue that single-cell models can benefit from more informative cell-context modeling. By comparing consistency and variation across cells, models can capture fine-grained gene-gene dependencies associated with cell states, which are essential for learning high-quality representations. Inspired by the use of multiple sequence alignment (MSA) context in protein modeling, we propose CellMSA, a single-cell representation learning framework that introduces an MSA-inspired inductive bias into transcriptomic modeling. For each target cell, CellMSA retrieves relevant cells from different batches and biologically related cell types as context, and summarizes cross-cell patterns into a context-dependent gene-pair representation. This representation is then injected into a pair-aware target-cell encoder for fine-grained representation learning. We pretrain CellMSA on a large-scale human single-cell corpus of approximately 109 million cell observations, including 65.6 million primary observations. Experiments show that our framework consistently outperforms existing methods across multiple benchmarks. Code is available at the following repository: https://github.com/PharMolix/CellMSA.</p></details> | <details><summary>Accep...</summary><p>Accepted by NeurIPS 2026, code released</p></details> |
| **[SPINET: Sheaf Protein Inverse Folding Network](https://arxiv.org/abs/2609.34153v1)** | 2026-09-28 | <details><summary>Show</summary><p>Proteins change shape as they function, yet most inverse folding models predict amino acid sequences from a single, fixed backbone. A central challenge in protein engineering is to design proteins that undergo specific motions, which requires accounting for how their structures change over time. This motivates inverse protein folding conditioned on protein motion. We introduce SPINET, which predicts sequences from molecular dynamics trajectories. It uses cellular sheaves to represent residue interactions within each frame and recurrent units to integrate information across frames, then predicts all amino acids in a single pass. We evaluate SPINET on mdCATH and ATLAS, where it outperforms all evaluated static and ensemble baselines in sequence recovery. On mdCATH, it achieves 56.7% top-1 recovery, compared with 44.5% for the strongest static baseline and 40.7% for the strongest ensemble baseline. We also evaluate whether the predicted sequences are compatible with conformations sampled along the target trajectory. On mdCATH, they achieve a median TM-score of 0.760, and structural recovery favors target conformations over unrelated decoys for 99.5% of test domains.</p></details> |  |
| **[Robust Biomolecular Complex Design Across Protein Conformational Landscapes](https://arxiv.org/abs/2609.33726v1)** | 2026-09-27 | <details><summary>Show</summary><p>Proteins populate conformational ensembles, yet structure-based biomolecular design typically optimizes candidates against a single target conformation. Consequently, a candidate that fits one state can lose favorable interactions or develop steric clashes when the target adopts another. We introduce FlexEvo, a model-agnostic evolutionary framework that adapts candidates once at inference time from a single target conformation to improve compatibility with alternative natural conformations unseen during adaptation, without retraining the source model or requiring a conformational ensemble. FlexEvo casts cross-state adaptation as geometry-constrained bi-objective optimization, balancing preservation of input-state interactions against robustness to plausible conformational perturbations. To limit the search space and reduce invalid structural edits, geometry-derived FlexBoxes define protected anchor regions, adaptable regions for local exploration, and forbidden regions for clash avoidance. A unified all-atom representation supports topology-preserving adaptation across diverse binder categories, while Pareto selection preserves nondominated candidates across the two objectives. We evaluate FlexEvo across multiple generation baselines and nine representative binder categories spanning diverse molecular sizes and structural topologies. FlexEvo reduces the category-balanced mean relative performance degradation from 47.8% to 4.4%, while adding only 1.4--3.1 minutes of adaptation per sample. These results establish single-state inference-time adaptation as a practical route toward robust biomolecular complex design across protein conformational landscapes.</p></details> |  |

Archive: [papers/PSA/](papers/PSA/)


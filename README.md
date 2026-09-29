# AI4Bio Daily ArXiv Papers
The project automatically fetches the latest papers from arXiv based on keywords related to computational biology.

`Each topic below shows only papers from the last 7 days (a recent view)`. The complete archive — including everything shown here — is stored under `papers/`, one folder per topic and one file per month. Papers are not duplicated: the links below are the same entries kept in `papers/`. Click the archive link under each topic to browse the full history.

Papers are accumulated over time (never removed) and deduplicated by arXiv id.

Last update: 2026-09-30


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
| **[SPINET: Sheaf Protein Inverse Folding Network](https://arxiv.org/abs/2609.34153v1)** | 2026-09-28 | <details><summary>Show</summary><p>Proteins change shape as they function, yet most inverse folding models predict amino acid sequences from a single, fixed backbone. A central challenge in protein engineering is to design proteins that undergo specific motions, which requires accounting for how their structures change over time. This motivates inverse protein folding conditioned on protein motion. We introduce SPINET, which predicts sequences from molecular dynamics trajectories. It uses cellular sheaves to represent residue interactions within each frame and recurrent units to integrate information across frames, then predicts all amino acids in a single pass. We evaluate SPINET on mdCATH and ATLAS, where it outperforms all evaluated static and ensemble baselines in sequence recovery. On mdCATH, it achieves 56.7% top-1 recovery, compared with 44.5% for the strongest static baseline and 40.7% for the strongest ensemble baseline. We also evaluate whether the predicted sequences are compatible with conformations sampled along the target trajectory. On mdCATH, they achieve a median TM-score of 0.760, and structural recovery favors target conformations over unrelated decoys for 99.5% of test domains.</p></details> |  |
| **[Robust Biomolecular Complex Design Across Protein Conformational Landscapes](https://arxiv.org/abs/2609.33726v1)** | 2026-09-27 | <details><summary>Show</summary><p>Proteins populate conformational ensembles, yet structure-based biomolecular design typically optimizes candidates against a single target conformation. Consequently, a candidate that fits one state can lose favorable interactions or develop steric clashes when the target adopts another. We introduce FlexEvo, a model-agnostic evolutionary framework that adapts candidates once at inference time from a single target conformation to improve compatibility with alternative natural conformations unseen during adaptation, without retraining the source model or requiring a conformational ensemble. FlexEvo casts cross-state adaptation as geometry-constrained bi-objective optimization, balancing preservation of input-state interactions against robustness to plausible conformational perturbations. To limit the search space and reduce invalid structural edits, geometry-derived FlexBoxes define protected anchor regions, adaptable regions for local exploration, and forbidden regions for clash avoidance. A unified all-atom representation supports topology-preserving adaptation across diverse binder categories, while Pareto selection preserves nondominated candidates across the two objectives. We evaluate FlexEvo across multiple generation baselines and nine representative binder categories spanning diverse molecular sizes and structural topologies. FlexEvo reduces the category-balanced mean relative performance degradation from 47.8% to 4.4%, while adding only 1.4--3.1 minutes of adaptation per sample. These results establish single-state inference-time adaptation as a practical route toward robust biomolecular complex design across protein conformational landscapes.</p></details> |  |
| **[When Riemann flows with Wasserstein: Generative Modeling of Probability Distributions on Manifolds](https://arxiv.org/abs/2609.25659v1)** | 2026-09-22 | <details><summary>Show</summary><p>Many scientific datasets, such as molecular conformational ensembles or single-cell tissue measurements, are naturally modeled as meta-distributions: distributions over probability measures on non-Euclidean domains. Existing generative methods largely assume Euclidean geometry and fail to capture this structure. We introduce Riemannian Wasserstein Entropic Flow Matching (RWEFM), a generative framework on the Wasserstein space $\mathcal{P}_2(\mathcal{M})$ of a Riemannian manifold $(\mathcal{M},g)$. RWEFM is trained by regressing a neural vector field onto Riemannian optimal transport velocities, using McCann displacement interpolations as conditional paths. We confirm theoretically that this construction leads to a valid flow matching approach on $\mathcal{P}_2(\mathcal{M})$ and introduce the Riemannian Entropic Map, a GPU-efficient approximation of the optimal transport map on manifolds. Our experiments show that by respecting the intrinsic geometry of the data, RWEFM can generate whole single-cell samples in hyperspherical latent spaces and protein conformational ensembles on the torus. As RWEFM requires only a geodesic distance and a projection operator, it is not restricted to manifolds with closed-form geometry, which we demonstrate by generating distributions on a general triangulated mesh.</p></details> |  |

Archive: [papers/PSA/](papers/PSA/)


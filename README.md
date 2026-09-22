# AI4Bio Daily ArXiv Papers
The project automatically fetches the latest papers from arXiv based on keywords related to computational biology.

`Each topic below shows only papers from the last 7 days (a recent view)`. The complete archive — including everything shown here — is stored under `papers/`, one folder per topic and one file per month. Papers are not duplicated: the links below are the same entries kept in `papers/`. Click the archive link under each topic to browse the full history.

Papers are accumulated over time (never removed) and deduplicated by arXiv id.

Last update: 2026-09-23


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

| **Title** | **Date** | **Abstract** | **Comment** |
| --- | --- | --- | --- |
| **[FOSY: Segmental Backbone Assignment in Intrinsically Disordered Proteins](https://arxiv.org/abs/2609.20384v1)** | 2026-09-17 | <details><summary>Show</summary><p>Backbone resonance assignment is a prerequisite for most biomolecular NMR applications, yet conventional multidimensional strategies frequently fail for intrinsically disordered proteins (IDPs) and regions (IDRs) because of severe spectral overlap, rapid amide proton exchange with water, and missing sequential correlations. In many biological applications, however, complete protein assignment is unnecessary, as only a limited sequence segment surrounding a functional site is required. Here we introduce segmental backbone assignment, an assignment strategy implemented by FOcused SpectroscopY (FOSY), which concentrates experimental effort on relatively short regions while retaining the high-dimensional sequential connectivity needed for unambiguous assignments. We present a self-consistent suite of selective two-dimensional FOSY experiments that enables bidirectional assignment walks along the protein sequence through complementary forward and backward transfer schemes. The methodology employs frequency-selective polarisation transfer to replace high-dimensional experiments with sensitive and readily interpretable 2D spectra while preserving the information content of multidimensional correlation experiments. The approach is demonstrated by completing the assignment of G302-K311 segment, which is missing in the published assignment of the 441-residue human Tau protein. The approach complements conventional multidimensional or residue type-selective assignment strategies by providing an efficient means of traversing assignment interruptions and rapidly characterising functionally important segments in intrinsically disordered proteins.</p></details> |  |

Archive: [papers/IDR/](papers/IDR/)

## Protein-DNA Modeling & Simulation (PDA)

No new papers in the last 7 days.

Archive: [papers/PDA/](papers/PDA/)

## Protein Structure Deep Learning (PSA)

| **Title** | **Date** | **Abstract** | **Comment** |
| --- | --- | --- | --- |
| **[Nucleosome simulations suggest mechanisms of electrostatically-driven mesoscale chromatin evolution](https://arxiv.org/abs/2609.24907v1)** | 2026-09-21 | <details><summary>Show</summary><p>Nucleosomes are structures made up of proteins called histones that bind and compact DNA, driving the mesoscale organization of the chromatin polymer. Although histone proteins have diversified over evolutionary time, their contributions to the corresponding diversification of chromatin structure are poorly understood. Here, we mine protein databases for histones and create \emph{in silico} nucleosomes for 3241 organisms spanning $>$1.5B years of evolution. Using a combination of electrostatic calculations and coarse-grained molecular dynamics simulations, we reveal extensive biophysical diversification of the nucleosome unit. Finally, we perform coarse-grained oligonucleosomal simulations on a subset of evolutionarily and biophysically divergent nucleosomes, demonstrating dramatic differences in bulk phase behavior of chromatin. Taken together, our results suggest a paradigm in which histones may have evolved to facilitate particular types of mesoscale chromatin behavior.</p></details> | working paper |
| **[TorchCraft: Unified binder design by inverting an all-atom structure predictor](https://arxiv.org/abs/2609.19770v1)** | 2026-09-17 | <details><summary>Show</summary><p>All-atom structure predictors model diverse molecular interactions, but using their learned structural priors for binder design remains challenging. Here we present TorchCraft, a unified binder-design framework that optimizes sequence logits through a frozen all-atom predictor. Implemented in TorchFold, TorchCraft combines confidence, contact, geometric, and sequence-prior objectives within a shared optimization procedure for minibinders, framework-conditioned VHHs, cyclic peptides, and ligand-binding proteins. Using pretrained AlphaFold 3 weights, TorchCraft generated representative minibinders and VHHs with experimentally measured binding across four targets in each format, without post hoc sequence redesign. Computational benchmarks further demonstrated the framework's applicability to cyclic peptides and ligand-conditioned pocket design. TorchCraft extends predictor inversion to multiple binder formats and molecular contexts, providing a common framework for reusing all-atom structural priors in design.</p></details> |  |
| **[Machine-Learned Dynamical Representations for Accelerated RiteWeight Convergence](https://arxiv.org/abs/2609.19388v1)** | 2026-09-16 | <details><summary>Show</summary><p>The increasing use of generative models has made ensembles of short molecular dynamics trajectories increasingly common, creating a growing need for methods that can recover physically meaningful steady-state populations and kinetics from improperly weighted conformational ensembles. Randomized Iterative Trajectory Reweighting (RiteWeight) addresses this problem through repeated random clustering and iterative reweighting, without requiring the fixed Markovian discretization used in conventional Markov state models (MSM). However, the choice of reduced feature space in which RiteWeight performs random clustering has not been systematically investigated. Here, we compare two machine-learned representations, DeepTICA and SPIB-VAE, with linear TICA for recovering steady-state observables from flawed distributions. DeepTICA learns nonlinear coordinates by targeting slow transfer-operator eigenmodes, whereas SPIB-VAE compresses configurations into a low-dimensional latent space while retaining information predictive of future metastable states. DeepTICA provided a comparatively robust RiteWeight representation under limited hyperparameter exploration, whereas SPIB-VAE benefited more strongly from broader optimization. Moreover, a kinetic score computed from a coarse MSM at a resolution comparable to that used for RiteWeight random clustering provided a useful criterion for efficiently selecting reduced representations and their hyperparameters for RiteWeight.</p></details> |  |

Archive: [papers/PSA/](papers/PSA/)


# AI4Bio Daily ArXiv Papers
The project automatically fetches the latest papers from arXiv based on keywords related to computational biology.

`Each topic below shows only papers from the last 7 days (a recent view)`. The complete archive — including everything shown here — is stored under `papers/`, one folder per topic and one file per month. Papers are not duplicated: the links below are the same entries kept in `papers/`. Click the archive link under each topic to browse the full history.

Papers are accumulated over time (never removed) and deduplicated by arXiv id.

Last update: 2026-09-25


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
| **[MT-ProtBERT: Multi-task Learning ProtBERT for Intrinsically Disordered Proteins Classification with Scarce Data](https://arxiv.org/abs/2609.25334v1)** | 2026-09-21 | <details><summary>Show</summary><p>Intrinsically disordered proteins (IDPs) differ from folded proteins in that they are dynamic, lack a stable three-dimensional conformation, and have low sequence similarity between similar proteins. The conformational heterogeneity of IDPs - while beneficial for their diverse functions - limits the use of traditional experimental tools to determine their conformation. The experimental difficulty, along with low sequence similarity, results in data scarcity, and makes it difficult to classify/detect IDPs that are similar or dissimilar, a task relevant to understand biology and evolution. We address this challenge using Multi-task ProtBERT (MT-ProtBERT), a multi-task extension of ProtBERT tailored for low-data regimes. MT-ProtBERT integrates Dynamic Window Masking, a Multi-Scale 1D Convolutional classifier (MS-Conv1D), and auxiliary objectives that jointly optimize masked language modeling and biochemistry-informed tasks. We evaluate this framework on two tasks under limited data: (i) phosphorylation site prediction (S/T/Y) in short sequences and small datasets, and (ii) protein compaction prediction on two small datasets (684 and 530 sequences), including sequences comparable in length to typical disordered regions. MT-ProtBERT consistently outperforms PARROT, an RNN-based IDP-specific model, across all tasks. These results demonstrate that combining self-supervised and biochemistry-informed tasks, and multi-scale learning enables robust modeling of unstructured proteins under data scarcity.</p></details> | <details><summary>14 pa...</summary><p>14 pages, 6 figures, 12 tables</p></details> |
| **[FOSY: Segmental Backbone Assignment in Intrinsically Disordered Proteins](https://arxiv.org/abs/2609.20384v1)** | 2026-09-17 | <details><summary>Show</summary><p>Backbone resonance assignment is a prerequisite for most biomolecular NMR applications, yet conventional multidimensional strategies frequently fail for intrinsically disordered proteins (IDPs) and regions (IDRs) because of severe spectral overlap, rapid amide proton exchange with water, and missing sequential correlations. In many biological applications, however, complete protein assignment is unnecessary, as only a limited sequence segment surrounding a functional site is required. Here we introduce segmental backbone assignment, an assignment strategy implemented by FOcused SpectroscopY (FOSY), which concentrates experimental effort on relatively short regions while retaining the high-dimensional sequential connectivity needed for unambiguous assignments. We present a self-consistent suite of selective two-dimensional FOSY experiments that enables bidirectional assignment walks along the protein sequence through complementary forward and backward transfer schemes. The methodology employs frequency-selective polarisation transfer to replace high-dimensional experiments with sensitive and readily interpretable 2D spectra while preserving the information content of multidimensional correlation experiments. The approach is demonstrated by completing the assignment of G302-K311 segment, which is missing in the published assignment of the 441-residue human Tau protein. The approach complements conventional multidimensional or residue type-selective assignment strategies by providing an efficient means of traversing assignment interruptions and rapidly characterising functionally important segments in intrinsically disordered proteins.</p></details> |  |

Archive: [papers/IDR/](papers/IDR/)

## Protein-DNA Modeling & Simulation (PDA)

No new papers in the last 7 days.

Archive: [papers/PDA/](papers/PDA/)

## Protein Structure Deep Learning (PSA)

| **Title** | **Date** | **Abstract** | **Comment** |
| --- | --- | --- | --- |
| **[When Riemann flows with Wasserstein: Generative Modeling of Probability Distributions on Manifolds](https://arxiv.org/abs/2609.25659v1)** | 2026-09-22 | <details><summary>Show</summary><p>Many scientific datasets, such as molecular conformational ensembles or single-cell tissue measurements, are naturally modeled as meta-distributions: distributions over probability measures on non-Euclidean domains. Existing generative methods largely assume Euclidean geometry and fail to capture this structure. We introduce Riemannian Wasserstein Entropic Flow Matching (RWEFM), a generative framework on the Wasserstein space $\mathcal{P}_2(\mathcal{M})$ of a Riemannian manifold $(\mathcal{M},g)$. RWEFM is trained by regressing a neural vector field onto Riemannian optimal transport velocities, using McCann displacement interpolations as conditional paths. We confirm theoretically that this construction leads to a valid flow matching approach on $\mathcal{P}_2(\mathcal{M})$ and introduce the Riemannian Entropic Map, a GPU-efficient approximation of the optimal transport map on manifolds. Our experiments show that by respecting the intrinsic geometry of the data, RWEFM can generate whole single-cell samples in hyperspherical latent spaces and protein conformational ensembles on the torus. As RWEFM requires only a geodesic distance and a projection operator, it is not restricted to manifolds with closed-form geometry, which we demonstrate by generating distributions on a general triangulated mesh.</p></details> |  |
| **[Nucleosome simulations suggest mechanisms of electrostatically-driven mesoscale chromatin evolution](https://arxiv.org/abs/2609.24907v1)** | 2026-09-21 | <details><summary>Show</summary><p>Nucleosomes are structures made up of proteins called histones that bind and compact DNA, driving the mesoscale organization of the chromatin polymer. Although histone proteins have diversified over evolutionary time, their contributions to the corresponding diversification of chromatin structure are poorly understood. Here, we mine protein databases for histones and create \emph{in silico} nucleosomes for 3241 organisms spanning $>$1.5B years of evolution. Using a combination of electrostatic calculations and coarse-grained molecular dynamics simulations, we reveal extensive biophysical diversification of the nucleosome unit. Finally, we perform coarse-grained oligonucleosomal simulations on a subset of evolutionarily and biophysically divergent nucleosomes, demonstrating dramatic differences in bulk phase behavior of chromatin. Taken together, our results suggest a paradigm in which histones may have evolved to facilitate particular types of mesoscale chromatin behavior.</p></details> | working paper |
| **[TorchCraft: Unified binder design by inverting an all-atom structure predictor](https://arxiv.org/abs/2609.19770v1)** | 2026-09-17 | <details><summary>Show</summary><p>All-atom structure predictors model diverse molecular interactions, but using their learned structural priors for binder design remains challenging. Here we present TorchCraft, a unified binder-design framework that optimizes sequence logits through a frozen all-atom predictor. Implemented in TorchFold, TorchCraft combines confidence, contact, geometric, and sequence-prior objectives within a shared optimization procedure for minibinders, framework-conditioned VHHs, cyclic peptides, and ligand-binding proteins. Using pretrained AlphaFold 3 weights, TorchCraft generated representative minibinders and VHHs with experimentally measured binding across four targets in each format, without post hoc sequence redesign. Computational benchmarks further demonstrated the framework's applicability to cyclic peptides and ligand-conditioned pocket design. TorchCraft extends predictor inversion to multiple binder formats and molecular contexts, providing a common framework for reusing all-atom structural priors in design.</p></details> |  |

Archive: [papers/PSA/](papers/PSA/)


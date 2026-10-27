# AI4Bio Daily ArXiv Papers
The project automatically fetches the latest papers from arXiv based on keywords related to computational biology.

`Each topic below shows only papers from the last 7 days (a recent view)`. The complete archive — including everything shown here — is stored under `papers/`, one folder per topic and one file per month. Papers are not duplicated: the links below are the same entries kept in `papers/`. Click the archive link under each topic to browse the full history.

Papers are accumulated over time (never removed) and deduplicated by arXiv id.

Last update: 2026-10-28


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
| **[Beyond Static Structures: Linking Protein Dynamics to Function via DynaReason-Pro](https://arxiv.org/abs/2610.33804v1)** | 2026-10-24 | <details><summary>Show</summary><p>Intrinsically disordered proteins (IDPs) carry out their functions through heterogeneous conformational ensembles that reflect their dynamics, yet most protein function prediction methods rely on sequence or a single static structure. To this end, we introduce DynaReason-Pro, the first framework to jointly predict GO terms from conformational ensembles and generate natural-language functional rationales. We evaluate DynaReason-Pro on a curated IDP benchmark from the Protein Ensemble Database (PED), with sequence- and structure-cluster-disjoint splits to prevent data leakage. Variability-stratified evaluation shows the clearest gains in the high-conformational-variability regime.</p></details> |  |
| **[Emergent Entropic Forces Drive Inverse and Reentrant Phase Transitions in Condensates of Intrinsically Disordered Proteins](https://arxiv.org/abs/2610.30627v1)** | 2026-10-22 | <details><summary>Show</summary><p>We present a phenomenological, mean-field model for condensates of intrinsically disordered proteins that describes inverse phase transitions and qualitatively predicts reentrant phase behavior as a function of salt concentration. The model is based on a matrix-based formulation of the Flory-Huggins free energy, in which the enthalpic interaction parameter and the protein valence, defined here as the number of effective "sticky patches", are treated as free parameters. Its central insight is that integrating out dynamics of fast-moving molecular species generates an effective entropic force that increases the free-energy barrier to mixing, even within a mean-field description. We account for this by linking Gaussian integration of co-solutes to the Schur complement of the matrix-based Flory-Huggins free energy. This provides a general thermodynamic framework illustrating how enthalpic interactions that increase the number of available microstates necessarily induce effective entropic forces. We demonstrate the expressiveness and predictive power of the model by qualitatively reproducing recent experimental observations on the rabies virus phosphoprotein.</p></details> | <details><summary>20 pa...</summary><p>20 pages. 7 Figures. Comments welcome!</p></details> |

Archive: [papers/IDR/](papers/IDR/)

## Protein-DNA Modeling & Simulation (PDA)

No new papers in the last 7 days.

Archive: [papers/PDA/](papers/PDA/)

## Protein Structure Deep Learning (PSA)

| **Title** | **Date** | **Abstract** | **Comment** |
| --- | --- | --- | --- |
| **[mdRNAcat: A Molecular Dynamics RNA Catalog of REST2 Conformational Ensembles](https://arxiv.org/abs/2610.35204v1)** | 2026-10-26 | <details><summary>Show</summary><p>Learning molecular models of RNA requires simulation data that capture conformational variability and provide consistent physical training signals. Here, we introduce mdRNAcat, a curated dataset of all-atom molecular dynamics (MD) simulations of 48 RNA systems selected to promote sequence diversity. Each system is simulated using replica-exchange with solute scaling (REST2), with 32 Hamiltonian states and production lengths of 200-300 ns per state. The dataset provides atomic coordinates, instantaneous forces, and forces reevaluated under the unscaled reference Hamiltonian, together with structural annotations and replica-exchange metadata. Coordinates and forces are available at 1 ps intervals for the reference state and 100 ps intervals across all states in a standardized HDF5 format. We characterize conformational sampling, exchange behavior, base pairing, and sugar-pucker distributions to document the properties of the simulated ensembles. mdRNAcat provides a reusable resource for developing and evaluating data-driven RNA models, including coarse-grained force fields.</p></details> | <details><summary>24 pa...</summary><p>24 pages, 9 figures. Dataset and accompanying resources available on Hugging Face under the HelmholtzAI-FZJ organization</p></details> |
| **[Ensemble-Aware Structural Encoding (EASE): Conditioning Protein Encoders on Peptide Conformational Ensembles](https://arxiv.org/abs/2610.27638v1)** | 2026-10-20 | <details><summary>Show</summary><p>Protein foundation models provide transferable representations for downstream peptide prediction tasks. However, existing representations typically reduce a peptide to a single sequence or structure, which may miss conformational variability relevant to key peptide properties, including antibacterial activity, hemolysis, toxicity, stability, and binding. For example, protease resistance correlates more strongly with conformational dynamics measured by hydrogen exchange than with average helicity. Therefore, we introduce Ensemble-Aware Structural Encoding (EASE), a framework for effectively extracting structural information from conformational ensembles for peptide representation. To extract useful information from noisy conformers, EASE selects central conformers representing a peptide's major structural states and fuses their individual representations with a permutation-invariant operator to produce a peptide-level representation for downstream prediction. We then evaluate our framework on six peptide property-prediction tasks under leakage-controlled splits. Against matched single-structure baselines, EASE improves performance consistently on six tasks with a mean absolute gain of about 3.0% across two structural encoders. Gains keep growing as we add conformers through K=20. A single peptide conformer therefore provides a limited basis for structural representation, whereas our framework distilling and fusing multiple conformers yields a more informative representation.</p></details> |  |

Archive: [papers/PSA/](papers/PSA/)


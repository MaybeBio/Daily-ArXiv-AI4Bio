# AI4Bio Daily ArXiv Papers
The project automatically fetches the latest papers from arXiv based on keywords related to computational biology.

`Each topic below shows only papers from the last 7 days (a recent view)`. The complete archive — including everything shown here — is stored under `papers/`, one folder per topic and one file per month. Papers are not duplicated: the links below are the same entries kept in `papers/`. Click the archive link under each topic to browse the full history.

Papers are accumulated over time (never removed) and deduplicated by arXiv id.

Last update: 2026-10-30


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
| **[Attention as Lattice Gauge Theory: Relations Interact Only Through Wilson Loops](https://arxiv.org/abs/2610.37656v1)** | 2026-10-27 | <details><summary>Show</summary><p>Relations compose through the entity they share - Alice is Bob's mother and Bob is Carol's father, so Alice is Carol's grandmother - and the order matters, since a father's mother is not a mother's father; verifying a composed relation means closing the loop. We show that if each entity's coordinate frame may be rotated independently (per-entity frame freedom), three things follow. In the pure-gauge sector, relations that share no cycle cannot interact at all. The only gauge-invariant score of a triangle is a class function of its holonomy $H = T_{ij} T_{jk} T_{ki}$ - a Wilson loop. And the only equivariant update of an edge is $U = Ψ(H)\, T_{ij}$ with $Ψ$ conjugation-equivariant. Edge attention by Wilson loops is therefore not one design among many but the unique form the symmetry permits. Three communities hold pieces of this form: the commuting-operator embeddings of knowledge graphs are its abelian (commuting) sector; AlphaFold's triangle update and the Edge Transformer have its shape - an edge updated through the third vertex - without its constraints; and lattice QCD builds it equivariantly on lattices. We instantiate the equivariant sub-family on general relational graphs as holonomy attention. With no training and composition alone, it infers unobserved $S_4$ relations on sparse graphs at 0.88 with a fifth of the edges corrupted, at or slightly below specialist synchronization algorithms, where every commutative architecture is capped at 0.083; its holonomy score flags corrupted triangles at AUC 0.99 where commuting scores are capped at 0.76 by a second selection rule, and it separates clusters without labels.</p></details> | <details><summary>7 pag...</summary><p>7 pages, 1 figure. Accepted at the 9th Workshop on Machine Learning and the Physical Sciences (ML4PS 2026), co-located with NeurIPS 2026</p></details> |
| **[A unified coarse-grained neural network potential for the dynamics of biomolecular complexes](https://arxiv.org/abs/2610.37606v1)** | 2026-10-27 | <details><summary>Show</summary><p>The behavior of biomolecular complexes is governed by chemically specific interactions and often involves rare events that atomistic molecular dynamics struggle to capture within accessible timescales. Here we introduce AMARO v2.0, a coarse-grained neural network potential that retains all heavy atoms and treats solvent implicitly. Hydrogen-aware bead types and total-charge conditioning provide a shared representation for proteins, drug-like molecules, and their complexes, including ternary protein-protein-ligand systems. The model preserves folded proteins and captures key features of protein conformational free-energy landscapes. Across 262 complexes spanning 11 targets, the learned potential retains most ligand poses, although quaternary structure reorientation is observed for the HIF2A ternary complex. In targeted case studies, AMARO v2.0 distinguishes the two protonation states of trypsin-benzamidine and reaches the crystal binding pose in 3.3-fold more trajectories than all-atom molecular mechanics at a fixed estimated GPU-time budget. The same framework also recovers a reference binding pose in TYK2 and supports binding free-energy estimation for both trypsin-benzamidine and TYK2-EJM31, although the resulting values are more energetically favorable than the experimental references. SHP2 and CDK8 systems expose remaining limitations in binding-pose recovery and site specificity, respectively. Together, these results support AMARO v2.0 as a shared heavy-atom potential for biomolecular complex dynamics.</p></details> |  |
| **[Accurate structural modelling of protein-glycan recognition with GlycoWeave](https://arxiv.org/abs/2610.37410v1)** | 2026-10-27 | <details><summary>Show</summary><p>Protein-glycan recognition underlies diverse biological processes, yet accurate prediction of protein-glycan complex structures remains challenging owing to the chemical diversity, conformational flexibility and sparse experimental structural coverage of glycans. Here we present GlycoWeave, a glycan-specific diffusion framework that integrates chemically constrained conformational sampling, multiscale molecular representations and multi-source learning. By operating in internal-coordinate space, GlycoWeave preserves glycan connectivity and stereochemistry while efficiently exploring bound conformations. A heterogeneous equivariant network couples atom-level interaction geometry with monosaccharide-level structural context, whereas multi-source, multi-head training integrates experimental complexes with structures refined using classical and quantum mechanics-informed potentials. On a benchmark of 698 protein-glycan complexes, GlycoWeave achieves a 71.9% Top-25 high-quality success rate, compared with 19.2% for AlphaFold 3, while requiring only 0.34 s per sampled pose. GlycoWeave further preserves glycan structural validity, recovers native protein-glycan interactions and reproduces linkage-specific conformational preferences, maintaining high accuracy across diverse glycan architectures and protein environments. These results establish GlycoWeave as an accurate, efficient and chemically faithful framework for modelling protein-glycan recognition. GlycoWeave is freely available at https://cadd.zju.edu.cn/glycoweave.</p></details> |  |
| **[mdRNAcat: A Molecular Dynamics RNA Catalog of REST2 Conformational Ensembles](https://arxiv.org/abs/2610.35204v1)** | 2026-10-26 | <details><summary>Show</summary><p>Learning molecular models of RNA requires simulation data that capture conformational variability and provide consistent physical training signals. Here, we introduce mdRNAcat, a curated dataset of all-atom molecular dynamics (MD) simulations of 48 RNA systems selected to promote sequence diversity. Each system is simulated using replica-exchange with solute scaling (REST2), with 32 Hamiltonian states and production lengths of 200-300 ns per state. The dataset provides atomic coordinates, instantaneous forces, and forces reevaluated under the unscaled reference Hamiltonian, together with structural annotations and replica-exchange metadata. Coordinates and forces are available at 1 ps intervals for the reference state and 100 ps intervals across all states in a standardized HDF5 format. We characterize conformational sampling, exchange behavior, base pairing, and sugar-pucker distributions to document the properties of the simulated ensembles. mdRNAcat provides a reusable resource for developing and evaluating data-driven RNA models, including coarse-grained force fields.</p></details> | <details><summary>24 pa...</summary><p>24 pages, 9 figures. Dataset and accompanying resources available on Hugging Face under the HelmholtzAI-FZJ organization</p></details> |

Archive: [papers/PSA/](papers/PSA/)


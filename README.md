# AI4Bio Daily ArXiv Papers
The project automatically fetches the latest papers from arXiv based on keywords related to computational biology.

`Each topic below shows only papers from the last 7 days (a recent view)`. The complete archive — including everything shown here — is stored under `papers/`, one folder per topic and one file per month. Papers are not duplicated: the links below are the same entries kept in `papers/`. Click the archive link under each topic to browse the full history.

Papers are accumulated over time (never removed) and deduplicated by arXiv id.

Last update: 2026-09-05


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
| **[An Integrative Computational Approach to Predict Viral Epitopes by Targeting the MHC-TCR Complexation](https://arxiv.org/abs/2609.03182v1)** | 2026-09-02 | <details><summary>Show</summary><p>T-cell immunity acts as a major defense system against controlling viral infections in vertebrates. During viral entry, innate immune cells degrade the viral proteins (antigens) and present them on their surface via Major Histocompatibility (MHC) proteins. T-cell receptors (TCRs) recognize these antigens/peptides presented by MHC (pMHC), initiating a T-cell mediated immune response. Despite its significance, the mechanism by which pMHC-TCR binding triggers T-cell activation remains unclear. In this study, we employed an integrative computational approach combining Bioinformatics, Molecular Dynamics (MD) simulations, and Machine Learning (ML) to identify viral epitopes as potential vaccine candidates. We performed large-scale all-atom and coarse-grained MD simulations on MHC-peptide-TCR complexes embedded into dendritic and T-cells, for which experimental immunogenicity data is available. One hundred fifty such systems are simulated for 1 μs each to capture the conformational and dynamical changes that underlie T-cell activation. Our ML model (DynamiT), trained on simulation-derived structural and dynamical features extracted from 2500 time points, revealed key determinants responsible for T-cell activation with an accuracy of 73.3%. Notably, we have identified the bending of the TCR transmembrane region, major dynamic motions of the TCRα constant region and the buried surface area at the pMHC and TCR interface as critical factors influencing immune response initiation. Our approach unravels the mechanism of T-cell mediated immune response and helps ML-guided screening of viral epitopes for vaccine development.</p></details> |  |
| **[RNA-like Polyelectrolyte in a Viral Capsid: Molecular Dynamics with Explicit Electrostatic Interactions](https://arxiv.org/abs/2608.27825v1)** | 2026-08-28 | <details><summary>Show</summary><p>The organization of RNA genomes within viral capsids is primarily controlled by electrostatic interactions between the negatively charged genome and positively charged N-terminal domains of coat proteins. In theoretical approaches, these interactions are commonly captured by mean-field models that smooth capsid charge over the inner surface and treat ionic screening as a continuum. However, charges are localized at discrete N-terminal binding sites and ionic screening arises from correlated ion distributions. Here we use molecular dynamics simulations with explicit ions, explicit water, and full Coulomb electrostatics to simulate a linear polyelectrolyte confined within a model capsid bearing discrete N-terminal-like charge sites. We first validate our approach by simulating a polyelectrolyte in bulk solution and demonstrating that persistence length decreases with increasing salt, matching experimental measurements for single-stranded RNA. When confined within a capsid, radial density profiles shift systematically inward from the capsid wall with increasing salt concentration, in agreement with mean-field predictions. By independently varying charge magnitude, binding-site density, and N-terminal protrusion length, we show that total electrostatic coupling governs global organization while geometric details modulate local genome-wall contact and angular genome organization near N-terminals (within the T=3 architecture, linear genome topology, and monovalent salt range studied here). Across all simulations, equilibration times increase sevenfold with salt, revealing kinetic effects inaccessible to equilibrium theory. These results validate continuum approximations for radial organization while revealing deviations arising from discrete molecular details and establishing a framework for future investigations of genome secondary structure, capsid geometry, and assembly kinetics.</p></details> |  |
| **[Resolving Spin-Phonon Relaxation Pathways in Molecular Qubits via Regularized Regression](https://arxiv.org/abs/2608.27820v1)** | 2026-08-28 | <details><summary>Show</summary><p>Designing molecular qubits requires controlling the spin-lattice relaxation pathways that fundamentally limit the coherence time. For spin-1/2 molecular qubits, significant discrepancies remain between theoretical predictions and experimental measurements of spin-phonon relaxation pathways, with theory often overestimating the role of low-frequency vibrational modes. Here, we present an alternative first-principles approach augmented with regularized regression that identifies spin-phonon relaxation pathways in an automated fashion without ad hoc mode selection. Applied to Cu porphyrins spin-1/2 molecular qubits, the method successfully reproduces experimental trends in relaxation times and predicts the curvature in the relaxation-vs-temperature profile. The g-tensor time series reveal distinct system-specific autocorrelation functions and spectral-density profiles despite the qubits' structural similarity. Further, regression between g-tensor time series and mode-projected vibrational-amplitude time series obtained from molecular dynamics yields linear and bilinear mode coupling contributions to each g-tensor component. Because the method is based on atomic displacements sampled directly from molecular dynamics, it naturally incorporates anharmonic effects and does not require the harmonic approximation. This framework puts forward a regression-driven, mode-resolved, and coupling-order-separated spin-phonon analysis as a general strategy for predicting and engineering longer-lived molecular qubits.</p></details> |  |

Archive: [papers/PSA/](papers/PSA/)


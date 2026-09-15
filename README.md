# AI4Bio Daily ArXiv Papers
The project automatically fetches the latest papers from arXiv based on keywords related to computational biology.

`Each topic below shows only papers from the last 7 days (a recent view)`. The complete archive — including everything shown here — is stored under `papers/`, one folder per topic and one file per month. Papers are not duplicated: the links below are the same entries kept in `papers/`. Click the archive link under each topic to browse the full history.

Papers are accumulated over time (never removed) and deduplicated by arXiv id.

Last update: 2026-09-16


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
| **[Multi-ligand simultaneous docking of Carica papaya leaf phytochemicals, Carpaine and Rutin, reveals multi-mechanism inhibition of cancer proteins BCL-2 and WWP1](https://arxiv.org/abs/2609.08547v1)** | 2026-09-08 | <details><summary>Show</summary><p>Cancer remains a major global health concern due to chemotherapy resistance and toxicity from high-dose treatments. To overcome these challenges, new therapeutic strategies targeting key proteins in cancer progression are essential. This study evaluates two phytochemicals, Carpaine (Car) and Rutin (Rut), from Carica papaya leaves, for their potential in enhancing cancer therapy by targeting B-cell lymphoma 2 (BCL-2) and WW domain-containing protein 1 (WWP1) proteins. We assessed their additive, allosteric, and synergistic effects using molecular docking, multi-ligand simultaneous docking (MLSD), molecular dynamics (MD) simulations, and MMPBSA analysis. Car and Rut showed an additive effect on BCL-2 by binding at distinct regions within the same pocket. MLSD revealed an improved binding affinity of -13.13 +/- 0.08 kcal/mol, compared with individual ligands or the commercial inhibitor Venetoclax. For WWP1, Car bound near the H-site and Rut near the Le-site, exhibiting an allosteric effect that increased Car's binding affinity in MLSD to -15.59 +/- 0.39 kcal/mol. Furthermore, Rut combined with bortezomib (Bort) demonstrated a synergistic interaction with WWP1. Binding energies were -7.64 +/- 0.156 kcal/mol for Bort, -10.26 +/- 0.07 kcal/mol for Rut, and -15.59 +/- 0.39 kcal/mol for MLSD, suggesting a more stable complex through synergy. These results suggest Car and Rut, particularly in combination with Bort, as promising candidates against cancer-related proteins BCL-2 and WWP1. Further experimental validation is warranted to explore their therapeutic potential.</p></details> | <details><summary>\c{op...</summary><p>\c{opyright} 2025 The Author(s). Published by Elsevier B.V</p></details> |
| **[Predicting directional flexibility in proteins](https://arxiv.org/abs/2609.08474v1)** | 2026-09-08 | <details><summary>Show</summary><p>Predicting protein dynamics is a long-standing problem in computational structural biology. Often, protein function critically depends on local directed motions, such as hinge movements, catalytic loop rearrangements and domain reorientations, which can be characterized by directional flexibility and correlated structural motions of the protein backbone. While Molecular Dynamics (MD) simulations provide an established but often prohibitively expensive approach, recent deep generative models aim to reduce this cost by directly predicting conformational ensembles, emulating MD. However, due to their large size and the need to generate several states until the derived dynamical properties converge, these models remain expensive. In this work, we propose BackFlip-2: a fast SE(3)-equivariant graph neural network trained to directly predict dynamical descriptors, such as directional backbone flexibility and pairwise dynamic correlations, from an equilibrium structure. In a series of experiments, we show that our model matches the accuracy of substantially larger ensemble generation models while being orders of magnitude faster, and demonstrate that the proposed equivariant architecture is especially well-suited for capturing anisotropic motions in proteins. BackFlip-2 model weights, training and inference code are available at https://github.com/graeter-group/backflip.</p></details> |  |

Archive: [papers/PSA/](papers/PSA/)


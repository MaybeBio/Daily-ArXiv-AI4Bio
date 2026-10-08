# AI4Bio Daily ArXiv Papers
The project automatically fetches the latest papers from arXiv based on keywords related to computational biology.

`Each topic below shows only papers from the last 7 days (a recent view)`. The complete archive — including everything shown here — is stored under `papers/`, one folder per topic and one file per month. Papers are not duplicated: the links below are the same entries kept in `papers/`. Click the archive link under each topic to browse the full history.

Papers are accumulated over time (never removed) and deduplicated by arXiv id.

Last update: 2026-10-09


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
| **[Effect of Temperature and Added Salt on a Model Polyzwitterion Polymer in Dilute Solution](https://arxiv.org/abs/2610.04932v1)** | 2026-10-04 | <details><summary>Show</summary><p>The competitive interactions arising from the proximity of positive and negatively charged groups in the monomers in polyzwitterions (PZ) makes these polymers have properties similar in some ways to intrinsically disordered proteins. To gain qualitative insights into this important class of water-soluble polymers, we performed molecular dynamics (MD) simulations of a model PZ chain with an explicit solvent to understand the conformational state in the absence and presence of added salt. We find that isolated PZ chains under salt-free conditions adopt a self-associated state having a weak dependence on temperature. The addition of an appreciable amount of NaCl leads to a weakening of the intrachain associations, resulting in chain expansion, a transition reminiscent of the denaturation of globular proteins. In particular, the hydrodynamic penetration function, the ratio of hydrodynamic radius to the radius of gyration, of the PZ chains under salt free conditions, is found to be more consistent with a randomly branched polymer or single chain nanoparticle than a random coil polymer where the physical cross-links within the chain arise from the dipoles within the chain. The chain conformation not only tends to become larger with the addition of salt but also acquires a more appreciable temperature dependence of its average size with temperature. This swelling trend of PZ molecules with added salt, sometimes referred to as the anti-polyelectrolyte effect, is distinct from the normal trend polyelectrolytes, which typically become more contracted with the addition of salt. We also examined the spatial extent of the dynamic hydration layer the PZ chain, both with and without added salt, and the effect of temperature and salt concentration on the water mobility within this layer, and PZ side-chain mobility, whose dynamics is apparently strongly coupled to the surrounding water molecules.</p></details> | 29 pages, 9 figures |
| **[Generative modeling of intrinsically disordered protein regions by reinforcing sparse autoencoder features](https://arxiv.org/abs/2610.02189v1)** | 2026-10-01 | <details><summary>Show</summary><p>Intrinsically disordered protein regions (IDRs) play central roles in cellular processes such as transcriptional regulation, signal transduction, and subcellular localization, yet their functional design remains challenging. Structure-based design methods do not readily apply to IDRs, and existing protein language models are trained on full-length protein sequences, thus learning a prior that is biased towards folded domains. Here, we present IDiom, an autoregressive protein language model trained on IDiom-DB, a dataset of 54 million predicted IDRs curated from the AlphaFold Database. IDiom generates diverse sequences that recapitulate the composition, patterning, motifs, and predicted disorder of natural IDRs. To control function-associated sequence patterns, we also introduce reinforcement learning with sparse autoencoder features (RL-SAE), a post-training method that rewards the generation of sequences that activate specified feature sets. Across eight IDR design tasks, RL-SAE sequences activate, on average, 90% of 30 targeted features, compared to 24% for activation steering. We demonstrate that RL-SAE improves the predicted subcellular localization and transcriptional activity of generated IDRs compared to steering and supervised fine-tuning, and enables features associated with distinct biological functions to be combined within individual sequences. Thus, IDiom and RL-SAE enable interpretable and composable IDR design through explicit control of function-associated sequence features. More broadly, RL-SAE could extend to other protein design settings where interpretable features provide useful design targets. Code is available at https://github.com/rotskoff-group/idiom.</p></details> |  |

Archive: [papers/IDR/](papers/IDR/)

## Protein-DNA Modeling & Simulation (PDA)

No new papers in the last 7 days.

Archive: [papers/PDA/](papers/PDA/)

## Protein Structure Deep Learning (PSA)

| **Title** | **Date** | **Abstract** | **Comment** |
| --- | --- | --- | --- |
| **[A Shortcut to Structure in AlphaFold 3](https://arxiv.org/abs/2610.08937v1)** | 2026-10-06 | <details><summary>Show</summary><p>AlphaFold 3 predicts protein structures with remarkable accuracy, yet how structural information emerges within the model remains poorly understood. Here, through causal interventions on internal representations and direct probing of every Pairformer block, we trace the formation of global protein geometry and identify the multiple sequence alignment (MSA) as a structural shortcut to the fold. Removing the MSA largely preserves local secondary structure while disrupting the long-range relationships that define global topology. Restoring the MSA-enriched pair representation at only forty residues recovers most of this lost organization, including at pairs never directly modified. This contribution depends on the detailed direction of the MSA module's output rather than its magnitude. The Pairformer rapidly converts this signal into global geometry: the final fold becomes recoverable by approximately block 9 of 48 for a majority of proteins, roughly twenty-seven blocks before the model's decoder can render it, whereas without the MSA it remains inaccessible for most proteins throughout the pass. Which homologs are supplied shapes this trajectory more strongly than which query is supplied; it persists for a designed query that never evolved but collapses for a shuffled sequence. Most importantly, an alignment built for a different protein that shares the fold, supplied only at the structurally corresponding columns, raises the median TM-score against experiment from 0.44 to 0.72, while the same alignment shifted a few residues along the chain performs worse than supplying no alignment at all. What AlphaFold 3 reads from an alignment is therefore a description of the fold itself, transferable between proteins that share one, rather than the query's own evolutionary history. This explains both its accuracy and the limits of what it has solved.</p></details> |  |
| **[Multi-Scale Temporal Flows for Peptide Trajectory Generation](https://arxiv.org/abs/2610.01086v1)** | 2026-10-01 | <details><summary>Show</summary><p>Peptides occupy a particularly challenging regime of biomolecular dynamics. Short peptides lack a stable folded core and populate broad conformational ensembles, while cyclization adds ring closure, non-local residue coupling, and stereochemical diversity. Deep generative models have made remarkable progress in emulating molecular-dynamics trajectories directly, yet each is trained on windows cut at a fixed interval and therefore observes the process at a fixed temporal resolution. More fundamentally, none takes that interval as an input, so the physical time a window spans is never represented, leaving the sparse frames on which a peptide crosses between metastable states difficult to learn. Here, we introduce PepTIDE, a multi-scale temporal framework for peptide trajectory generation. The stride of each training window is drawn from a continuous range, so one model observes the same dynamics at many temporal resolutions, and an Adaptive Physical-Time Embedding encodes the relative interval of a window together with the absolute time of each frame, making the shared velocity field interval-aware. All frames are generated jointly through a stochastic-interpolant flow, and pair-aware invariant point attention captures the geometry and topology of both linear and cyclic peptides. On PepMD and a 50-system cyclic-peptide benchmark, PepTIDE reaches state-of-the-art distribution agreement and structural validity. Read in temporal order, its trajectories recover these sparse transition frames and reproduce inter-state fluxes more faithfully, confirming that modeling multiple temporal scales is what makes these rare events accessible.</p></details> |  |

Archive: [papers/PSA/](papers/PSA/)


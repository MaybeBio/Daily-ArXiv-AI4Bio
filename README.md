# AI4Bio Daily ArXiv Papers
The project automatically fetches the latest papers from arXiv based on keywords related to computational biology.

`Each topic below shows only papers from the last 7 days (a recent view)`. The complete archive — including everything shown here — is stored under `papers/`, one folder per topic and one file per month. Papers are not duplicated: the links below are the same entries kept in `papers/`. Click the archive link under each topic to browse the full history.

Papers are accumulated over time (never removed) and deduplicated by arXiv id.

Last update: 2026-10-11


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

Archive: [papers/IDR/](papers/IDR/)

## Protein-DNA Modeling & Simulation (PDA)

No new papers in the last 7 days.

Archive: [papers/PDA/](papers/PDA/)

## Protein Structure Deep Learning (PSA)

| **Title** | **Date** | **Abstract** | **Comment** |
| --- | --- | --- | --- |
| **[Three-dimensional imaging of isolated membrane-protein complexes in vacuo with an X-ray laser](https://arxiv.org/abs/2610.11729v1)** | 2026-10-08 | <details><summary>Show</summary><p>The prospect of imaging single biomolecules, viruses and cells with intense, ultrashort X-ray pulses has driven the development of X-ray free-electron lasers (XFELs). However, the weak scattering from small particles is easily swamped by background from residual gas, which has so far limited applications to strongly scattering targets such as viruses, cell organelles and cells. Here we report a three-dimensional (3D) reconstruction of an isolated 1-MDa membrane-protein complex, photosystem I (PS I), from single-particle diffraction data. PS I trimers were aerosolised by charge-reduction electrospray ionisation and injected into the European XFEL beam, with partial helium gas exchange reducing background scattering by 80%. From 32 788 diffraction patterns of single trimers in random orientations, we reconstructed the 3D electron density to a resolution of 3.8 nm, limited by the detector geometry. The disc-shaped density, about 22 nm across and 10 nm thick, matches the size of a PS I trimer in a detergent micelle and is consistent with the compaction predicted by molecular dynamics simulations of the complex in vacuo and observed in native mass spectrometry. These results show that membrane-protein complexes can be imaged in vacuo with X-ray lasers, an important step towards ultrafast diffractive imaging of single macromolecules.</p></details> |  |
| **[MD-LLM-2: A Transferable Language Model of Molecular Dynamics with Physical Conditioning and Explicit Path Probabilities](https://arxiv.org/abs/2610.10879v1)** | 2026-10-07 | <details><summary>Show</summary><p>Molecular dynamics (MD) simulations model the motion of proteins between conformational states, but crossing free energy barriers and sampling multiple thermodynamic conditions remain computationally costly. We recently introduced MD-LLM-1, which showed that language models can generate conformational trajectories at lower cost, but required a separate model for each protein and did not explicitly model thermodynamics or kinetics. Here we introduce MD-LLM-2, a transferable language model that generates trajectories conditioned on sequence, temperature and molecular history. Because each step defines a normalized distribution over structural tokens, the model assigns an explicit likelihood to every generated or simulated trajectory. Trained across mdCATH domains, MD-LLM-2 reproduces the median radius of gyration of MD within 1 Angstrom in 10 of 12 unseen domains, predicts reduced Trp-cage compaction at higher temperature, and generates L99A T4 lysozyme trajectories that reach published transition-region backbone structures. In alanine dipeptide simulations, conditioning on a torsional scaling parameter $λ$ predicts basin populations at unseen couplings with a mean absolute error of 0.09 versus 0.35 for MBAR, and first-passage probabilities with an error of 0.08 versus 0.16 for a reversible Markov state model. Frame-isoentropic sampling further limits the accumulation of errors during autoregressive trajectory generation. Together, these results extend MD-LLM from protein-specific trajectory generation to transferable, physically conditioned modelling with explicit path likelihoods, and show that the framework can predict equilibrium populations for force-field parameters not seen during training, with an initial indication that first-passage kinetics can also be captured.</p></details> |  |
| **[A Shortcut to Structure in AlphaFold 3](https://arxiv.org/abs/2610.08937v1)** | 2026-10-06 | <details><summary>Show</summary><p>AlphaFold 3 predicts protein structures with remarkable accuracy, yet how structural information emerges within the model remains poorly understood. Here, through causal interventions on internal representations and direct probing of every Pairformer block, we trace the formation of global protein geometry and identify the multiple sequence alignment (MSA) as a structural shortcut to the fold. Removing the MSA largely preserves local secondary structure while disrupting the long-range relationships that define global topology. Restoring the MSA-enriched pair representation at only forty residues recovers most of this lost organization, including at pairs never directly modified. This contribution depends on the detailed direction of the MSA module's output rather than its magnitude. The Pairformer rapidly converts this signal into global geometry: the final fold becomes recoverable by approximately block 9 of 48 for a majority of proteins, roughly twenty-seven blocks before the model's decoder can render it, whereas without the MSA it remains inaccessible for most proteins throughout the pass. Which homologs are supplied shapes this trajectory more strongly than which query is supplied; it persists for a designed query that never evolved but collapses for a shuffled sequence. Most importantly, an alignment built for a different protein that shares the fold, supplied only at the structurally corresponding columns, raises the median TM-score against experiment from 0.44 to 0.72, while the same alignment shifted a few residues along the chain performs worse than supplying no alignment at all. What AlphaFold 3 reads from an alignment is therefore a description of the fold itself, transferable between proteins that share one, rather than the query's own evolutionary history. This explains both its accuracy and the limits of what it has solved.</p></details> |  |

Archive: [papers/PSA/](papers/PSA/)


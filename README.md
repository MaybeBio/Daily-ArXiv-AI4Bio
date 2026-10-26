# AI4Bio Daily ArXiv Papers
The project automatically fetches the latest papers from arXiv based on keywords related to computational biology.

`Each topic below shows only papers from the last 7 days (a recent view)`. The complete archive — including everything shown here — is stored under `papers/`, one folder per topic and one file per month. Papers are not duplicated: the links below are the same entries kept in `papers/`. Click the archive link under each topic to browse the full history.

Papers are accumulated over time (never removed) and deduplicated by arXiv id.

Last update: 2026-10-27


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
| **[Emergent Entropic Forces Drive Inverse and Reentrant Phase Transitions in Condensates of Intrinsically Disordered Proteins](https://arxiv.org/abs/2610.30627v1)** | 2026-10-22 | <details><summary>Show</summary><p>We present a phenomenological, mean-field model for condensates of intrinsically disordered proteins that describes inverse phase transitions and qualitatively predicts reentrant phase behavior as a function of salt concentration. The model is based on a matrix-based formulation of the Flory-Huggins free energy, in which the enthalpic interaction parameter and the protein valence, defined here as the number of effective "sticky patches", are treated as free parameters. Its central insight is that integrating out dynamics of fast-moving molecular species generates an effective entropic force that increases the free-energy barrier to mixing, even within a mean-field description. We account for this by linking Gaussian integration of co-solutes to the Schur complement of the matrix-based Flory-Huggins free energy. This provides a general thermodynamic framework illustrating how enthalpic interactions that increase the number of available microstates necessarily induce effective entropic forces. We demonstrate the expressiveness and predictive power of the model by qualitatively reproducing recent experimental observations on the rabies virus phosphoprotein.</p></details> | <details><summary>20 pa...</summary><p>20 pages. 7 Figures. Comments welcome!</p></details> |

Archive: [papers/IDR/](papers/IDR/)

## Protein-DNA Modeling & Simulation (PDA)

No new papers in the last 7 days.

Archive: [papers/PDA/](papers/PDA/)

## Protein Structure Deep Learning (PSA)

| **Title** | **Date** | **Abstract** | **Comment** |
| --- | --- | --- | --- |
| **[Ensemble-Aware Structural Encoding (EASE): Conditioning Protein Encoders on Peptide Conformational Ensembles](https://arxiv.org/abs/2610.27638v1)** | 2026-10-20 | <details><summary>Show</summary><p>Protein foundation models provide transferable representations for downstream peptide prediction tasks. However, existing representations typically reduce a peptide to a single sequence or structure, which may miss conformational variability relevant to key peptide properties, including antibacterial activity, hemolysis, toxicity, stability, and binding. For example, protease resistance correlates more strongly with conformational dynamics measured by hydrogen exchange than with average helicity. Therefore, we introduce Ensemble-Aware Structural Encoding (EASE), a framework for effectively extracting structural information from conformational ensembles for peptide representation. To extract useful information from noisy conformers, EASE selects central conformers representing a peptide's major structural states and fuses their individual representations with a permutation-invariant operator to produce a peptide-level representation for downstream prediction. We then evaluate our framework on six peptide property-prediction tasks under leakage-controlled splits. Against matched single-structure baselines, EASE improves performance consistently on six tasks with a mean absolute gain of about 3.0% across two structural encoders. Gains keep growing as we add conformers through K=20. A single peptide conformer therefore provides a limited basis for structural representation, whereas our framework distilling and fusing multiple conformers yields a more informative representation.</p></details> |  |
| **[ProtGlycanDock: Towards Accurate Protein-Glycan Docking with Tailored Dataset, Benchmark and Model](https://arxiv.org/abs/2610.26009v1)** | 2026-10-19 | <details><summary>Show</summary><p>Performing accurate protein-glycan docking is critical to understanding protein-glycan interactions which govern many biological processes. However, this important task is hampered by the lack of tailored datasets, benchmarks and models for protein-glycan docking. To fill this blank, we first curate a standard benchmark ProtGlycanDock for training and evaluating protein-glycan docking models under both protein and glycan generalization settings. On this benchmark, we evaluate ten models in three categories, physics-based docking methods, machine-learning-based docking models and molecular structure prediction models. To obtain more precise binding poses, we further propose two finetuning techniques to inject the knowledge of glycan conformations into a general-purpose molecular structure prediction model. These two techniques respectively augment model inputs with glycan topological features and refine glycan binding pose with a glycan energy loss. Benchmark results show the superiority of AlphaFold 3 among existing methods, and the two proposed finetuning techniques can be well combined to achieve a state-of-the-art model for protein-glycan docking. Also, we perform stratified benchmark analysis and case studies to better understand the strengths and weaknesses of current models, providing insights for future model improvements. We maintain datasets at https://huggingface.co/datasets/ProtGlycanDock/ProtGlycanDock and source codes at https://github.com/kasawa1234/ProtGlycanDock</p></details> | <details><summary>Accep...</summary><p>Accepted by NeurIPS 2026 Evaluations and Datasets Track. Datasets and source codes are released</p></details> |
| **[Stronger artificial intelligence breakthroughs hasten their own exhaustion](https://arxiv.org/abs/2610.27296v1)** | 2026-10-19 | <details><summary>Show</summary><p>Progress in artificial intelligence is widely assumed to scale with effort: more researchers, papers and investment should accelerate discovery. Theories of technological growth instead locate the difficulty of discovery in the space of ideas. Here we show that neither scale nor space is enough: breakthroughs depend on diverse attention, which collective concentration can deplete. Across 36 years of computer science, we analyze 7.2 million papers, 73,089 peer reviews and 3.7 million researchers and their topic shifts. The field expanded while its attention narrowed sharply after the Transformer. Over half of topic-shifting researchers moved into AI, especially mid-career ones, and reviewer confidence fell by a full point on a 5-point scale. Each successive breakthrough, from AlexNet to large language models, raised the field's carrying capacity for ideas but was followed by steeper exhaustion of those ideas. Bigger breakthroughs capture attention more completely, depleting the diversity their successors may draw upon. Structural biology shows the same cycle after cryo-EM and AlphaFold. Simulations show how well-intentioned and widely used policies such as reciprocal reviewing empower prolific authors and further narrow what the field accepts. We call for institutions that protect diverse attention in artificial intelligence rather than reward concentration on the winning paradigm.</p></details> |  |
| **[Magnolia: A Persistent-Memory Agent Framework for Computational Chemistry](https://arxiv.org/abs/2610.27230v1)** | 2026-10-19 | <details><summary>Show</summary><p>Chemistry has recently entered a high-data regime as molecular databases from high-throughput platforms or computational studies have become available. Increasing automation within the chemical sciences leads to a more digital and precision chemistry. Dedicated scientific agents are becoming central to guiding the chemist through an ever-increasing amount of data and findings, including negative ones. Here, we introduce Magnolia, a persistent-memory artificial intelligence agent framework that integrates computational protocols, from docking to quantum chemistry, lab notebooks and chat logs relying on large language models (LLMs). It relies on a three-tier memory system: session-level observations are automatically captured and distilled into structured learnings, confirmed and elevated to project-tier entries and, when human-validated, promoted to cross-project rules that actively guide subsequent work and provide direct chemical feedback. We illustrate Magnolia on four case studies: quantum-chemical evaluation of aromatic systems (COMPAS database), molecular dynamics of butane and of modified DNA, and a protein-peptide docking campaign. Across these projects, Magnolia tracked 317 runs and accumulated 116 project-tier entries, from which four cross-project rules were promoted; in controlled replays of four tasks, runs with memory passed the checks that runs without it failed (for example, ten of ten docking-configuration checks, against one to four of ten). By combining automation, reproducibility, and human-in-the-loop control, our Magnolia framework streamlines docking, molecular dynamics and quantum chemistry calculations with direct analysis and LLM-augmented feedback, offering accelerated access to computational (bio)chemistry.</p></details> | <details><summary>https...</summary><p>https://github.com/HolobiomicsLab/Magnolia-AI</p></details> |

Archive: [papers/PSA/](papers/PSA/)


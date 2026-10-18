# AI4Bio Daily ArXiv Papers
The project automatically fetches the latest papers from arXiv based on keywords related to computational biology.

`Each topic below shows only papers from the last 7 days (a recent view)`. The complete archive — including everything shown here — is stored under `papers/`, one folder per topic and one file per month. Papers are not duplicated: the links below are the same entries kept in `papers/`. Click the archive link under each topic to browse the full history.

Papers are accumulated over time (never removed) and deduplicated by arXiv id.

Last update: 2026-10-19


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
| **[Calibrating AlphaFold confidence scores for interface quality](https://arxiv.org/abs/2610.17108v1)** | 2026-10-12 | <details><summary>Show</summary><p>AlphaFold confidence scores are widely used to rank protein complex predictions and to select subsets of models for downstream applications. Although these scores provide strong discriminatory power for distinguishing prediction quality, their numerical values were never intended to represent the probability that a prediction satisfies a given structural quality criterion. In this work, we calibrate commonly used confidence scores to estimate the probability that a predicted complex exceeds a chosen threshold of DockQ, an established measure of interface quality. On antibody-antigen and general multimer datasets, post-hoc isotonic calibration consistently improves agreement between predicted probabilities and observed DockQ success rates while preserving the underlying score ordering. The calibrated probabilities also provide more accurate estimates of the fraction of selected models expected to pass a given structural quality threshold. Although the mapping is fitted within a given prediction distribution and therefore transfers imperfectly across prediction domains, we show that reliable estimates are recovered from a small number of labeled target-domain samples. Because the calibration is entirely post hoc and requires no underlying AlphaFold model fine-tuning, it provides a straightforward and customizable way to convert existing model quality rankings into calibrated probabilities of passing a chosen structural quality threshold.</p></details> |  |

Archive: [papers/PSA/](papers/PSA/)


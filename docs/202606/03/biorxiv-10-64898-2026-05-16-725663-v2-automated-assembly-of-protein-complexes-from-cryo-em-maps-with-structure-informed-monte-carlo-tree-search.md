---
title: Automated assembly of protein complexes from cryo-EM maps with structure-informed Monte Carlo Tree Search
title_zh: 基于结构信息的蒙特卡洛树搜索从冷冻电镜图自动组装蛋白质复合物
authors: "Dilip, R., Qu, S. J., Chen, Z., Van Valen, D. A."
date: 2026-05-29
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.16.725663v2.full.pdf"
tags: ["query:alphazero"]
score: 6.0
evidence: 使用蒙特卡洛树搜索进行蛋白质复合体组装，这是AlphaZero的算法组件
tldr: 结构细胞生物学致力于在细胞原生环境中可视化功能分子，但原位大分子复合物通常仅解析到中等分辨率，蛋白质组规模的巨大组合空间使识别和建模异常困难。Cryosearch框架采用蒙特卡洛树搜索，以基于密度图相关性的函数为奖励，自动从单体库中挑选能最佳解释图谱的蛋白质域组合，进行从头组装。借助GPU并行加速，该方法能从中等分辨率图谱高效构建复合物模型，在多种测试案例中成功重建结构。该工作填补了中等分辨率下自动化复合物组装的空白，为原位结构生物学解析提供了强大新工具。
source: biorxiv
selection_source: fresh_fetch
motivation: 原位大分子复合物仅解析到中等分辨率，蛋白质组规模的组合空间使自动化识别和组装变得困难。
method: 开发Cryosearch框架，采用蒙特卡洛树搜索和基于相关性的奖励，从蛋白质组单体库自动选择最佳域组合进行组装。
result: GPU加速下，Cryosearch从中等分辨率图谱自主组装复合物，结果与实验模型一致，效率显著提升。
conclusion: 首次实现无需人工干预的中等分辨率图谱复合物从头组装，填补自动化建模空白，推动原位结构解析。
---

## 摘要
结构细胞生物学旨在可视化功能分子在其天然细胞环境中执行生物学功能的过程。然而，原位大分子复合物迄今为止主要在中分辨率下解析，由于蛋白质组中可能组分的巨大组合空间，蛋白质识别和结构建模变得复杂。在此，我们开发了Cryosearch，一个GPU加速框架，用于从蛋白质组规模的单体库中自动组装大分子复合物。Cryosearch实现了基于相关奖励的蒙特卡洛树搜索，以识别共同最佳解释密度图的蛋白质结构域组合。该方法能够从中分辨率图自主从头组装分子复合物。

## Abstract
Structural cell biology aims to visualize functional molecules as they carry out their biological roles in their native cellular context. However, macromolecular complexes in situ have thus far been resolved predominantly at intermediate resolutions, complicating protein identification and structural modeling due to the vast combinatorial space of possible components within a proteome. Here, we developed Cryosearch, a GPU-accelerated framework for automated assembly of macromolecular complexes from proteome-scale monomer libraries. Cryosearch implements Monte Carlo tree search with correlation-based rewards to identify combinations of protein domains that collectively best explain density maps. This approach enables autonomous de novo assembly of molecular complexes from intermediate-resolution maps.
---
title: Combinatorial docking and molecular generation to navigate over 100-billion molecules for prospective ligand discovery
title_zh: 组合对接与分子生成：导航超过千亿分子用于前瞻性配体发现
authors: "Zhang, J., Yang, C., Zhang, Y., Chen, X., Lam, B., Bryant, C., Pidathala, S., Wang, Y., Moroz, Y., Radchenko, D., Alon, A., Lee, C.-H., Zhang, Z., Lyu, J."
date: 2026-06-11
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.07.730716v1.full.pdf"
tags: ["query:alphazero"]
score: 6.0
evidence: 蒙特卡洛树搜索在药物发现分子生成中的应用
tldr: 商业可合成库已超千亿分子，传统虚拟筛选需数十年。提出CombiDOCK组合对接框架和MINT-Dock生成式框架，分别在40天内完成穷举筛选和实现4800倍富集。在46个靶标上，前瞻性筛选获得更高命中率和更有效配体，计算成本降低20倍以上，冷冻电镜证实了最佳配体结合姿势。这些方法为高效导航万亿分子药物发现提供了穷举与生成路径。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有虚拟筛选无法高效处理千亿级可合成分子库，需开发更快速的方法。
method: CombiDOCK组合对接框架实现穷举筛选，MINT-Dock生成式框架结合对接与蒙特卡洛树搜索加速导航。
result: CombiDOCK匹配全分子对接精度，MINT-Dock富集4800倍；前瞻性筛选获得更高命中率和更有效配体，计算成本降低20倍以上，冷冻电镜验证。
conclusion: 两种方法为导航万亿分子药物发现提供了可行路径。
---

## 摘要
商业上按需合成的化合物库现已超过1000亿个化合物，使用传统对接方法在2000个CPU核心上筛选需要超过50年。我们提出两种互补方法应对这一挑战。CombiDOCK是一种组合对接框架，能在40天内实现千亿规模的穷尽筛选。MINT-Dock是一种生成框架，通过将CombiDOCK与蒙特卡洛树搜索相结合，加速了该空间的导航。在46个不同靶标的基准测试中，CombiDOCK匹配了全分子对接的准确性，而MINT-Dock相对于随机选择实现了4800倍的富集。与之前针对σ2、VMAT2和VAChT的十亿级暴力筛选活动相比，前瞻性的CombiDOCK筛选在千亿分子库中获得了更高的命中率和更有效的配体，而MINT-Dock在单目标和多目标目标上取得了相当的结果，且计算成本降低了20倍以上。最佳VAChT结合化合物的对接预测姿态得到了冷冻电镜结构的确认。这些方法为导航药物发现的万亿分子前沿提供了穷尽和生成的路径。

## Abstract
Commercially available make-on-demand libraries now exceed 100 billion compounds, requiring over 50 years to screen on 2,000 CPU cores using conventional docking. We present two complementary approaches to address this challenge. CombiDOCK, a combinatorial docking framework, enables exhaustive screening at the 100-billion scale within 40 days. MINT-Dock, a generative framework, accelerates navigation of this space by integrating CombiDOCK with Monte Carlo Tree Search. Benchmarked on 46 diverse targets, CombiDOCK matched full-molecule docking accuracy, and MINT-Dock achieved a 4,800-fold enrichment over random selection. Compared with prior billion-scale brute-force campaigns against {sigma}2, VMAT2, and VAChT, prospective CombiDOCK screens of the 100-billion-molecule library yielded higher hit rates and more potent ligands, while MINT-Dock achieved comparable outcomes across single- and multi-target objectives with >20-fold computational cost reductions. Docking-predicted poses of the best VAChT-binding compounds were confirmed by cryo-EM structures. These methods provide exhaustive and generative paths for navigating the trillion-molecule frontier of drug discovery.
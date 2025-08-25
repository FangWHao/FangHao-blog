---
title: 2025.08 文献阅读记录
published: 2025-08-25
pinned: false
description: 总结一下文献的内容和好思路
tags: [Markdown, Blogging, Mermaid]
category: Examples
draft: false
---
# Single-cell RNA-seq highlights intra-tumoral heterogeneity  and malignant progression in pancreatic ductal  

> 样本：24例胰腺导管腺癌（PDAC）肿瘤和11个对照胰腺的共57,530个细胞进行了深入的转录组分析。

> 鉴定出了多种不同的恶性细胞和基质细胞亚群，发现存在两种基因表达谱截然不同的导管细胞：一种是基因表达异常的“1型导管细胞”，另一种是恶性的“2 型导管细胞” 。通过**拷贝数变异（CNV）分析证实**，2型导管细胞是主要的恶性细胞来源，在肿瘤组织中显著增多，而在正常组织中则未被发现 。进一步的分析揭示，恶性的 2 型导管细胞内部还包含多个具有不同增殖和迁移潜能的亚群。通过构建细胞演进轨迹，该研究描绘了导管细胞从异常状态向恶性状态转变的过程，并**识别出在此过程中多个关键肿瘤相关通路（如ErbB和Notch信号通路）的动态激活** 。一项重要的发现是，**一个具有高度增殖特征的恶性导管细胞亚群的存在与肿瘤浸润T细胞的失活状态密切相关**，这表明肿瘤细胞自身的转录状态可以影响免疫微环境，从而导致不良预后。


![](Aug-paper/2025-08-25-14-47-08.png)
Subgroup 3 cells are the major population present in most patients, suggesting that this subgroup is shared among PDAC patients. In contrast, subgroups 1, 2, 4, 5 and 6 are exclusively observed in some patients, which reflects the tumor heterogeneity of individual patient. 

- 树状图：上方为亚群之间的相似性，左侧为不同病人样本之间的相似性。
- 可视化：pheatmap/ComplexHeatmap
- 思路：查看不同 cluster 之间的分布
  - 分布都比较多 → 共享特征
  - 部分病人很高 → 个体差异大，肿瘤异质性
  - 稀有但广泛存在

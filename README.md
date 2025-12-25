# Medical Vision Foundation Models (MVFMs): A Comprehensive Review

[![GitHub Stars](https://img.shields.io/github/stars/ice-TuoShui/MVFM-Review?style=social)](https://github.com/ice-TuoShui/MVFM-Review) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> **📚 综述 | 代码资源 | 持续更新**  
> 本项目旨在系统梳理医学视觉基础模型的技术演进与临床转化，并配套维护一个高质量的开源方法及代码链接索引。

---

## 📖 概述
本文是一篇关于**医学视觉基础模型**的系统性综述论文。文章系统分析了从2019至2025年间该领域的137项核心研究，探讨了MVFMs的技术生命周期、数据基础设施，并从技术可靠性、临床整合与监管合规性等多个维度，深入剖析了其从实验室能力到临床现实所面临的“可信鸿沟”。

**核心贡献：**
1.  **系统性宏观分析**：绘制了该领域从探索、爆发到深化的三阶段发展轨迹。
2.  **双维技术框架**：提出了统一的分析框架，涵盖“预训练范式”与“下游任务适应策略”。
3.  **数据约束分析**：深入阐述了医学数据生态如何作为根本性约束塑造技术发展路径。
4.  **临床可信鸿沟诊断**：首次系统剖析了阻碍临床转化的多维度障碍。
5.  **未来路径前瞻**：提出了迈向“可信通用医学视觉智能”的四大演进路径。

## 🗂️ 资源索引：医学视觉基础模型方法与代码
这是本项目的核心价值之一。我们持续收集、筛选并整理了数十个高质量的医学视觉基础模型（VFM）开源实现、预训练权重及官方代码库链接。

**索引原则**：收录的项目均在论文中有所提及或评估，确保与综述内容强相关，并优先选择维护活跃、复现性好的资源。

| 模型/框架名称 | 核心论文/出处 | 官方/推荐代码链接 | 预训练权重 | 备注 (特点/任务) |
| :--- | :--- | :--- | :--- | :--- |
| **ViS-MAE** | *An Efficient Self-supervised Learning Approach...* | [GitHub Link](https://github.com/xxx) | Available | 多模态（CT, MRI, X-ray等）生成式预训练 |
| **CTransPath** | *A foundation model for clinical-grade...* | [GitHub Link](https://github.com/xxx) | Available | 病理学基础模型，3亿patch预训练 |
| **UNETR** | *Transformers for 3D Medical Image Segmentation* | [GitHub Link](https://github.com/xxx) | Available | 基于Transformer的3D医学图像分割 |
| **MedSAM** | *Segment anything in medical images* | [GitHub Link](https://github.com/xxx) | Available | 医学图像分割通用适配模型 |
| **STU-Net** | *Scalable and Transferable Medical Image...* | [GitHub Link](https://github.com/xxx) | Available | 大规模有监督预训练的分割模型 |
| **UniverSeg** | *Universal Medical Image Segmentation* | [GitHub Link](https://github.com/xxx) | Available | 基于上下文的通用医学图像分割 |
| **[其他模型名]** | *[对应论文]* | [GitHub Link]() | - | *[补充说明]* |
*（请用你收集的实际信息填充此表格，此表格可随收藏增加而扩展）*

## 📄 论文内容
- **最新版手稿**：[`MVFM-Review_Manuscript.pdf`](MVFM-Review_Manuscript.pdf) - 你可以直接下载阅读。
- **预印本**：[arXiv:xxxx.xxxxx](https://arxiv.org/abs/xxxx.xxxxx) *（投稿后可补充链接）*
- **引用信息**（BibTeX）:
```bibtex
@article{lin2025medical,
  title={Medical Vision Foundation Models: A Comprehensive Review from Technical Evolution to Clinical Translation},
  author={Lin, Nengjian},
  journal={IEEE Transactions on Medical Imaging (Under Review)},
  year={2025}
}

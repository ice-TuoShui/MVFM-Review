## Medical Vision Foundation Models: Method Summary Tables

This repository contains structured summary tables of key methods in **Medical Vision Foundation Models (MVFMs)**, based on the comprehensive review paper *"Medical Vision Foundation Models: A Comprehensive Review from Technical Evolution to Clinical Translation"* (under review).

The following four tables categorize and summarize state-of-the-art approaches in medical vision foundation models, grouped by their core learning paradigms and adaptation strategies.

---

## 📊 Table 1: Summary of Generative Learning Approaches

| Methods         | Research Questions | Pre-training | Adaptation | Backbone         | Modalities          | Downstream | Year | Code                                                     |
| --------------- | ------------------ | ------------ | ---------- | ---------------- | ------------------- | ---------- | ---- | -------------------------------------------------------- |
| Virchow         | FSL, DG, Interp.   | GL           | PEFT       | ViT              | Path.               | CLS        | 2024 |                                                          |
| DINOv2          | FSL, DG            | GL           | PEFT       | ViT              | X-ray, CT, MRI      | CLS, SEG   | 2023 | [GitHub](https://github.com/facebookresearch/dinov2)     |
| M4oE            | DG                 | GL           | FT         | SwinUNet         | CT, MRI             | SEG        | 2024 | [GitHub](https://github.com/csyfjiang/M4oE)              |
| FedFMS          | DG                 | GL           | FT, PEFT   | ViT              | MRI, Path., Fundus  | SEG        | 2024 | [GitHub](https://github.com/LIU-YUXI/FedFMS)             |
| MAISI           | FSL                | GL           | FT         | VAE-GAN, U-Net   | CT, MRI             | SEG        | 2025 | [GitHub](https://github.com/Ziwei-Niu/Maisi_Var)         |
| GL-MAE          | DG                 | GL           | FT         | ViT              | CT, MRI             | SEG, CLS   | 2025 | [GitHub](https://github.com/JiaxinZhuang/GL-MAE)         |
| SSFedMRI        | FSL, DG            | GL           | FT         | MoDL             | MRI                 | REC        | 2023 |                                                          |
| MRM             | FSL                | GL           | FT         | ViT-B, SNN       | Fundus, Gen., Path. | CLS, SEG   | 2024 | [GitHub](https://github.com/CityU-AIM-Group/MRM)         |
| EAGLE           | DG                 | GL           | FT         | ViT-g            | Path.               | CLS        | 2025 | [GitHub](https://github.com/chadvanderbilt/EAGLE)        |
| Static DiMo     | Recon.             | GL           | -          | U-Net            | MRI                 | REC        | 2025 |                                                          |
| Uni4Eye++       | FSL, DG, Cont.     | GL           | FT         | ViT              | Multimodal images   | CLS, SEG   | 2024 | [GitHub](https://github.com/Davidczy/Uni4Eye_pp)         |
| USFM            | FSL, DG            | GL           | FT, PE     | Transformer      | US                  | Multi-task | 2024 |                                                          |
| DeblurringMIM   | DG                 | GL           | FT         | ViT (MAE)        | US                  | CLS        | 2023 | [GitHub](https://github.com/MembrAI/DeblurringMIM)       |
| GVSL            | FSL, DG            | GL           | FT         | 3D U-Net         | CT, MRI             | SEG, CLS   | 2023 | [GitHub](https://github.com/YutingHe-list/GVSL)          |
| MIS-FM          | FSL, DG            | GL           | FT         | PCT-Net          | CT                  | SEG        | 2023 | [GitHub](https://github.com/openmedlab/MIS-FM)           |
| RETFound        | FSL, Interp.       | GL           | FT         | ViT-large (MAE)  | CFP, OCT            | CLS        | 2023 | [GitHub](https://github.com/rmaphoh/RETFound)            |
| ModelsGenesis   | SSL                | GL           | FT         | U-Net, ResNet    | Multimodal images   | SEG, CLS   | 2019 | [GitHub](https://github.com/MrGiovanni/ModelsGenesis)    |
| SelfMedMAE      | FSL, DG            | GL           | FT         | ViT (MAE)        | X-ray, CT, MRI      | CLS, SEG   | 2022 | [GitHub](https://github.com/cvlab-stonybrook/SelfMedMAE) |
| VIS-MAE         | DG, Label Eff.     | GL           | FT         | Swin Transformer | Multimodal images   | SEG, CLS   | 2025 | [GitHub](https://github.com/lzl199704/VIS-MAE)           |
| Swin-UMamba†    | FSL                | GL           | FT         | Mamba            | MRI, Endo., Micro.  | SEG        | 2025 | [GitHub](https://github.com/JiarunLiu/Swin-UMamba)       |
| DenseFormer-MoE | DG                 | GL           | FT         | DenseNet, ViT    | sMRI                | CLS, REG   | 2025 |                                                          |

---

## 📊 Table 2: Summary of Contrastive Learning Approaches

| Methods                     | Research Questions | Pre-training | Adaptation | Backbone         | Modalities        | Downstream | Year | Code                                                                                      |
| --------------------------- | ------------------ | ------------ | ---------- | ---------------- | ----------------- | ---------- | ---- | ----------------------------------------------------------------------------------------- |
| BrainIAC                    | FSL, DG            | CL           | FT         | ResNet50         | MRI               | CLS, REC   | 2024 | [GitHub](https://github.com/AIM-KannLab/BrainIAC)                                         |
| CIA-Net                     | FSL                | CL           | FT         | ResNet           | X-ray             | CLS, DET   | 2019 |                                                                                           |
| ClinicalContrastiveLearning | FSL                | CL           | FT         | ResNet           | OCT               | CLS        | 2023 |                                                                                           |
| SSRDL                       | FSL                | CL           | FT         | ViT (DINO)       | Path.             | CLS        | 2025 | [GitHub](https://github.com/lazytkm/SSRDL)                                                |
| SAM                         | FSL, Interp.       | CL           | PE         | ResNet, FPN      | CT, X-ray         | Multi-task | 2022 | [GitHub](https://github.com/alibaba-damo-academy/self-supervised-anatomical-embedding-v2) |
| DINOv2-ALPNet               | FSL                | CL           | FT, PEFT   | ViT (DINOv2)     | CT, MRI           | SEG        | 2024 | [GitHub](https://github.com/levayz/DINOv2-based-Self-Supervised-Learning)                 |
| ViT-3D-Med                  | FSL, Interp.       | CL           | FT         | ViT (DeiT-S)     | CT                | CLS        | 2022 |                                                                                           |
| Adam                        | FSL, Interp.       | CL           | FT         | ResNet           | X-ray, Fundus     | Multi-task | 2023 | [GitHub](https://github.com/MR-HosseinzadehTaher/Eden)                                    |
| UNI                         | FSL, DG, Interp.   | CL           | PEFT       | ViT-L            | Path.             | Multi-task | 2024 | [GitHub](https://github.com/mahmoodlab/UNI)                                               |
| PDCR-UAFR                   | FSL, Interp.       | CL           | FT         | DeepLabV3+       | Multimodal images | SEG        | 2022 | [GitHub](https://github.com/lzh19961031/PDCR_UAFR-MIS)                                    |
| LVM-Med                     | DG                 | CL           | FT, PE     | ResNet, ViT      | Multimodal images | Multi-task | 2023 | [GitHub](https://github.com/duyhominhnguyen/LVM-Med)                                      |
| BROW                        | FSL, DE-Adapt.     | CL           | PEFT       | ViT              | Path.             | CLS, SEG   | 2023 | [GitHub](https://github.com/openmedlab/BROW)                                              |
| Endo-FM                     | DG                 | CL           | FT         | Transformer      | Endo. Vid.        | Multi-task | 2023 | [GitHub](https://github.com/openmedlab/Endo-FM)                                           |
| Virchow                     | FSL, DG            | CL           | PEFT       | ViT (DINOv2)     | Path.             | CLS        | 2024 |                                                                                           |
| MedLSAM                     | FSL                | CL           | PE         | CNN, ViT         | CT                | DET, SEG   | 2025 | [GitHub](https://github.com/openmedlab/MedLSAM)                                           |
| MoCo-CXR                    | FSL                | CL           | FT         | ResNet, DenseNet | X-ray             | CLS        | 2021 | [GitHub](https://github.com/stanfordmlgroup/MoCo-CXR)                                     |
| RudolfV                     | FSL, DG            | CL           | FT, PEFT   | ViT (DINOv2)     | Path.             | Multi-task | 2024 |                                                                                           |
| SimCLR                      | FSL                | CL           | FT         | ResNet           | Nat. Img.         | CLS        | 2020 | [GitHub](https://github.com/google-research/simclr)                                       |
| CTransPath                  | DG, Interp.        | CL           | PEFT, FT   | Swin Transformer | Path.             | Multi-task | 2022 | [GitHub](https://github.com/Xiyue-Wang/TransPath)                                         |

---

## 📊 Table 3: Summary of Hybrid and Supervised Learning Approaches

| Methods            | Research Questions | Pre-training | Adaptation | Backbone         | Modalities        | Downstream | Year | Code                                                    |
| ------------------ | ------------------ | ------------ | ---------- | ---------------- | ----------------- | ---------- | ---- | ------------------------------------------------------- |
| HeadCT-Foundation  | FSL, DG, Interp.   | HL           | FT         | ViT-3D           | CT                | CLS        | 2025 | [GitHub](https://github.com/NYUMedML/headCT_foundation) |
| MedicalTransformer | FSL                | HL           | FT         | ResNet           | MRI               | Multi-task | 2023 | [GitHub](https://github.com/ejjun92/MedicalTransformer) |
| TransVW            | FSL                | HL           | FT         | U-Net, ResNet    | CT, X-ray         | CLS, SEG   | 2021 | [GitHub](https://github.com/fhaghighi/TransVW)          |
| PCRL               | FSL, DG            | HL           | FT         | U-Net            | XR, CT, MRI       | SEG, CLS   | 2021 | [GitHub](https://github.com/Luchixiang/PCRL)            |
| DSMT-Net           | FSL, DG, Interp.   | HL           | FT         | ViT              | Endo.             | Multi-task | 2024 | [GitHub](https://github.com/Torchlight-ljj/DSMT-Net)    |
| TITAN              | FSL, DG            | HL           | -          | ViT (ALiBi)      | Path. WSI, Text   | Multi-task | 2025 | [GitHub](https://github.com/mahmoodlab/TITAN)           |
| Alice              | DG, Interp.        | HL           | FT         | ViT              | CT                | SEG, CLS   | 2023 | [GitHub](https://github.com/alibaba-damo-academy/alice) |
| UniMiSS+           | DG                 | HL           | FT         | MiT, MedT        | CT, X-ray         | SEG, CLS   | 2024 | [GitHub](https://github.com/YtongXie/UniMiSS-code)      |
| CADS               | DG                 | HL           | FT         | PVT-Unet         | CT, X-ray         | SEG        | 2025 | [GitHub](https://github.com/yeerwen/CADS)               |
| SegVol             | FSL, Interp.       | HL           | FT, PE     | 3D ViT           | CT, MRI           | SEG        | 2023 | [GitHub](https://github.com/BAAI-DCAI/SegVol)           |
| Swin UNETR         | FSL, DG            | HL           | FT         | Swin Transformer | CT                | SEG        | 2022 | [GitHub](https://github.com/LeonidAlekseev/Swin-UNETR)  |
| GATE               | FSL, Interp.       | SL           | FT         | GCN              | fMRI              | CLS        | 2023 | [GitHub](https://github.com/LarryUESTC/GATE)            |
| HGFM               | FSL, Interp.       | SL           | FT         | HGNN             | fMRI              | CLS        | 2025 |                                                         |
| STU-Net            | Generalizab.       | SL           | FT         | U-Net            | CT, MRI, PET      | SEG        | 2023 | [GitHub](https://github.com/uni-medical/STU-Net)        |
| VisionFM           | FSL, DG            | SL           | PEFT       | Transformer      | Multimodal Ophth. | Multi-task | 2024 |                                                         |
| Med3D              | FSL, DG            | SL           | FT         | ResNet           | CT, MRI           | SEG, CLS   | 2019 | [GitHub](https://github.com/Tencent/MedicalNet)         |

---

## 📊 Table 4: Summary of Prompt-Driven Foundation Models

| Methods        | Research Questions | Pre-training | Adaptation | Backbone       | Modalities         | Downstream | Year | Code                                                        |
| -------------- | ------------------ | ------------ | ---------- | -------------- | ------------------ | ---------- | ---- | ----------------------------------------------------------- |
| KnowSAM        | FSL, SSL           | PD           | PEFT       | U-Net, V-Net   | Multimodal images  | SEG        | 2025 | [GitHub](https://github.com/taozh2017/KnowSAM)              |
| VerSemi        | FSL, SSL           | PD           | FT         | V-Net          | CT, MRI            | SEG        | 2025 | [GitHub](https://github.com/maxwell0027/VerSemi)            |
| AdaptiveSAM    | FSL, DG, Interp.   | PD           | PEFT       | ViT (SAM)      | Surg. Vid., US, XR | SEG        | 2023 | [GitHub](https://github.com/JayParanjape/biastuning)        |
| SegmentAnyBone | FSL, DG            | PD           | PEFT       | ViT (SAM)      | MRI                | SEG        | 2024 | [GitHub](https://github.com/mazurowski-lab/SegmentAnyBone)  |
| SurgicalSAM    | DG, PS             | PD, CL       | PEFT       | ViT (SAM)      | Endo.              | SEG        | 2023 | [GitHub](https://github.com/wenxi-yue/SurgicalSAM)          |
| SAM-LoRA       | FSL                | PD           | PEFT       | ViT-Base (SAM) | MRI, CT            | SEG        | 2024 |                                                             |
| DeSAM          | DG                 | PD           | PEFT       | SAM, ViT-H     | CT, MRI            | SEG        | 2024 | [GitHub](https://github.com/yifangao112/DeSAM)              |
| SAMM           | DG                 | PD           | PE         | ViT (SAM)      | CT, MRI, US        | SEG        | 2024 | [GitHub](https://github.com/bingogome/samm)                 |
| SAM-Path       | DG                 | PD, CL       | FT, PE     | ViT, ViT-Small | Path.              | SEG        | 2023 | [GitHub](https://github.com/cvlab-stonybrook/SAMPath)       |
| SAMed          | DG                 | PD           | PEFT       | ViT (SAM)      | CT                 | SEG        | 2023 | [GitHub](https://github.com/hitachinsk/SAMed)               |
| nnSAM          | FSL                | PD           | FT         | ViT, nnUNet    | CT, MRI, X-ray     | SEG        | 2024 | [GitHub](https://github.com/Kent0n-Li/nnSAM)                |
| SAMAug         | DG                 | PD           | -          | ViT, CNN-based | Endo., Path.       | SEG        | 2023 | [GitHub](https://github.com/yhydhx/SAMAug)                  |
| AutoSAM        | DG                 | PD           | PE         | ViT, H-Dense   | Path., Endo.       | SEG        | 2023 | [GitHub](https://github.com/talshaharabany/AutoSAM)         |
| MSA            | DG                 | PD           | PEFT       | ViT (SAM)      | Multimodal images  | SEG        | 2025 | [GitHub](https://github.com/ImprintLab/Medical-SAM-Adapter) |
| MA-SAM         | FSL, DG            | PD           | PEFT       | ViT (SAM)      | Multimodal image   | SEG        | 2024 | [GitHub](https://github.com/cchen-cc/MA-SAM)                |
| SAM-Med2D      | DG                 | PD           | FT         | ViT (SAM)      | Multimodal images  | SEG        | 2023 | [GitHub](https://github.com/OpenGVLab/SAM-Med2D)            |
| AFTer-SAM      | DG                 | PD           | PEFT       | ViT (SAM)      | CT                 | SEG        | 2024 |                                                             |
| 3DSAM-adapter  | DG                 | PD           | PEFT       | ViT (SAM)      | CT                 | SEG        | 2023 | [GitHub](https://github.com/med-air/3DSAM-adapter)          |
| ProMISe        | FSL, DG            | PD           | PEFT, PE   | ViT (SAM), CNN | CT                 | SEG        | 2024 | [GitHub](https://github.com/MedICL-VU/ProMISe)              |
| CellSAM        | FSL, DG            | PD           | PEFT       | ViT (SAM)      | Multimodal images  | SEG        | 2025 | [GitHub](https://github.com/vanvalenlab/cellSAM)            |
| MVG            | FSL, DG            | PD, GL       | PE         | ViT            | Multimodal images  | SEG        | 2024 | [GitHub](https://github.com/OliverRensu/MVG)                |
| VISTA3D        | FSL, DG            | PD, SL       | FT         | SegResNet      | CT                 | SEG        | 2025 | [GitHub](https://github.com/Project-MONAI/VISTA)            |
| UniverSeg      | FSL, DG            | PD, SL       | PE         | U-Net          | Multimodal images  | SEG        | 2023 | [GitHub](https://github.com/JJGO/UniverSeg)                 |

---

## 📌 Abbreviation Key

| Abbreviation | Meaning                         |
| ------------ | ------------------------------- |
| FSL          | Few-Shot Learning               |
| DG           | Domain Generalization           |
| Interp.      | Interpretability                |
| SSL          | Self-Supervised Learning        |
| GL           | Generative Learning             |
| CL           | Contrastive Learning            |
| HL           | Hybrid Learning                 |
| SL           | Supervised Learning             |
| PD           | Prompt-Driven                   |
| PEFT         | Parameter-Efficient Fine-Tuning |
| FT           | Full Fine-Tuning                |
| PE           | Prompt Engineering              |
| Path.        | Pathology                       |
| Endo.        | Endoscopy                       |
| US           | Ultrasound                      |
| OCT          | Optical Coherence Tomography    |
| CFP          | Color Fundus Photography        |
| sMRI         | structural MRI                  |
| WSI          | Whole Slide Image               |
| fMRI         | functional MRI                  |
| CLS          | Classification                  |
| SEG          | Segmentation                    |
| REC          | Reconstruction                  |
| REG          | Registration                    |
| DET          | Detection                       |
| Cont.        | Continual Learning              |
| Label Eff.   | Label Efficiency                |
| DE-Adapt.    | Data-efficient Adaptation       |
| Surg. Vid.   | Surgical Video                  |
| Nat. Img.    | Natural Images                  |
| Gen.         | Genetics                        |
| Micro.       | Microscopy                      |

---

## 📚 About

This collection is part of the ongoing review:  
**Medical Vision Foundation Models: A Comprehensive Review from Technical Evolution to Clinical Translation**  
_(Currently under review)_

Maintained by: [Nengjian Lin et al.](https://github.com/ice-TuoShui/MVFM-Review)

---

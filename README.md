# LWANet: Lightweight Wavelet Attention Network for 3D-HEVC Compressed Depth Map Enhancement

Official PyTorch implementation of the paper **"LWANet: Lightweight Wavelet Attention Network for 3D-HEVC Compressed Depth Map Enhancement"**.

[![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)](https://pytorch.org/) 
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Journal](https://img.shields.io/badge/Journal-Nuclear%20Physics%20B-green.svg)](https://www.journals.elsevier.com/nuclear-physics-b)

---

## 📖 Introduction

![fig1_page-0001](https://github.com/user-attachments/assets/64021028-8799-4823-b60f-f8c552bede95)

Depth maps play a crucial role in synthesized view generation for 3D Video (3DV) systems. However, **3D-HEVC** compression inevitably introduces artifacts like blockiness and ringing, which degrade the quality of synthesized views and cause visual discomfort in VR/AR applications.

**LWANet** is an ultra-lightweight deep learning solution that:
- Employs a **dual-stream architecture** to capture global geometric structures and local details.
- Integrates a **wavelet attention mechanism** to reduce spatial redundancy while preserving high-frequency edges.
- Achieves state-of-the-art performance with only **461K parameters** (a 60% reduction compared to existing methods).

---

## ✨ Key Contributions

![fig2_page-0001](https://github.com/user-attachments/assets/315925db-343f-42ba-a4ba-729666ba432d)

* **Specific Design for Depth Maps:** Unlike general image enhancement, LWANet focuses on the geometric characteristics of depth maps to ensure high-fidelity virtual view synthesis.
* **Lightweight Feature Extraction (LFE):** Utilizes Wavelet Channel Aggregation (WCA) and Wavelet Residual Blocks (WRB) for efficient multi-scale analysis.
* **Residual Feature Enhancement (RFE):** A hierarchical branch that progressively refines features using Multi-level Wavelet Residual Blocks (MWRB).
* **Efficiency-Performance Balance:** Optimized for real-time multimedia systems with minimal computational overhead.

---

## 🛠️ Network Architecture

The pipeline consists of three main stages:
1.  **LFE Module:** Extracts multi-scale features via wavelet decomposition and adaptive channel weighting.
2.  **RFE Module:** Progressively enhances the extracted features to recover lost edge details.
3.  **Reconstruction Stage:** Aggregates all refined information to generate the final high-quality depth map.

---

## 🚀 Getting Started

> [!IMPORTANT]
> **The full source code and pre-trained models will be released soon upon the official acceptance of the paper.** ---

## ✍️ Citation

If you use this code or model in your research, please cite our paper:
> **The full source code and pre-trained models will be released soon upon the official acceptance of the paper.** ---

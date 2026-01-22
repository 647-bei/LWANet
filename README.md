# LWANet: Lightweight Wavelet Attention Network for 3D-HEVC Compressed Depth Map Enhancement

Official implementation of the paper: **"LWANet: Lightweight Wavelet Attention Network for 3D-HEVC Compressed Depth Map Enhancement"**.

[![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)](https://pytorch.org/) 
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Academic](https://img.shields.io/badge/Journal-Nuclear%20Physics%20B-green.svg)](https://www.journals.elsevier.com/nuclear-physics-b)

---

## 📖 Introduction

In 3D Video (3DV) systems, depth map quality is crucial for synthesized view generation. However, depth maps compressed by **3D-HEVC** often suffer from severe artifacts (blockiness, ringing), which lead to geometric distortions and visual discomfort in VR/AR applications.

**LWANet** is a novel lightweight solution designed to:
- **Repair** edge distortions and detail loss caused by lossy compression.
- **Minimize** model complexity (only **461K** parameters) for real-time applications.
- **Leverage** Wavelet Transform to capture multi-scale features and key regions effectively.



---

## ✨ Key Contributions

1. **Focus on Depth Enhancement:** This is the first work to specifically address depth map distortions in 3D-HEVC, directly optimizing the quality of synthesized views from the source.
2. **Dual-Stream Architecture:** Integrates a **Lightweight Feature Extraction (LFE)** branch for multi-scale capture and a **Residual Feature Enhancement (RFE)** branch for detail refinement.
3. **Ultra-Lightweight:** Achieves superior performance with **over 60% reduction** in parameters compared to existing state-of-the-art image enhancement algorithms.

---

## 🛠️ Method Overview

### LWANet Framework
LWANet consists of three main stages:
- **LFE Module:** Uses Wavelet Channel Aggregation (WCA) and Wavelet Residual Blocks (WRB) to extract features while reducing spatial redundancy.
- **RFE Module:** Features a Multi-level Wavelet Residual Block (MWRB) that captures hierarchical wavelet coefficients.
- **Reconstruction:** Aggregates refined features through simplified convolution layers to output high-quality depth maps.



---

## 📊 Experimental Results

LWANet provides a better balance between **Performance (PSNR)** and **Computational Cost (FLOPs)** compared to common methods like QECNN, TSAN, and RDEN.

| Metric | Parameters | PSNR (dB) | SSIM |
| :--- | :--- | :--- | :--- |
| **LWANet (Ours)** | **461 K** | *Check paper* | *Check paper* |

[Image comparing LWANet's PSNR vs GFLOPs performance against other methods like QECNN and MIRNet]

---

## 🚀 Getting Started

### Prerequisites
- Python 3.x
- PyTorch
- CUDA (if training/testing on GPU)

### Installation
```bash
git clone [https://github.com/647-bei/LWANet.git](https://github.com/647-bei/LWANet.git)
cd LWANet
pip install -r requirements.txt

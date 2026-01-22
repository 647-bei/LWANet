LWANet: Lightweight Wavelet Attention Network for 3D-HEVC Compressed Depth Map Enhancement
Official PyTorch implementation of the paper: "LWANet: Lightweight Wavelet Attention Network for 3D-HEVC Compressed Depth Map Enhancement".

📖 Introduction
In 3D Video (3DV) systems, depth map quality is crucial for virtual view synthesis (DIBR). However, the 3D-HEVC standard introduces significant compression artifacts (blockiness, ringing) in depth maps, leading to holes and geometric distortions in synthesized views.

LWANet is a novel lightweight solution that:

Dual-Stream Architecture: Combines a Lightweight Feature Extraction (LFE) branch and a Residual Feature Enhancement (RFE) branch.

Wavelet Attention Mechanism: Leverages Wavelet Transform (WT) to capture multi-scale features and preserve high-frequency edge information.

Extreme Efficiency: Reduces model parameters by over 60% (only 461K) while achieving state-of-the-art enhancement performance.

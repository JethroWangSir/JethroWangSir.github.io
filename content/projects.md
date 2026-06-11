---
title: "Selected Projects"
date: 2026-06-11
draft: false
---

* **Enterprise AI Evaluation & Speech Deployment Workflows** | E.SUN Financial Holding Co., Ltd.
  * Built evaluation workflows for internal KM context recall and internal ASR benchmarking.
  * Deployed an external vendor's **VoAI TTS** model to an internal **GKE** environment.
  * Focus: enterprise AI evaluation, speech model assessment, cloud-native deployment, and reproducible benchmarking.
  * 企業內部 AI 專案：KM context recall 指標評估、ASR 評估流程、VoAI TTS 模型上 GKE 部署。
* **MOS Predictor for AudioMOS Challenge 2025 - QAMRO** [C4] | May 2025 - Jun. 2025
  * Designed a quality-aware ranking system for evaluating text-to-speech (TTS), text-to-audio (TTA), and text-to-music (TTM) generation systems.
  * Achieved **3rd place for Track 1** in AudioMOS Challenge 2025.
  * Research focus: human-aligned audio generation assessment, adaptive margin ranking, and robust MOS prediction.
  * [GitHub Repository](https://github.com/JethroWangSir/QAMRO)
* **Keyword Spotter** | Realtek Semiconductor Corp. | Mar. 2025 - May 2025
  * Improved two keyword spotting models, [BC-ResNet](https://github.com/JethroWangSir/bcresnet/tree/sr) and [PhonMatchNet](https://github.com/JethroWangSir/PhonMatchNet/tree/phonmatchnet), for noisy industrial scenarios.
  * Achieved a **43.23% reduction in false alarms** under challenging noise conditions.
  * Focus: robust KWS, false alarm reduction, noisy-condition evaluation, and model comparison.
* **Voice Activity Detector - SincQDR-VAD** [C5] | Realtek Semiconductor Corp. | Nov. 2024 - Feb. 2025
  * Built a compact noise-robust VAD framework using a learnable **Sinc-extractor** front end and **quadratic disparity ranking (QDR)** loss.
  * Improved robustness in low-SNR scenarios, including absolute AUROC gains on AVA-Speech and relative F2-Score gains on ACAM.
  * Reduced parameter count by **31%** compared with a representative lightweight VAD baseline, supporting practical edge/resource-constrained deployment.
  * [Paper](https://arxiv.org/pdf/2508.20885)
  * [Hugging Face Demo](https://huggingface.co/spaces/jethrowang/SincQDR-VAD)

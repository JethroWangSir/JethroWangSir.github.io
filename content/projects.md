---
title: "Selected AI/ML Projects"
date: 2026-06-11
draft: false
---

精選專案聚焦於企業 AI 評估與語音模型研究，涵蓋 KM retrieval/context recall、ASR benchmark、TTS deployment、MOS prediction、KWS、VAD 等應用。

* **Enterprise AI Evaluation & Speech Deployment Workflows** | E.SUN Financial Holding Co., Ltd.
  * Problem: establish reproducible evaluation workflows for internal KM retrieval quality, ASR comparison, and TTS service deployment.
  * Method: defined **recall** and **context recall** metrics using **600 test questions** (200 retail banking, 400 corporate banking) and **250 documents** (100 retail, 150 corporate).
  * Result: built **MER-based ASR benchmarking** for internal Kaldi models, pre-trained Whisper, and Gemini ASR; deployed **VoAI TTS** as an internal service/API on **GKE**.
  * 中文摘要：企業內部 AI 專案，涵蓋 KM recall/context recall 評估、ASR MER benchmark、VoAI TTS 模型上 GKE 內部服務部署。
* **MOS Predictor for AudioMOS Challenge 2025 - QAMRO** [C4] | May 2025 - Jun. 2025
  * Problem: improve human-aligned quality assessment for TTS, TTA, and TTM generation systems.
  * Method: designed a quality-aware adaptive margin ranking system for robust MOS prediction.
  * Result: achieved **3rd place for Track 1** in AudioMOS Challenge 2025.
  * 中文摘要：設計音訊生成品質評估模型，在 AudioMOS Challenge 2025 Track 1 獲得第三名。
  * [GitHub Repository](https://github.com/JethroWangSir/QAMRO)
* **Keyword Spotter** | Realtek Semiconductor Corp. | Mar. 2025 - May 2025
  * Problem: reduce false alarms for keyword spotting under challenging noisy conditions.
  * Method: improved [BC-ResNet](https://github.com/JethroWangSir/bcresnet/tree/sr) and [PhonMatchNet](https://github.com/JethroWangSir/PhonMatchNet/tree/phonmatchnet) variants for industrial KWS scenarios.
  * Result: achieved a **43.23% reduction in false alarms** under challenging noise conditions.
  * 中文摘要：與 Realtek 產學合作，針對噪音環境改善 KWS 模型並降低誤觸發。
* **Voice Activity Detector - SincQDR-VAD** [C5] | Realtek Semiconductor Corp. | Nov. 2024 - Feb. 2025
  * Problem: improve VAD robustness under unseen and low-SNR noise conditions.
  * Method: built a compact noise-robust VAD framework using a learnable **Sinc-extractor** front end and **quadratic disparity ranking (QDR)** loss.
  * Result: improved low-SNR robustness, increased AUROC/F2-Score by **5%**, and reduced parameter count by **31%** compared with a representative lightweight VAD baseline.
  * 中文摘要：與 Realtek 產學合作，提出 SincQDR-VAD，在低訊噪比情境提升語音偵測穩健性並降低模型參數量。
  * [Paper](https://arxiv.org/pdf/2508.20885)
  * [Hugging Face Demo](https://huggingface.co/spaces/jethrowang/SincQDR-VAD)

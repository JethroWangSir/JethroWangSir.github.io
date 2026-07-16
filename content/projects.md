---
title: "Selected AI/ML Projects"
date: 2026-07-16
draft: false
---

精選專案聚焦於企業級 AI 應用落地、生成式 AI 自動化評估，以及穩健語音演算法研究。

## 🏢 Enterprise AI & Production (E.SUN Bank)

* **Wealth Management Copilot (個金 Copilot)** | Jun. 2026 - Present
  * **Objective:** Modernize the conversational AI experience by transitioning from high-latency batch processing to a real-time streaming architecture, ensuring transparent system state tracking (e.g., retrieving, thinking).
  * **Implementation:** Engineered a robust backend streaming pipeline utilizing Server-Sent Events (SSE) via the Google ADK. Orchestrated an advanced agentic workflow integrating **Gemini 3.5 Flash** with **Vertex AI RAG**.
  * **Current Status:** Successfully deployed the streaming backend for testing, enabling seamless, typewriter-like dynamic responses and real-time operational transparency.
  * **中文摘要：** 開發個金 Copilot 後端串流服務。導入 Google ADK Server-Sent Events (SSE) 技術，並整合 Gemini 3.5 Flash 與 Vertex AI RAG 構建代理工作流 (Agentic Workflow)，將原先的批次延遲回覆升級為具備系統狀態追蹤、打字機般流暢的即時互動體驗。

* **Streaming TTS (TTS 平台)** | May 2026 - Present
  * **Objective:** Operationalize internal Text-to-Speech (TTS) models by packaging and deploying them into a highly scalable, production-ready environment.
  * **Implementation:** Containerized proprietary VoAI TTS models and established them as robust internal microservices/APIs deployed on **Google Kubernetes Engine (GKE)**.
  * **Current Status:** Successfully provisioned a scalable API infrastructure, currently preparing for comprehensive integration testing with downstream enterprise banking services.
  * **中文摘要：** 負責企業級 TTS 平台的模型服務化與部署。將內部自研之 VoAI TTS 模型全面容器化，並部署於 Google Kubernetes Engine (GKE) 作為內部 API 服務，成功建立具備高擴展性的基礎架構，為後續全行系統串接奠定基礎。

* **E.SUN Knowledge Management Evaluation Pipeline (全行 KM)** | Apr. 2026 - Jun. 2026
  * **Objective:** Design and establish a reproducible, automated evaluation workflow to continuously monitor and optimize the retrieval quality of the enterprise-wide RAG system.
  * **Implementation:** Architected an automated evaluation pipeline leveraging the **Ragas** framework and an **LLM-as-a-judge** methodology (powered by **Gemini 3.1 Flash Lite**) to precisely compute context recall.
  * **Impact:** Delivered a standardized metric calculation tool that empowers business units to autonomously quantify and verify the performance impact of new document ingestions prior to production deployment.
  * **中文摘要：** 建立全行知識管理 (KM) 系統的 RAG 自動化評估管線。結合 Ragas 框架與 Gemini 3.1 Flash Lite，導入 LLM-as-a-judge 評估機制精準計算 Context Recall。此工具成功賦能業管單位，使其能在新文件上線前自動化量化並驗證檢索品質。
---

## 🔬 Advanced Speech Processing & Deep Learning Research

* **MOS Predictor for AudioMOS Challenge 2025 - QAMRO** [C2] | May 2025 - Jun. 2025
  * **Objective:** Enhance human-aligned quality assessment mechanisms for advanced speech and music generation systems (TTS, TTA, TTM).
  * **Implementation:** Developed QAMRO (Quality-Aware Adaptive Margin Ranking Optimization), a novel framework designed for robust Mean Opinion Score (MOS) prediction.
  * **Impact:** Awarded **3rd Place for Track 1** at the globally recognized AudioMOS Challenge 2025.
  * **中文摘要：** 研發針對語音與音樂生成系統的高擬真品質評估模型。提出 QAMRO 框架以優化 MOS 預測之穩健性，並榮獲國際賽事 AudioMOS Challenge 2025 Track 1 全球第三名。
  * [GitHub Repository](https://github.com/JethroWangSir/QAMRO)

* **Keyword Spotter** | Realtek Semiconductor Corp. | Mar. 2025 - May 2025
  * **Objective:** Mitigate false alarm rates in industrial keyword spotting (KWS) systems operating under severe, non-stationary noise environments.
  * **Implementation:** Optimized and enhanced the architectures of [BC-ResNet](https://github.com/JethroWangSir/bcresnet/tree/sr) and [PhonMatchNet](https://github.com/JethroWangSir/PhonMatchNet/tree/phonmatchnet) variants tailored for complex industrial deployment scenarios.
  * **Impact:** Achieved a substantial **43.23% reduction in false alarms**, significantly boosting system reliability under challenging acoustic conditions.
  * **中文摘要：** 與瑞昱半導體進行產學合作，針對高雜訊工業場景優化關鍵字喚醒 (KWS) 系統。透過改良 BC-ResNet 與 PhonMatchNet 模型架構，在複雜且非平穩的噪音環境下，成功將誤觸發率大幅降低 43.23%。

* **Voice Activity Detector - SincQDR-VAD** [C3] | Realtek Semiconductor Corp. | Nov. 2024 - Feb. 2025
  * **Objective:** Elevate the robustness of Voice Activity Detection (VAD) systems specifically for low-SNR and unseen acoustic environments.
  * **Implementation:** Engineered SincQDR-VAD, a compact and noise-robust framework integrating a learnable **Sinc-extractor** front-end with a novel **Quadratic Disparity Ranking (QDR)** loss function.
  * **Impact:** Outperformed representative lightweight VAD baselines by increasing AUROC and F2-Score by **5%**, while simultaneously reducing the total model parameter count by **31%**.
  * **中文摘要：** 聯手瑞昱半導體開發輕量且抗噪的語音活動偵測 (VAD) 框架。結合可學習的 Sinc-extractor 前端與二次差異排序 (QDR) 損失函數，在模型參數量減少 31% 的前提下，於低訊噪比環境中將 AUROC 與 F2-Score 逆勢提升 5%。
  * [Paper](https://arxiv.org/pdf/2508.20885) | [Hugging Face Demo](https://huggingface.co/spaces/jethrowang/SincQDR-VAD)

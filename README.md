# AI Co-Scientist-Guided Generative Augmentation for Rare Disease Research
**Democratizing Medical AI for Rare Diseases: A Human-AI Collaborative VAE Framework**

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](#)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-2.0%2B-ee4c2c)
![License](https://img.shields.io/badge/License-MIT-green)

## Project Overview
This repository contains the official implementation of the research paper: **"Democratizing Medical AI for Rare Diseases: A Human-AI Collaborative VAE Framework."**

We address the "Small-n, Large-p" problem in rare disease research (specifically Celiac Disease) by utilizing a **Variational Autoencoder (VAE)** optimized via **Sampling Temperature Scaling**. This project was conducted under the **AI Co-Scientist Framework**, where AI agents actively participated in hypothesis generation, coding, and robustness validation.

## Key Features
* **AI Co-Scientist Collaboration:** Full research lifecycle managed with Multi-LLM agents.
* **Robustness Validated:** Proven stability across **5 independent runs** (Random Seeds: 42, 10, 2024, 777, 99).
* **Optimized VAE:** Overcomes mode collapse using `Sampling Temperature = 2.0`.
* **High Utility:** Achieved **TSTR Accuracy 0.993 ± 0.015**.

## Results (Reproducibility Check)
We validated the reproducibility of our model by running the pipeline 5 times with different random seeds.
Results are reported as mean ± standard deviation over five independent runs.

| Metric | Mean ± Std | Range |
| :--- | :--- | :--- |
| **Accuracy** | **0.993 ± 0.015** | [0.965 - 1.000] |
| **F1-score** | **0.993 ± 0.015** | [0.966 - 1.000] |

<p align="center">
  <img src="results/figures/pca_validation_final.png" width="600" alt="Representative PCA Plot">
  <br>
  <em>Figure: Representative visualization of the latent space (Run 1). The synthetic data (orange) closely aligns with the real data (blue).</em>
</p>

## Installation & Usage

1. **Clone the repository**
   ```bash
   git clone https://github.com/SynBio-AI-Lab/Celiac-VAE-Augmentation.git
   cd Celiac-VAE-Augmentation

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt

3. **Run the 5-Run Robustness Check**
   ```bash
   python robustness_check.py
   
## Co-Scientist Statement
This project is a submission for the **2026 AI Co-Scientist Challenge**, demonstrating a fully collaborative research loop between human and AI agents.

* **Human Researcher:** Project design, Decision making, Final validation.
* **AI Agents (The Team):**
  * **Cursor (Claude 4.5 Opus):** Core implementation (VAE modeling), Designing the "5-Run Robustness Check" pipeline.
  * **Gemini 3 Pro:** Academic writing, Logical flow verification, Peer review simulation (Reviewer role).
  * **Perplexity:** Literature review, Initial translation using domain-specific terminology search.
  * **ChatGPT (GPT-5.2):** Cross-Validation & Red Teaming. Verified reference integrity (detected/fixed truncation errors) and cross-checked translation nuances.
 
## Contact
(Anonymous for Blind Review)

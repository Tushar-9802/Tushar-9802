## Hi, I'm Tushar 👋

I'm an ML engineer who fine-tunes small language models on consumer hardware — and builds the products around them. Most of my work sits at the messy intersection of **applied research** and **things people actually use**: clinical AI for frontline health workers, offline-first LLM pipelines, and cross-modal transfer learning.

My paper on cross-modal LoRA degradation was presented at **IMPACT 2025 (Springer)**. A second one, on preventing catastrophic forgetting, is in preparation.

Systems Dev intern @ Cognavi &nbsp;·&nbsp; Uttar Pradesh, India &nbsp;·&nbsp; [Portfolio](https://tushar-9802.github.io/Portfolio/)

---

### Research

**Cross-Modal Transfer Learning in Domain-Adaptive Video Summarization**
*IMPACT 2025, Springer — presented Dec 6, 2025 · proceedings forthcoming*

I found that LoRA fine-tuning on academic papers degrades video summarization by 14–50%, then built a 5-method curriculum framework to fix it.

| System | Video ROUGE-1 | Video ROUGE-2 | CMC |
|---|---|---|---|
| Baseline (zero-shot) | 0.263 | 0.032 | 0.356 |
| IMPACT 2025 naive LoRA | 0.272 | 0.060 | — |
| **Full framework (Phase 3)** | **0.417 (+58%)** | **0.119 (+272%)** | **0.531** |

*p < 0.005, paired t-test · bootstrap 95% CI · 1,400-line eval harness*

Second paper in preparation: *Preventing Catastrophic Forgetting in Cross-Modal Summarization*.

---

### Projects

**Clinical AI**

| Project | What it does | Highlights |
|---|---|---|
| **[Sakhi](https://github.com/Tushar-9802/Sakhi)** | Offline-first Hindi voice-to-form for India's 1M+ ASHA health workers — home-visit conversations become structured government forms with real-time maternal & child referral decisions. | 87% end-to-end pass on synthetic Hindi audio · dual deploy: health-center (~15s) + on-device Android via Cactus SDK (~5min) · 6-layer anti-hallucination pipeline · Gemma 4 Good Hackathon |
| **[MedScribe](https://github.com/Tushar-9802/MedScribe)** | Speech → concise SOAP notes in physician shorthand, fully offline on 16GB VRAM. Built for the Google MedGemma Impact Challenge 2026. | 16 → 5 min per encounter · 0% hallucinated findings · 90/100 quality · LoRA-tuned on 712 samples for $1.28 |

**Generative AI**

| Project | What it does | Highlights |
|---|---|---|
| **[YouTube Transcript Summariser](https://github.com/Tushar-9802/YouTube-Transcript-Summarizer)** | Domain-adaptive summarization for 90-minute lectures on a single 8GB GPU. The negative result that started the research. | Published — IMPACT 2025 (Springer) · documented a 14–50% cross-modal ROUGE drop, p<0.001 |
| **[Hybrid Dataset Summariser](https://github.com/Tushar-9802/Hybrid-Dataset-Summariser)** | The follow-up that fixes it — a 3-phase curriculum (LoRA+, OPLoRA, EWC, CrossCLR) on Mistral-7B over a 4,324-sample cross-modal dataset. | Video ROUGE-1 0.417 (+58%), ROUGE-2 +272% · forgetting held at 14.1% vs 31.4% · all gains p<0.005 · [HF model](https://huggingface.co/Tushar9802/hybrid-summariser-crossmodal-lora) · [dataset](https://www.kaggle.com/datasets/tusharjaju/hybrid-dataset-summariser-crossmodal) |
| **[Bawarchi](https://github.com/Tushar-9802/Bawarchi)** | Multimodal recipe generation: vision detects ingredients, embeddings + PMI suggest cuisine-appropriate swaps, a fine-tuned LLM writes the recipe. | YOLOv8m 66.5% mAP · substitution engine 85% precision · Llama 3.2 3B tuned on 335K recipes (74.1% accuracy) |

**Data Products**

| Project | What it does | Highlights |
|---|---|---|
| **[DPDPA Compliance](https://github.com/Tushar-9802/DPDPA)** | Legal-tech automation for India's Digital Personal Data Protection Act, 2023 — 50+ regulatory requirements assessed in minutes instead of days. | 40 hours → 5 minutes (480× the manual baseline) · ~95% PDF extraction accuracy · 9-table relational DB · 15-question assessment engine · targets the May 2027 deadline |
| **[Tech Layoffs Dashboard](https://github.com/Tushar-9802/Tech-Layoffs-Analysis)** | Interactive analytics on global tech-sector layoffs, 2020–2025, with six custom metrics (efficiency, instability, severity, and more). | [Live Streamlit](https://tushar9802-tech-layoffs-analysis.streamlit.app/) · YoY/QoQ trend analysis · company-level deep-dives · [Kaggle EDA](https://www.kaggle.com/code/tusharjaju/tech-layoffs-analysis-2020-2025) |

---

### Open Source

**[llmclean](https://pypi.org/project/llmclean/)** — zero-dependency Python library for cleaning and normalizing raw LLM output · PyPI

**[Model Adapters](https://huggingface.co/Tushar9802)** — trained LoRA adapters for MedScribe, Bawarchi, and the Hybrid Summariser · Hugging Face

**[Datasets](https://www.kaggle.com/tusharjaju)** — curated training datasets for all projects · Kaggle

---

### Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![CUDA](https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

Beyond the badges: Transformers · PEFT / LoRA · QLoRA · Unsloth · bitsandbytes · OPLoRA · EWC · Whisper · YOLOv8 · Mistral · Gemma · Llama 3.2

---

### GitHub

<p align="center">
  <img height="160" src="https://github-readme-stats.vercel.app/api?username=Tushar-9802&show_icons=true&hide_border=true&count_private=true" />
  <img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Tushar-9802&layout=compact&hide_border=true&langs_count=8" />
</p>

---

### Links

[Portfolio](https://tushar-9802.github.io/Portfolio/) · [Hugging Face](https://huggingface.co/Tushar9802) · [LinkedIn](https://linkedin.com/in/tushar-jaju-240b501a6) · [Kaggle](https://www.kaggle.com/tusharjaju) · tusharbrisingr9802@gmail.com

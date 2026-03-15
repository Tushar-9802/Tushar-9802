## Tushar Jaju — ML Engineer

Fine-tuning large language models on consumer hardware. Developing and Researching real-life projects.

---

### Research

**Cross-Modal Transfer Learning in Domain-Adaptive Video Summarization**  
*IMPACT 2025, Springer — presented Dec 6, 2025 · proceedings forthcoming*

Found that LoRA fine-tuning on academic papers degrades video summarization by 14–50%.
Built a 5-method curriculum framework to fix it.

| System | Video ROUGE-1 | Video ROUGE-2 | CMC |
|---|---|---|---|
| Baseline (zero-shot) | 0.263 | 0.032 | 0.356 |
| IMPACT 2025 naive LoRA | 0.272 | 0.060 | — |
| **Full framework (Phase 3)** | **0.417 (+58%)** | **0.119 (+272%)** | **0.531** |

*p < 0.005, paired t-test · bootstrap 95% CI · 1,400-line eval harness*

Second paper in preparation: *Preventing Catastrophic Forgetting in Cross-Modal Summarization*

---

### Projects

| Project | What it does | Key numbers |
|---|---|---|
| [Hybrid-Dataset-Summariser](https://github.com/Tushar-9802/Hybrid-Dataset-Summariser) | LoRA+, OPLoRA, EWC, CrossCLR curriculum on Mistral-7B | Video R-1 +58%, R-2 +272% · 4,324-sample cross-modal dataset |
| [MedScribe](https://github.com/Tushar-9802/MedScribe-1) | Speech → concise SOAP notes · 6 clinical tools · fully offline | 46% shorter notes · 0% hallucinations · 3.4GB VRAM · $1.28 training cost |
| [Bawarchi](https://github.com/Tushar-9802/Bawarchi) | YOLOv8 ingredient detection + role-aware recipe generation | 66.5% mAP · 74.1% recipe accuracy · 522K recipe corpus |
| [Tech-Layoffs-Analysis](https://github.com/Tushar-9802/Tech-Layoffs-Analysis) | Interactive dashboard · 6 custom metrics (LES, LIS, LSI, ...) | 2020–2025 · live Streamlit deploy |
| [YouTube-Transcript-Summarizer](https://github.com/Tushar-9802/YouTube-Transcript-Summarizer) | The negative result that started the research | Published finding: modality > domain similarity |

---

### Open Source

**[llmclean](https://pypi.org/project/llmclean/)** — zero-dependency Python library for cleaning and normalizing raw LLM output · PyPI

**[Model Adapters](https://huggingface.co/Tushar9802)** — Trained LoRA adapters for MedScribe, Bawarchi, and the Hybrid Summariser · HuggingFace

**[Datasets](https://www.kaggle.com/tusharjaju)** — Curated training datasets for all projects · Kaggle
---

### Stack

`PyTorch` `HuggingFace` `PEFT` `bitsandbytes` `Mistral-7B` `MedGemma` `Llama 3.2` `YOLOv8` `Whisper` `Gradio` `Streamlit` `Python` `SQL`


---

### Links

[Portfolio](https://tushar-9802.github.io/Portfolio/) · [HuggingFace](https://huggingface.co/Tushar9802) · [LinkedIn](https://linkedin.com/in/tushar-jaju-240b501a6) · [Kaggle](https://www.kaggle.com/tusharjaju) · tusharbrisingr9802@gmail.com

<div align="center">

# Houssem Eddine Ghribi

### AI Researcher & Engineer | Explainable AI · LLMs & RAG · Multimodal & Agentic Systems

<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=26&pause=1200&color=2E9EF7&center=true&vCenter=true&width=780&lines=I+build+AI+systems+and+prove+they+work;Explainable+AI+%C2%B7+LLMs+%C2%B7+RAG+%C2%B7+NLP+%C2%B7+Vision;Causal+Probing+%C2%B7+Rigorous+Evaluation;Seeking+a+PhD+%C2%B7+Fall+2027" alt="Typing SVG" />

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/houssemeddineds)
[![Email](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:houssemeddineds@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-D6C2A1?style=for-the-badge&logo=google-chrome&logoColor=black)](https://houssemds.github.io)
[![ORCID](https://img.shields.io/badge/ORCID-0009--0007--2027--2520-A6CE39?style=for-the-badge&logo=orcid&logoColor=white)](https://orcid.org/0009-0007-2027-2520)

</div>

---

## 👋 About Me

Final-year AI engineering student at ESPRIT University (Master's-level, graduating 2027) with **2+ years of industry AI work for companies in Germany and France**.

I am driven by one question: **does this AI system actually work, and why?** I build real systems (LLM and RAG platforms, vision models, multi-agent pipelines) and then open them up: causal probing to see what happens inside a model, controlled ablations to see which design choices matter, and pre-specified evaluation to make sure a result is real and not noise.

The domain changes, the method does not. Whether it is a **vision-language model** reading an X-ray, a **RAG system** answering from contracts, an **LLM** writing clinical reports, or a **vision model** inspecting a production line, I ask the same three questions: *what is the model actually using, which choices really matter, and would the result survive a fresh test?* That thread connects my work across **explainable AI, LLMs, RAG, NLP, computer vision, and medical imaging**.

> 🎯 **Seeking:** a **PhD position starting Fall 2027** in AI (XAI, LLMs, RAG, NLP, multimodal, or applied AI). Also open to a 6-month research internship from **January 2027**.

---

## ⚡ At a Glance

| Area | Highlight |
|---|---|
| 📄 **Research** | Independent single-author paper on VLM interpretability, published on Zenodo with full code |
| 🧪 **Evaluation** | 749-run golden-dataset harness proving a small LLM matches a frontier model at ~7x lower cost |
| 🏭 **Real impact** | Return rate 6.8% → 0.2% · food waste -55% · reporting time -30% · labelling work -70% |
| 🌍 **International** | Industry work for teams in Germany 🇩🇪 and France 🇫🇷 |
| 👨‍🏫 **Teaching** | Founded DeepFlow: 20+ AI workshops for 200+ students |
| 🏆 **Awards** | Mutualhack 3.0 winner · 2nd place Insight for Impact |

---

## 🔍 Research Interests

- **Explainable & interpretable AI:** what really happens inside LLMs and VLMs, using causal methods (attention knockout, information flow, representation analysis).
- **LLM reliability, RAG & NLP:** hallucination, faithfulness, grounding, and evaluation methodology (golden datasets, LLM-as-judge, ablations).
- **Multimodal & agentic systems:** models and multi-agent architectures that combine vision, language, and structured reasoning.
- **Applied AI with real stakes:** healthcare, industry, and regulated domains where errors cost something.

---

## 📄 Papers

> All papers and code are open. Full list on [ORCID](https://orcid.org/0009-0007-2027-2520). More in progress.

| Year | Title | Topic | Links |
|------|-------|-------|-------|
| 2026 | **Medical Fine-Tuning Changes Answer Commitment and Information Flow in a Vision-Language Model: A Split-Sample Study on VQA-RAD** <br> *Houssem Eddine (single author)* | XAI · VLMs · Interpretability | [![Paper](https://img.shields.io/badge/Paper-Zenodo-1682D4?logo=zenodo&logoColor=white)](https://zenodo.org/records/23766104) [![Code](https://img.shields.io/badge/Code-GitHub-181717?logo=github)](https://github.com/HoussemDs/vlm-attention-knockout) |

<details>
<summary><b>📌 Paper summary: what fine-tuning changes inside a vision-language model</b></summary>
<br>

- **Question:** when a general VLM is fine-tuned for a domain, does it start relying more on the image and less on the question text?
- **Method:** per-layer causal attention knockout (image→answer and question→answer) on Gemma-3-4B vs. its fine-tune MedGemma-4B, under a written protocol with a discovery split (n=100) and a held-out confirmation split (n=150).
- **Result:** the pre-specified primary test confirms: median question-dominance ratio 5.36 → 4.15 (p=0.006). 4 of 5 discovery effects replicate. One effect that looked strong on discovery fails to replicate and is reported honestly as a null.
- **Next:** the vision encoder changes sharply (CKA 0.155), so an encoder-swap experiment is planned to separate encoder from decoder effects.
- **Compute:** run entirely on free Kaggle GPUs, fully reproducible.

</details>

---

## 🧭 What I Want to Work On Next

- **Inside the model:** causal interpretability for LLMs and VLMs. Which layers and components actually drive an answer?
- **Trustworthy LLMs & RAG:** detecting when a model answers from prior knowledge instead of the evidence it was given.
- **Better evaluation:** protocols that separate real improvements from noise, for any AI system.

---

## 🌟 Research & Engineering Highlights

**🔬 Causal interpretability of vision-language models** (paper above)
Turned attention-knockout probing into a before/after measurement instrument with built-in replication. Architecture-agnostic, works on any HuggingFace VLM, no retraining.

**📚 Evaluation-driven RAG reliability** | Alight Consulting, Germany
*Question:* can a lightweight LLM match a frontier model on grounded question answering, and how do you prove it? Built a golden-dataset harness (factual, analytical, refusal, access-control) scored by an LLM-as-judge rubric, with controlled ablations (HyDE on/off, compression sweeps) over **749 graded runs across 10 configurations**. *Finding:* a small model reached frontier-level quality (**96.8% pass**) at **~7x lower cost**.

**🫀 Clinically validated 3D segmentation** | Alight Consulting, Germany
3D cardiac MRI segmentation (MONAI) validated by a blinded study with 2 senior cardiologists across 40 cases: **Dice 0.88 to 0.91**, clinically acceptable in **95%+** of cases.

---

## 🛠️ Selected Projects

| Project | What it does |
|---------|--------------|
| 🔬 **[VLM Attention Knockout](https://github.com/HoussemDs/vlm-attention-knockout)** | Per-layer causal probing for any HuggingFace VLM via PyTorch hooks. Code for my paper. |
| 🏗️ **Document AI RAG Platform** | Production Azure RAG: hybrid BM25 + vector retrieval with RRF, adaptive HyDE routing, document-level access control, prompt compression, inline PDF citations. |
| 🤖 **[OpportuNet](https://github.com/HoussemDs/OpportuNet)** | 7-agent LLM orchestration: parallel execution, scam detection, opportunity scoring, auto-reply drafting. |
| 📊 **B2B Lead Intelligence Engine** | Agentic system over EU procurement data, company registries and bilingual NLP signals, multi-LLM orchestration, live dashboard. |
| 🏭 **YOLOv8 Visual QC** | Real-time defect detection on an automotive assembly line. Return rate **6.8% → 0.2%** in 30 days. |

---

## 💼 Experience

### AI Engineer | Alight Consulting GmbH (Remote, Germany) | Jun 2026 to Present
`Azure AI Search · Azure OpenAI · Document Intelligence · FastAPI · Next.js · LLMLingua`
- Architected a production RAG platform: 4-stage ingestion, hybrid BM25 + HNSW retrieval with Reciprocal Rank Fusion, adaptive HyDE routing (faithfulness 4.96/5).
- Index-level access control validated at **100% compliance**, zero leakage across 31 cases and 7 group configurations.
- Evaluation harness (749 runs, 10 configs): chose a model matching gpt-4.1 quality at **~7x lower cost**, cost-modeled to ~$496/mo at 500 users.
- Full-stack app with multi-turn conversation and a PDF viewer that opens on the exact cited page.

### AI Engineer | SBT Tunisia | Jan to Aug 2026
`YOLOv8 · OpenCV · LangChain · LangGraph · FastAPI · Playwright · A2A · MCP`
- **Computer vision:** mobile CV pipeline on a wiring harness line cut return rate from **6.8% to 0.2%** in 30 days.
- **Agentic GTM (freelance):** delivered a one-click lead intelligence app; a two-hop channel graph turned 400+ targets into ~10 high-leverage contacts.

### AI Engineer, Apprenticeship | Recordati / Opalia | May to Jun 2026
- Built **GreenOPS AI**, a human-in-the-loop energy optimization system for a pharmaceutical plant. **2nd place**, Insight for Impact.

### AI Engineer, Internship | Alight Consulting GmbH (Remote, Germany) | Jun to Sep 2025
`MONAI · PyTorch · SFT + DPO · ONNX`
- 3D segmentation pipeline: Dice **0.88 to 0.91**, **18%** over baseline, clinically validated.
- Fine-tuned an LLM (SFT + DPO) on 200+ expert-reviewed reports: reporting time **-30%**, hallucination rate **-35%**.

### Computer Vision Engineer, Contract | CMA CGM, France | Jan to Jun 2025
- **92.4% IoU** on multimodal satellite imagery, **70%** less manual labelling, **31%** better generalisation to unseen terrain.
- CrewAI multi-agent reporting: ~10 hours of weekly work down to ~20 minutes.

### Founder | AI-Powered Retail | May 2023 to Present
- Forecasting error (MAPE) **48% → 12%**, unsold inventory **-42%**, VLM-based product analysis **+20%** conversion.

### Data Analyst | Newrest, Tunisia | Jun to Sep 2023
- Promoted from intern to full-time in one month after a model cut food waste by **55%**.

---

## 🧰 Tech Stack

<p>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white"/>
<img src="https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black"/>
<img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white"/>
<img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white"/>
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white"/>
<img src="https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white"/>
<img src="https://img.shields.io/badge/Azure-0078D4?style=flat-square&logo=microsoftazure&logoColor=white"/>
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
<img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white"/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
<img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white"/>
</p>

**XAI & Evaluation:** attention knockout · information flow · GradCAM · CKA · ablation design · LLM-as-judge · pre-specified testing
**LLMs, RAG & NLP:** LangChain · LangGraph · CrewAI · hybrid retrieval · HyDE · LLMLingua · SFT + DPO · A2A · MCP
**Vision & Imaging:** YOLOv8 · U-Net · MONAI · SimpleITK · DICOM · 3D Slicer

---

## 🎓 Education

**Diplôme d'Ingénieur, Computer Science (AI Specialisation)** | ESPRIT University | 2022 to 2027
Master's-level degree (EQF Level 7). GPA: 15/20 (French scale), approximately 3.7 / 4.0.

---

## 👨‍🏫 Teaching & Leadership

**Founder & Tech Manager** | DeepFlow | Jun 2023 to Present
AI education initiative: 20+ workshops (deep learning, LLMs, medical imaging) for 200+ engineering students; mentored 24 hackathon competitors.

---

## 🏆 Recognition

| Event | Result |
|-------|--------|
| **Mutualhack 3.0** | 🥇 Winner, HANEN (AI voice companion for the elderly), MAZAM incubation |
| **Insight for Impact** (ESPRIT × Recordati) | 🥈 2nd place, GreenOPS AI |
| **European Agentic AI Bootcamp** | Participant, Jul 2025 |

---

## 🗣️ Languages

| Language | Level |
|----------|-------|
| 🇬🇧 English | Fluent (C1/C2), primary working language |
| 🇸🇦 Arabic | Native |
| 🇫🇷 French | Professional working proficiency |
| 🇩🇪 German | A2 / B1 (actively learning) |

---

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect_with_me-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=0077B5)](https://linkedin.com/in/houssemeddineds)
[![Email](https://img.shields.io/badge/Email-Drop_a_message-D14836?style=for-the-badge&logo=gmail&logoColor=white&labelColor=D14836)](mailto:houssemeddineds@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit_site-D6C2A1?style=for-the-badge&logo=google-chrome&logoColor=black&labelColor=D6C2A1)](https://houssemds.github.io)

</div>

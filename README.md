<div align="center">

# Houssem Eddine Ghribi

### AI Engineer & Researcher | Trustworthy AI · Multimodal & Agentic Systems · Medical AI

<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=26&pause=1200&color=2E9EF7&center=true&vCenter=true&width=720&lines=Production+AI+for+the+Real+World;LLMs+%7C+Vision+%7C+Agents+%7C+Clinical+AI;Seeking+PFE+2027+%2B+PhD+%C2%B7+Relocation-Ready" alt="Typing SVG" />

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/houssemeddineds)
[![Email](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:houssemeddineds@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-D6C2A1?style=for-the-badge&logo=google-chrome&logoColor=black)](https://houssemds.github.io)

</div>

---

## Overview

Final-year AI engineering student at ESPRIT University (graduating 2027). I work on **trustworthy, evaluable AI**: building systems and then measuring whether they actually hold up, through ablation studies, golden-dataset evaluation, and clinical validation rather than demos. My work spans retrieval and LLM reliability, multimodal and multi-agent reasoning, and medical imaging.

What draws me to research is the part after the model runs: designing the protocol that tells you whether it is really working. A segmentation model checked by blinded cardiologists, a retrieval system stress-tested across 749 graded runs and controlled ablations, a multi-agent clinical pipeline built for explainability and traceable outputs. I care about the evaluation as much as the architecture.

**Seeking:** a research-oriented final placement (**PFE**) from **January 2027** that can continue into a **PhD** with the same group, ideally on the same topic. Relocation-ready and open to opportunities internationally (currently in Tunisia).

> Much of my strongest work is proprietary, built for companies under NDA. What is shown here is a representative sample; deeper walkthroughs, methodology, and demos are available on request.

---

## Research Interests

- **Trustworthy and evaluable AI:** hallucination, faithfulness, and evaluation methodology for LLM and VLM systems (golden datasets, LLM-as-judge rubrics, ablation studies).
- **Multimodal and agentic systems:** retrieval-augmented and multi-agent architectures that combine vision, language, and structured reasoning.
- **Medical and clinical AI:** segmentation, diagnostic support, and explainable, regulatory-aware models validated with clinicians.

I read broadly and apply widely: the three themes above overlap more than they separate, and I am comfortable moving between them.

---

## Research Highlights

**Evaluation-driven RAG reliability** — Alight Consulting
*Question:* can a lightweight model match a frontier model on grounded question answering, and how do you actually prove it? I built a golden-dataset harness (factual, analytical, refusal, and access-control categories) scored by an LLM-as-judge rubric, and ran controlled ablations (HyDE on/off, compression keep-rate sweeps) over 749 graded runs across 10 configurations. *Finding:* a small model reached frontier-level quality (96.8% pass) at roughly 7x lower cost, with grounding and citation validity verified across the set and the faithfulness-versus-latency tradeoff of each design choice measured rather than assumed.

**Multi-agent clinical reasoning for brain MRI** — co-authored, under review at KES 2026
*Approach:* a multi-agent architecture coupling case retrieval (MedViT embeddings + FAISS), tumor segmentation (U-Net / ResNet encoder), LLM-based explainability, and structured report generation, alongside a parallel multimodal virtual-consultation pipeline for symptom reasoning. *Emphasis:* explainability and traceable, structured clinical outputs (JSON / PDF) over a single black-box prediction.

**Clinical validation of 3D cardiac segmentation** — Alight Consulting
*Study design:* trained a multi-class 3D cardiac MRI segmentation model (MONAI, ACDC dataset) and validated it with a blinded preference study, 2 senior cardiologists across 40 cases. *Result:* Dice 0.88 to 0.91 (18% over the 3D U-Net baseline), rated clinically acceptable in 95%+ of cases, with EU MDR / IVDR technical documentation and GradCAM explainability for regulatory traceability.

---

## Publications & Academic Research

- **Multi-Agent VLM Pipeline for Brain Tumor Analysis** (co-author). Under review at KES 2026, revisions submitted.
- **Multi-Modal Brain Safety and Mental Health Assessment.** ESPRIT research project (Sep to Dec 2025): brain MRI, video, and sensor fusion with an agentic interview system that surfaces assessments for clinician review.

---

## Selected Engineering Projects

| Project | What it does |
|---------|--------------|
| 🏗️ **Document AI RAG Platform** | Production Azure RAG for regulated document workflows. Hybrid BM25 + HNSW retrieval with RRF, adaptive HyDE query routing, index-level RBAC, LLMLingua-2 compression, inline PDF citation viewer. Deployed end to end and cost-modeled to production scale. |
| 🏭 **YOLOv8 Visual QC** | Real-time defect detection on automotive wiring harnesses. Return rate cut from **6.8% to 0.2%** within 30 days, mobile pipeline on the assembly line. |
| 📊 **B2B Lead Intelligence Engine** | Agentic GTM system: TED procurement API + French NAF registry + bilingual signal queries, two-hop channel graph, multi-LLM orchestration, live dashboard. |

---

## Work Experience

### AI Engineer | Alight Consulting GmbH (Remote) | Jun 2026 to Present
`Azure AI Search · Document Intelligence · Azure OpenAI · FastAPI · Next.js · LLMLingua · Entra ID`

- Architected a production Document AI RAG platform on Azure: 4-stage ingestion, hybrid BM25 + HNSW retrieval with Reciprocal Rank Fusion, and an adaptive router applying HyDE only to complex analytical queries (faithfulness 4.96/5 vs 4.91).
- Engineered server-side RBAC using OData filters at the index level for document-level access control, validated at 100% compliance with zero cross-group leakage across 31 cases under all 7 group configurations.
- Built a golden-dataset evaluation harness (749 graded runs, 10 configurations): 96.8% pass rate, selected a lightweight model matching gpt-4.1 quality at ~7x lower cost per query, trimmed further with LLMLingua-2 at zero quality loss, cost-modeled to ~$496/mo at 500-user scale.
- Built the full-stack app: FastAPI backend with multi-turn conversation and automatic follow-up rewriting, Next.js + TypeScript frontend with an inline PDF viewer that opens to the exact cited source page.

### AI Engineer | SBT Tunisia | Jan to Aug 2026
`YOLOv8 · OpenCV · LangChain · LangGraph · Flask · FastAPI · SQLite · Playwright · Katana · A2A · MCP Server`

Computer vision contract followed by a freelance GTM build for the same client, delivered as a standalone app.

**Computer Vision (contract, Jan to Jun 2026)**
- Reduced client return rate from **6.8% to 0.2%** within 30 days on an automotive wiring harness assembly line via a mobile CV pipeline validating cable routing, colour sequencing, and configuration compliance.
- Integrated A2A communication and an MCP Server for automated production reporting and database connectivity.

**AI GTM Engineering (freelance, Jun to Aug 2026)**
- Built and delivered a fully automated agentic B2B lead intelligence engine as a self-contained app: one click runs the pipeline and launches the interface. Sources EU procurement (TED API), bilingual signal queries (French / Italian), and the French national company registry (NAF-filtered firmographics), with multi-provider LLM orchestration at near-zero cost.
- Engineered a two-hop channel graph turning 400+ individual targets into ~10 referencing bodies each covering 20 to 36 distributors.
- Delivered a live streaming dashboard with ranked call-lists, one-click actions, CSV export, and pipeline status tracking, handed off to the client as a working product.

### AI Engineer, Apprenticeship | Recordati / Opalia | May to Jun 2026
`Agentic AI · Energy Optimization · GMP Compliance`

- Built **GreenOPS AI**, an energy optimization system for a live pharmaceutical manufacturing plant. Placed **2nd at Insight for Impact** (2,000 TND prize).
- Designed a human-in-the-loop AI architecture for industrial energy decisions, prioritizing operator trust and auditability over full automation.

### Medical AI Engineer, Internship | Alight Consulting GmbH (Remote) | Jun to Sep 2025
`MONAI 3D · PyTorch · LangChain · SFT + DPO · DICOM · SimpleITK · ONNX`

- Built a production-grade multi-class 3D cardiac segmentation pipeline (LV, RV, myocardium) on the ACDC dataset: Dice **0.88 to 0.91**, HD95 3.0 to 5.0 mm, 18% improvement over the 3D U-Net baseline.
- Blinded preference study with 2 senior cardiologists across 40 cases: outputs rated clinically acceptable in **95%+** of cases across all three cardiac structures, exported to ONNX and validated in OHIF Viewer and 3D Slicer for radiologist sign-off.
- Fine-tuned a clinical LLM (SFT + DPO) on 200+ physician-reviewed reports, cutting per-study reporting time by **30%** and hallucination rate by **35%** (held-out set, scored by two independent cardiologists). Produced EU MDR / IVDR-aligned technical documentation with GradCAM explainability maps.

### Geospatial AI Engineer, Contract | CMA CGM, France | Jan to Jun 2025
`U-Net · PyTorch · CrewAI · Docker · Multimodal Satellite Imagery`

- Achieved **92.4% IoU** on multimodal satellite imagery for environmental planning and reforestation site selection, 8% above baseline, eliminating **70%** of manual labelling workload (validated on 150+ reference tiles). Fine-tuned for desert terrain: **31%** improvement in generalisation to unseen geographies.
- Architected a CrewAI multi-agent system reducing weekly analysis and reporting from ~10 hours to ~20 minutes of validation.

### Solo Founder | AI-Powered Retail (personal small business) | May 2023 to Present
`PyTorch · Prophet · Scikit-Learn · LangChain · VLM · OpenCV · Facebook Graph API`

- Demand forecasting on 90-day rolling sales data: reduced forecast error (MAPE) from **48% to 12%**, cutting unsold inventory by **42%**.
- VLM-based customer / product analysis (**+20%** sales conversion) plus social media trend detection identifying emerging fashion trends 10 to 12 days ahead of peak demand.

### Data Analyst | Newrest, Tunisia | Jun to Sep 2023
`Python · Pandas · Scikit-Learn · Forecasting`

- Promoted from intern to full-time within one month after delivering a forecasting model that reduced food waste by **55%** at airport retail shops. Automated inventory forecasting cut processing time from days to under a second.

---

## Tech Stack

**AI / ML:** Python · PyTorch · TensorFlow · Scikit-Learn · ONNX

**Medical Imaging:** MONAI · SimpleITK · OpenCV · NiBabel · DICOM · 3D Slicer · OHIF Viewer

**Agentic AI & LLMs:** LangChain · LangGraph · CrewAI · OpenAI · Groq · A2A Protocol · MCP Server

**Cloud & Infra:** Microsoft Azure · Azure AI Search · Azure OpenAI · Azure Document Intelligence · Docker · Git

**Web & Backend:** FastAPI · Flask · Next.js · TypeScript · SQLite

---

## Education

**Diplôme d'Ingénieur, Computer Science (AI Specialisation)** | ESPRIT University | 2022 to 2027
GPA: 15/20 (French scale), approximately 3.7 / 4.0.

---

## Leadership & Teaching

**Tech Manager & Mentor** | DeepFlow | Jun 2023 to Present
Founded and run an AI education initiative. Delivered 20+ AI / ML workshops (medical imaging, clinical AI, core deep learning) to 200+ engineering students, and mentored 24 competitors through a hackathon.

---

## Recognition

| Event | Result |
|-------|--------|
| **Insight for Impact** (ESPRIT × Recordati) | 🥈 2nd place, GreenOPS AI (2,000 TND) |
| **Mutualhack 3.0** | 🥇 Winner, HANEN (AI voice companion for elderly), MAZAM incubation |
| **European Agentic AI Bootcamp** | Participant, Jul 2025 |

---

## Languages

| Language | Level |
|----------|-------|
| 🇸🇦 Arabic | Native |
| 🇬🇧 English | C1 Advanced |
| 🇫🇷 French | C1 Advanced |
| 🇩🇪 German | A2 / B1 (actively learning) |

---

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect_with_me-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=0077B5)](https://linkedin.com/in/houssemeddineds)
[![Email](https://img.shields.io/badge/Email-Drop_a_message-D14836?style=for-the-badge&logo=gmail&logoColor=white&labelColor=D14836)](mailto:houssemeddineds@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit_site-D6C2A1?style=for-the-badge&logo=google-chrome&logoColor=black&labelColor=D6C2A1)](https://houssemds.github.io)

</div>

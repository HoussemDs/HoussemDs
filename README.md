<div align="center">

# Houssem Eddine Ghribi

### AI Engineer | Medical Imaging | Production LLM Systems

<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=26&pause=1200&color=2E9EF7&center=true&vCenter=true&width=720&lines=Document+AI+%7C+Computer+Vision+%7C+Clinical+AI;Building+Production+AI+for+the+Real+World" alt="Typing SVG" />

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/houssemeddineds)
[![Email](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:houssemeddineds@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-D6C2A1?style=for-the-badge&logo=google-chrome&logoColor=black)](https://houssemds.github.io)

</div>

---

## Overview

I build AI systems where accuracy has real-world stakes: medical diagnoses, manufacturing quality, regulated documents. Recent work: 3D cardiac MRI segmentation validated by cardiologists, a defect-detection pipeline that took an automotive line from **6.8% to 0.2%** return rate, and a production Document AI RAG platform on Azure with document-level RBAC.

**Currently:** AI Engineer at Alight Consulting GmbH (remote), building a production Document AI RAG platform on Microsoft Azure.

**Seeking:** 6-month engineering final placement (**PFE**) starting **January 2027**. Focus: healthcare AI, clinical decision support, diagnostic imaging, or applied LLM systems.

**Based in:** Tunis. Open to remote or relocation.

---

## Publications

| Paper | Venue | Links |
|-------|-------|-------|
| **Multi-Agent VLM Pipeline for Brain Tumor Analysis** | KES 2026 (revisions submitted) | [Preprint](https://doi.org/10.17605/OSF.IO/F5QX3) |

---

## Featured Projects

| Project | What it does |
|---------|--------------|
| 🏗️ **Document AI RAG Platform** | Production Azure RAG for regulated document workflows. Hybrid BM25 + semantic retrieval with RRF, HyDE query expansion, index-level RBAC, LLMLingua compression (2 to 4x prompt token reduction), inline PDF citation viewer. |
| 🫀 **Cardiac Segmentation (ACDC)** | 3D cardiac MRI with MONAI. Dice **0.88 to 0.91**, 18% over U-Net baseline. Blinded cardiologist validation rated outputs clinically acceptable in **95%+** of cases. |
| 🧠 **Multi-Agent Brain Tumor Pipeline** | KES 2026 submission. MedViT embeddings, FAISS retrieval, U-Net segmentation, GradCAM XAI, LLaMA 70B report generation. |
| 📊 **B2B Lead Intelligence Engine** | Agentic GTM system: TED procurement API + French NAF registry + bilingual signal queries, two-hop channel graph, multi-LLM orchestration, live dashboard. |
| 🏭 **YOLOv8 Visual QC** | Real-time defect detection on automotive wiring harnesses. Return rate cut from **6.8% to 0.2%** within 30 days, mobile pipeline on the assembly line. |

---

## Work Experience

### AI Engineer | Alight Consulting GmbH (Remote) | Jun 2026 to Present
`Azure AI Search · Document Intelligence · Azure OpenAI · FastAPI · Next.js · LLMLingua · Entra ID`

- Architected a production Document AI RAG platform on Azure: 4-stage ingestion, hybrid BM25 + semantic retrieval with Reciprocal Rank Fusion, HyDE-augmented query expansion.
- Engineered server-side RBAC using OData filters at the index level for strict document-level access control with zero cross-group data exposure.
- Integrated LLMLingua context compression (**2 to 4x** prompt token reduction). Built full-stack app with multi-turn conversation, automatic follow-up rewriting, and an inline PDF viewer that opens to the exact cited source page.

### AI Engineer | SBT Tunisia | Jan 2026 to Present
`YOLOv8 · OpenCV · LangChain · LangGraph · Flask · FastAPI · SQLite · Playwright · Katana · A2A · MCP Server`

Started as a computer vision contract, continued as a freelance engagement building agentic GTM tooling for the same client.

**Computer Vision (contract, Jan to Jun 2026)**
- Reduced client return rate from **6.8% to 0.2%** within 30 days on an automotive wiring harness assembly line via a mobile CV pipeline validating cable routing, colour sequencing, and configuration compliance.
- Integrated A2A communication and an MCP Server for automated production reporting and database connectivity.

**AI GTM Engineering (freelance, Jun 2026 to Present)**
- Built a fully automated agentic B2B lead intelligence engine over EU procurement (TED API), bilingual signal queries (French / Italian), and the French national company registry (NAF-filtered firmographics), with multi-provider LLM orchestration running at near-zero cost.
- Engineered a two-hop channel graph turning 400+ individual targets into ~10 referencing bodies each covering 20 to 36 distributors.
- Delivered a live streaming dashboard with ranked call-lists, one-click actions, CSV export, and pipeline status tracking.

### AI Engineer, Apprenticeship | Recordati / Opalia | May to Jun 2026
`Agentic AI · Energy Optimization · GMP Compliance`

- Built **GreenOPS AI**, an energy optimization system for a live pharmaceutical manufacturing plant. Placed **2nd at Insight for Impact** (2,000 TND prize).
- Designed a human-in-the-loop AI architecture for industrial energy decisions, prioritizing operator trust and auditability over full automation.

### Medical AI Engineer, Internship | Alight Consulting GmbH (Remote) | Jun to Sep 2025
`MONAI 3D · PyTorch · LangChain · SFT + DPO · DICOM · SimpleITK · ONNX`

- Built a 3D cardiac segmentation pipeline on the ACDC dataset: Dice **0.88 to 0.91**, HD95 3.0 to 5.0 mm, 18% improvement over U-Net baseline.
- Blinded preference study with 2 senior cardiologists across 40 cases: outputs rated clinically acceptable in **95%+** of cases across all three cardiac structures.
- Fine-tuned a clinical LLM (SFT + DPO) on 200+ physician-reviewed reports, cutting per-study reporting time by **30%** and hallucination rate by **35%**. Produced EU MDR / IVDR-aligned technical documentation with GradCAM explainability maps.

### Geospatial AI Engineer, Contract | CMA CGM, France | Jan to Jun 2025
`U-Net · PyTorch · CrewAI · Docker · Multimodal Satellite Imagery`

- Achieved **92.4% IoU** on multimodal satellite imagery, 8% above baseline, eliminating **70%** of manual labelling workload. Fine-tuned for desert terrain: **31%** improvement in generalisation to unseen geographies.
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

**Medical Imaging:** MONAI · SimpleITK · OpenCV · NiBabel · DICOM · 3D Slicer

**Agentic AI & LLMs:** LangChain · LangGraph · CrewAI · OpenAI · Groq · A2A Protocol · MCP Server

**Cloud & Infra:** Microsoft Azure · Azure AI Search · Azure OpenAI · Azure Document Intelligence · Docker · Git

**Web & Backend:** FastAPI · Flask · Next.js · TypeScript · SQLite

---

## Education

**Diplôme d'Ingénieur, Computer Science (AI Specialisation)** | ESPRIT University | 2022 to 2027
GPA: 15/20 (French scale), approximately 3.7 / 4.0.

**Tech Manager & Mentor** | DeepFlow | Jun 2023 to Present
20+ AI / ML workshops on medical imaging and clinical AI to 200+ engineering students. Mentored 24 hackathon competitors.

**Research: Multi-Modal Brain Safety & Mental Health Assessment** | ESPRIT × Research Dept | Sep to Dec 2025
Autonomous pipeline combining brain MRI, video, and sensor data with an agentic patient interview system flagging clinical assessments to a remote clinician.

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
| 🇫🇷 French | B2 Upper-Intermediate |
| 🇩🇪 German | A2 to B1 (actively learning) |

---

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect_with_me-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=0077B5)](https://linkedin.com/in/houssemeddineds)
[![Email](https://img.shields.io/badge/Email-Drop_a_message-D14836?style=for-the-badge&logo=gmail&logoColor=white&labelColor=D14836)](mailto:houssemeddineds@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit_site-D6C2A1?style=for-the-badge&logo=google-chrome&logoColor=black&labelColor=D6C2A1)](https://houssemds.github.io)

</div>

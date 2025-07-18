# 🧠 Mock’n-Hire: AI System for Resume Screening and Emotion-Aware Interview Feedback

[![ICCCNT 2025 Accepted](https://img.shields.io/badge/ICCCNT--2025-Accepted-blue)](https://icccnt2025.org)
[![Python](https://img.shields.io/badge/Python-3.10-blue.svg)](https://www.python.org/)
[![LangChain](https://img.shields.io/badge/LangChain-Enabled-success)](https://www.langchain.com/)
[![Deployment](https://img.shields.io/badge/Deployment-Vercel-green)](https://vercel.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 🚀 Overview

**Mock’n-Hire** is a **Generative AI-powered recruitment platform** that seamlessly integrates:

- ⚙️ Automated Resume Screening using Transformer-based embeddings  
- 🎤 Emotion-Aware Mock Interviews with real-time video-based stress detection  
- 🧠 Personalized Question Generation using LLMs  
- ☁️ Scalable backend via **FastAPI** + **Supabase**  
- 📊 Real-time analytics and user feedback loop  

> 📌 Presented at **IEEE ICCCNT 2025**. This project transforms candidate evaluation by combining **technical screening** with **emotional intelligence**.

---

## 🔍 Key Features

| Feature                            | Description                                                                 |
|-----------------------------------|-----------------------------------------------------------------------------|
| 📝 Resume Screening                | PDF parsing, BERT-style embeddings, recruiter-defined scoring              |
| 🎯 Semantic Matching              | Uses **SentenceTransformers** + weighted cosine similarity                  |
| 💬 Personalized Mock Interviews   | Role-specific questions from LLMs using **LangChain**                      |
| 🎥 Emotion Detection              | Video analysis using **MobileNetV2** + **FER-2013** dataset                 |
| 🔐 Authentication                 | Supabase Auth (email, OAuth, token-based)                                  |
| 🌐 Cloud Deployment               | Hosted on **Vercel** with CI/CD support                                    |
| 📊 Feedback & Reports             | Candidate stress report, dashboard views for recruiters                    |

---

## 🧠 Tech Stack

| Layer         | Technology Used                            |
|---------------|--------------------------------------------|
| 💡 Generative AI | Mistral-8x7B, LangChain, Transformers         |
| 🧾 NLP         | SentenceTransformers, HuggingFace            |
| 🖼️ CV Model     | MobileNetV2, OpenCV, FER-2013                |
| ⚙️ Backend      | FastAPI, LangChain Chains, RESTful APIs       |
| 🗃️ Database     | Supabase (PostgreSQL + Storage + Auth)       |
| 💻 Frontend     | React + Tailwind CSS (UI v2 in progress)     |
| ☁️ Deployment   | Vercel (Frontend) + Railway/Render (API)     |

---

## 📁 Folder Structure

```bash
mock-n-hire/
├── backend/                 # FastAPI backend with AI modules
│   ├── routes/             # Resume, Interview, Feedback APIs
│   ├── models/             # Transformer & Emotion models
│   └── utils/              # Preprocessing, similarity, analysis
├── frontend/                # React frontend with Dashboards
│   └── components/         # UI pages (recruiter, candidate)
├── notebooks/               # Jupyter prototypes for training
├── data/                    # FER-2013 and anonymized resumes
├── langchain_chains/        # LangChain prompt logic
└── README.md
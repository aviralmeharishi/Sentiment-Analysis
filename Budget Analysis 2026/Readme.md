# **📊 Indian Union Budget 2026-27: AI & Sentiment Analysis**

> **An Industrial-Grade NLP & Generative AI Project** analyzing the authentic Indian Union Budget Speech to extract underlying themes, sentiments, and sector-wise allocations.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python)
![NLP](https://img.shields.io/badge/NLP-NLTK%20%7C%20TextBlob-orange?style=for-the-badge)
![GenAI](https://img.shields.io/badge/GenAI-Ollama%20%7C%20Gemini-brightgreen?style=for-the-badge)
![Stats](https://img.shields.io/badge/Stats-SciPy-yellow?style=for-the-badge)
![License](https://img.shields.io/badge/License-Apache-purple?style=for-the-badge)

---

## 📖 Overview
The Union Budget of India is the most highly anticipated economic event of the year. This project bypasses media interpretations and leverages **Natural Language Processing (NLP)** and **Large Language Models (LLMs)** to analyze the raw, authentic Parliamentary text directly from the official government portal.

It systematically processes the speech to identify emotional trajectories (Sentiment Analysis), most emphasized sectors (Thematic EDA), and utilizes both **local and cloud-based LLMs** for a precise breakdown of Government Revenue and Expenditure.

---

## ✨ Key Features
- **🌍 Automated Ingestion:** Live extraction of the authentic `.docx` speech from the official `indiabudget.gov.in` portal.
- **🧹 Text Preprocessing:** Custom stopword removal (filtering financial terms like 'crore', 'lakhs'), tokenization, and text normalization using NLTK.
- **📈 Exploratory Data Analysis (EDA):** WordClouds, N-gram frequency analysis, and custom sector-focus mapping (Agriculture, Defence, Tech, etc.) visualized via Seaborn and Matplotlib.
- **🧠 Statistical Sentiment Analysis:** Polarity tracking across the document utilizing TextBlob, strictly validated by an **Independent T-Test** to map tone shifts between the first and second half of the speech.
- **🤖 Multi-LLM Deep Dive:** Advanced prompt engineering evaluated via:
  - **Local LLMs (Ollama):** Phi-3, Llama 3.1, Qwen 2
  - **Cloud APIs:** Google Gemini 3.5 Flash
  - Generates structured Markdown tables for *Sector-Wise Allocations*, *Revenue Model ("Rupee Comes From")*, and *Expenditure Model ("Rupee Goes To")*.

---

## 🛠️ Tech Stack & Libraries

| Category | Tools & Libraries |
| --- | --- |
| **Data Gathering** | `requests`, `python-docx` |
| **Data Manipulation & Stats** | `pandas`, `numpy`, `scipy` |
| **Natural Language Processing** | `nltk`, `textblob` |
| **Visualizations** | `matplotlib`, `seaborn`, `wordcloud` |
| **Generative AI** | `ollama` (Local), `google-genai` (Cloud) |
| **Environment & Config** | `python-dotenv` |

---

## 📂 Project Structure
```text
📦 budget-ai-analysis
 ┣ 📜 BudgetAnalysis.ipynb     # Main Jupyter Notebook containing full pipeline
 ┣ 📜 requirements.txt         # Project dependencies
 ┣ 📜 Budget_Speech.docx       # Exclusive Speech of FM Nirmala Sitaraman
 ┣ 📜 Summary.md               # Summary of analysis
 ┣ 📜 Disclaimer.md            # Disclaimer regarding this Analysis
 ┣ 📜 README.md                # Project documentation

# 📊 Indian Union Budget: AI & Sentiment Analysis

An industrial-grade Natural Language Processing and Generative AI pipeline analyzing authentic Parliamentary transcripts to decode national economic priorities, policy sentiment, and fiscal models.

`Python 3.10+` · `NLTK & TextBlob` · `Ollama (Local SLMs)` · `Google Gemini 3.5` · `SciPy T-Test` · `Apache 2.0 License`

---

## 📖 Executive Summary

The **Union Budget of India** is the most consequential economic event of the fiscal year. While financial news cycles often condense the announcement into brief soundbites, the authentic 35-to-40 page address delivered by the Hon'ble Finance Minister contains the foundational blueprint for India's macroeconomic trajectory.

This project bypasses secondary interpretations by deploying an **end-to-end data science and text-mining pipeline** directly on verbatim Parliamentary transcripts. Through paragraph-level sentiment modeling, statistical hypothesis testing, and multi-LLM comparative synthesis, unstructured legislative text is transformed into empirical economic intelligence.

---

## 🏗️ Architecture & Pipeline

```text
  Authentic Parliamentary Speech (.docx / .pdf)
                       │
                       ▼
         Text Preprocessing & Normalization
         (Regex Tokenization · Financial Stopwords)
                       │
        ┌──────────────┴──────────────┐
        ▼                             ▼
   Thematic EDA             Sentiment Trajectory
  • High-Frequency Vocab     • Paragraph Polarity Scoring
  • Bigram Collocations      • Two-Sample T-Test (Part A vs B)
  • 10-Sector Focus Matrix
        │                             │
        └──────────────┬──────────────┘
                       │
                       ▼
           Multi-LLM Policy Synthesis
         • Local SLMs: Phi-3, Llama 3.1, Qwen 2
         • Cloud API: Google Gemini 3.5 Flash
                       │
                       ▼
     Structured Accounting Breakdown (Markdown)
   [Sector Allocations · Rupee Inflows · Rupee Outflows]
```

---

## ✨ Core Highlights

* **Automated Data Retrieval:** Direct programmatic extraction of authentic parliamentary speeches from the official `indiabudget.gov.in` portal.
* **Financial Domain Normalization:** Custom stopword engine removing parliamentary boilerplate and currency markers (`crore`, `lakh`, `rupees`, `hon'ble`, `speaker`) to isolate substantive policy themes.
* **Thematic Text Mining:** WordClouds, frequency rankings, and bigram co-occurrence networks mapping the administration's lexical emphasis.
* **10-Sector Focus Matrix:** Automated keyword tracking across critical national verticals including *Agriculture, Health, Education, Railways, Technology & AI, Defence, Nari Shakti, Youth, MSME, and Infrastructure*.
* **Empirical Tone Trajectory:** Continuous sentiment tracking across 400+ paragraphs using TextBlob polarity metrics.
* **Hypothesis Testing (Two-Sample T-Test):** Rigorous statistical validation (`scipy.stats`) proving significant tone divergence ($p < 0.05$) between Part-A (Vision & Outlays) and Part-B (Taxation & Statutory Measures).
* **Multi-LLM Policy Extraction:** Few-shot prompt engineering benchmarking both local open models (via Ollama) and cloud inference (Gemini 3.5 Flash) to generate verified revenue and expenditure tables.

---

## 🛠️ Stack & Dependencies

| Domain | Technologies |
| :--- | :--- |
| **Document Ingestion** | `requests`, `python-docx`, `pypdf` |
| **Data & Numerics** | `pandas`, `numpy` |
| **Natural Language Processing** | `nltk`, `textblob`, `collections` |
| **Statistical Inference** | `scipy.stats` (Two-sample $t$-test) |
| **Visualization** | `matplotlib`, `seaborn`, `wordcloud` |
| **Generative AI** | `ollama` (Local: `llama3.1`, `phi3`, `qwen2`), `google-genai` (`gemini-3.5-flash`) |
| **Configuration** | `python-dotenv` |

---

## 📂 Repository Layout

```text
📦 budget-ai-analysis
 ┣ 📜 BudgetAnalysis.ipynb     # Interactive Jupyter Notebook with full pipeline
 ┣ 📜 requirements.txt         # Pinned production dependencies
 ┣ 📜 Budget_Speech.docx       # Authentic Parliamentary speech transcript
 ┣ 📜 Summary.md               # Synthesized economic highlights & tables
 ┗ 📜 README.md                # Technical documentation
 ┗ 📜 Disclaimer.md           
```

## 🏛️ Data Sourcing & Attribution

All primary text analyzed in this repository originates directly from public domain records published by the **Ministry of Finance, Government of India**:

* **Official Portal:** [India Budget Portal](https://www.indiabudget.gov.in/)
* **Speeches Archive:** [Parliamentary Speeches Archive](https://www.indiabudget.gov.in/bspeech.php)

---

## ⚖️ Disclaimer

* **Academic Use Only:** This analysis is developed solely for educational and research benchmarking. It does not constitute financial, investment, legal, or tax advice.
* **Source of Truth:** In the event of interpretive discrepancies, official publications tabled in Parliament and released by the Ministry of Finance, Government of India remain the sole authoritative authority.

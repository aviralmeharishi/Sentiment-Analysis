# **Indian Union Budget 2024–2025 Analysis (Full Budget)**
### 📊 End-to-End NLP, Sentiment Dynamics & Multi-LLM Economic Synthesis

[![License: Apache-2.0](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![Python](https://img.shields.io/badge/Python-3.10%2B-brightgreen.svg)](https://www.python.org/)
[![NLP](https://img.shields.io/badge/NLP-NLTK%20%7C%20TextBlob-orange.svg)](https://www.nltk.org/)
[![LLMs](https://img.shields.io/badge/LLMs-Gemini%20%7C%20Llama%203.1%20%7C%20Phi--3%20%7C%20Qwen2-purple.svg)](https://ollama.ai)
[![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-F37626.svg)](https://jupyter.org/)

---

## 📌 Context & Speech Overview

| Attribute | Details |
| :--- | :--- |
| **Document Analyzed** | Official Union Budget 2024-25 Speech (Full Budget) |
| **Presented By** | Smt. Nirmala Sitharaman (Hon'ble Union Minister of Finance & Corporate Affairs) |
| **Date of Delivery** | July 23, 2024 |
| **Location** | Lok Sabha, New Delhi, India |
| **Source PDF** | [Ministry of Finance, Government of India (bs2024_25.pdf)](https://www.indiabudget.gov.in/doc/bspeech/bs2024_25.pdf) |
| **Dataset Volume** | 1,371 Filtered Sentences / Analytical Paragraphs |
| **Duration:** | Approximately 85 minutes (~1 hour 25 minutes)|

> [!NOTE]
> **Interim vs. Full Budget Context:**  
> The Interim Budget (Feb 2024) was a temporary "Vote on Account" meant to keep public administration operational during the 2024 General Elections. This **Full Budget (July 2024)** represents the comprehensive 5-year economic roadmap and legislative tax blueprint of the newly formed government.

---

## 💡 What Do These NLP Concepts Mean? *(Quick Guide)*

* ☁️ **WordCloud (Keyword Visualizer):**  
  Words ki frequency ko unke font size se dikhata hai. Jo word Finance Minister ne sabse zyada baar bola, woh canvas par sabse bada aur highlighted dikhta hai.
* 🔗 **N-Grams / Bigrams (Two-Word Pairs):**  
  Single words kabhi-kabhi poora meaning nahi dete. E.g., *"Tax"* se zyada insightful hota hai *"Income Tax"*, *"Customs Duty"*, ya *"Capital Gains"*. Bigram do lagatar aane wale shabdon ka context capture karta hai.
* 📈 **Sentiment Trajectory & Polarity Score:**  
  Har paragraph ka tone $-1.0$ (Very Negative/Cautious) se $+1.0$ (Very Positive/Optimistic) ke beech score hota hai. Isse pata chalta hai ki speech mein kis point par reformist optimism tha aur kahan technical/cautious policy talk.
* 📐 **Two-Sample T-Test ($p$-value):**  
  Ek statistical proof yeh confirm karne ke liye ki speech ke pehle aadhi hisse (First Half) aur doosre aadhi hisse (Second Half) ke tone mein genuine difference hai ya sirf random chance.
* 🤖 **Multi-LLM Synthesis:**  
  Raw Parliamentary speeches 30-40 pages ki hoti hain. Local LLMs (Ollama) aur State-of-the-art Cloud LLMs (Gemini) speech se actual quantitative data extract karke crisp executive tables banate hain.

---

## 🔄 End-to-End Execution Pipeline



---

## 📊 Key Findings from the Notebook

### 1️⃣ Top 10 High-Frequency Keywords
| Rank | Keyword | Occurrences | Analytical Relevance |
| :---: | :--- | :---: | :--- |
| 1 | `tax` | **95** | Central priority on direct & indirect tax structure |
| 2 | `section` | **81** | Legal amendments to the Income-Tax Act & CGST Act |
| 3 | `development` | **50** | Regional & economic growth corridors |
| 4 | `act` | **48** | Legislative statutory modifications |
| 5 | `years` | **46** | Multi-year vision & sunset clauses |
| 6 | `financial` | **38** | Financial sector stability & asset regulations |
| 7 | `new` | **33** | New tax slabs, schemes, and industrial nodes |
| 8 | `support` | **31** | Fiscal support for MSMEs & strategic states (AP/Bihar) |
| 9 | `time` | **31** | Compliance timelines & limitation periods |
| 10 | `propose` | **31** | Direct budgetary proposals tabled by the FM |

---

### 2️⃣ Top 10 Critical Bigrams (Two-Word Phrases)
| Rank | Bigram | Occurrences | Policy Insight |
| :---: | :--- | :---: | :--- |
| 1 | `cgst act` | **19** | Central Goods and Services Tax statutory changes |
| 2 | `section section` | **15** | Cross-referencing legal taxation provisions |
| 3 | `section cgst` | **14** | Specific CGST procedural simplifications |
| 4 | `time limit` | **13** | Easing assessment deadlines & dispute timelines |
| 5 | `financial assets` | **13** | Clarification on short/long term capital classification |
| 6 | `income tax` | **12** | Personal income tax slab rationalization |
| 7 | `tax regime` | **11** | Incentivizing transition to the New Tax Regime |
| 8 | `act amended` | **11** | Formal statutory amendments introduced |
| 9 | `capital gains` | **9** | Rationalized 12.5% LTCG & 20% STCG revisions |
| 10 | `five years` | **8** | Five-year outlay packages for skilling & employment |

---

### 3️⃣ Sentiment & Speech Tone Dynamics

Using `TextBlob`, paragraph-level polarity was measured across **1,371 paragraphs**:

| Metric | Measured Value |
| :--- | :--- |
| **Total Analyzed Paragraphs** | 1,371 |
| **Mean Polarity** | `+0.030` (Neutral-Optimistic) |
| **Standard Deviation** | `0.139` |
| **First Half Average Tone** | `+0.046` (High visionary & developmental optimism) |
| **Second Half Average Tone** | `+0.015` (Factual, precise, legal tax statutory clauses) |
| **T-Test Statistic** | `4.1493` |
| **P-Value** | `0.0000` ($p < 0.05$) |

> **Statistical Conclusion:** The $p$-value is significantly below the $0.05$ threshold. This proves a **statistically significant shift in tone**: the speech opens with socio-economic welfare and growth announcements before transitioning into rigid, legalistic taxation details.

---

## 🏛️ Executive LLM Synthesis (Gemini Engine)

### 📌 1. Sector-Wise Allocations & Major Announcements
* 🌾 **Agriculture & Farmers:** ₹1.52 lakh crore outlay; release of 109 climate-resilient crop varieties; 1 crore farmers initiated into natural farming; Digital Public Infrastructure (DPI) covering 6 crore farmers over 3 years.
* 🎓 **Education & Skills:** ₹1.48 lakh crore provision; 1,000 ITIs upgraded in hub-and-spoke model; education loan e-vouchers up to ₹10 lakh with 3% interest subvention.
* 💼 **Youth & Employment:** PM’s 5-scheme package with ₹2 lakh crore central outlay over 5 years (targeting 4.1 crore youth); 3 Employment-Linked Incentive schemes; paid internship program in top 500 companies for 1 crore youth.
* 🚀 **Startups & MSMEs:** **Complete abolition of Angel Tax** for all investor classes; ₹100 crore credit guarantee scheme for MSME machinery purchases; Mudra loan limit increased to ₹20 lakh under 'Tarun' category.
* 🏗️ **Infrastructure:** Massive capital expenditure outlay maintained at **₹11,11,111 crore (3.4% of GDP)**; ₹1.5 lakh crore in 50-year interest-free loans to states; plug-and-play industrial parks across 100 cities.
* 👩 **Women Empowerment:** Outlay of over ₹3 lakh crore for schemes directly targeting women and girls; lower stamp duties encouraged on property registered in women's names.

---

### 💰 2. 'Rupee Comes From' (Revenue Profile)
* **Total Non-Borrowing Receipts:** ₹32.07 lakh crore
* **Net Tax Receipts:** ₹25.83 lakh crore
* **Gross Market Borrowings:** ₹14.01 lakh crore (Net: ₹11.63 lakh crore)
* **Direct & Corporate Tax Reforms:** Corporate tax on foreign companies reduced from 40% to 35%; New Tax Regime standard deduction raised to ₹75,000.
* **Capital Gains Realignment:** Short-term gains on specified financial assets raised to 20%; Long-term capital gains unified at 12.5%.
* **Indirect Taxes:** Customs duties slashed on gold & silver (to 6%), critical minerals, and mobile manufacturing components.

---

### 💸 3. 'Rupee Goes To' (Expenditure Profile)
* **Total Budget Expenditure:** ₹48.21 lakh crore
* **Public Capital Expenditure (CapEx):** ₹11.11 lakh crore
* **Employment & Skilling Package:** ₹2 lakh crore (5-year horizon)
* **Rural Development Outlay:** ₹2.66 lakh crore
* **Strategic State Support:** ₹15,000 crore arranged for Andhra Pradesh capital development; ₹58,900+ crore committed for Bihar road, power, and flood management projects.

---

## 🛠️ Tech Stack & Dependencies
## 🔄 End-to-End Execution Pipeline

  

┌────────────────────────────────────────────────────────┐
│ 1. PDF Ingestion: pypdf parses official bs2024_25.pdf  │
└──────────────────────────┬─────────────────────────────┘
▼
┌────────────────────────────────────────────────────────┐
│ 2. Text Preprocessing: Regex + Custom Domain Stopwords │
└──────────────────────────┬─────────────────────────────┘
▼
┌────────────────────────────────────────────────────────┐
│ 3. Thematic EDA: WordCloud, Top Words & Bigrams Count  │
└──────────────────────────┬─────────────────────────────┘
▼
┌────────────────────────────────────────────────────────┐
│ 4. Sentiment Analytics: TextBlob Polarity + T-Test     │
└──────────────────────────┬─────────────────────────────┘
▼
┌────────────────────────────────────────────────────────┐
│ 5. LLM Synthesis: Ollama (Phi-3, Llama 3.1) & Gemini   │
└────────────────────────────────────────────────────────┘


---
```python
# Core Data & Text Processing
pypdf==4.2.0
nltk==3.8.1
textblob==0.18.0.post0
pandas==2.2.2
numpy==1.26.4

# Visualization
matplotlib==3.8.4
seaborn==0.13.2
wordcloud==1.9.3

# AI & LLM Inference
ollama           # Local models: Phi-3, Llama 3.1, Qwen2
google-genai     # Google Gemini API

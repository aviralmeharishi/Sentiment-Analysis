# 📊 Indian Union Budget 2023–2024: NLP Analysis

An end-to-end Natural Language Processing (NLP) project that programmatically extracts, cleans, and analyzes the official **Union Budget Speech (2023–24)**—the *"First Budget of Amrit Kaal"*—to uncover dominant themes, sectoral priorities (*Saptarishi*), sentiment trajectories, and parliamentary discourse directly from the official transcript.

---

## 🎙️ Speech Delivery & Metadata

| Attribute | Official Details |
| :--- | :--- |
| **Delivered By** | **Smt. Nirmala Sitharaman** (Hon'ble Minister of Finance and Corporate Affairs) |
| **Occasion** | Annual Financial Statement for FY 2023–2024 (*First Budget in Amrit Kaal*) |
| **Date & Time** | **February 1, 2023 (Wednesday)** at **11:00 AM IST** |
| **Duration** | **87 minutes** (~1 hour 27 minutes) — *Her most crisp and concise full budget speech* |
| **Venue** | **Lok Sabha Chamber**, Parliament House (*Sansad Bhavan*), New Delhi |
| **Document Source** | [Ministry of Finance Portal (bs2023_24.pdf)](https://www.indiabudget.gov.in/doc/bspeech/bs2023_24.pdf) |
| **Corpus Size** | **1,246 Analytical Paragraphs / Sentences** parsed via `pypdf` |

---

## 📰 Media Coverage & Public Reception

Budget 2023–24 received widespread acclaim across national dailies, economists, and market analysts for maintaining fiscal discipline while injecting a record ₹10 Lakh Crore public capital outlay.


| Publication | Headline / Editorial Theme | Rating / Sentiment | Key Assessment & Media Take |
| :--- | :--- | :---: | :--- |
| **The Times of India (TOI)** | *"Rebate of the State / Sweet Spot for Middle Class"* | ★★★★☆<br>**(Strong Cheer)** | Celebrated the overhaul of the New Tax Regime; rebate raised to ₹7 lakh and standard deduction extended. |
| **The Indian Express** | *"The Capex-Heavy Engine: Walking the Fiscal Wire"* | ★★★★☆<br>**(Prudent & Growth-Oriented)** | Praised the 33% capex jump to ₹10 Lakh Crore (3.3% of GDP) while trimming the fiscal deficit target to 5.9%. |
| **The Hindu** | *"Prudence Over Populism in the Amrit Kaal Blueprint"* | ★★★★☆<br>**(Balanced & Measured)** | Commended the refusal to turn populist ahead of 2024 general elections; sustained supply-side capex push. |
| **Mint (Livemint)** | *"Growth-Friendly, Forward-Looking & Market-Prudent"* | ★★★★½<br>**(Thumbs Up from Dalal Street)** | Cheered highest surcharge cut from 37% to 25% (peak tax 42.7% ➔ 39%); Sensex spiked +1,200 pts intraday. |

### 👥 Public & Industry Sentiment (*Janta ka Response*)
* **Middle-Class & Salaried Earners:** Welcomed the revised 5-slab New Tax Regime, making income up to ₹7 Lakh effectively tax-free with Section 87A rebate.
* **Corporate & Industry Bodies (CII, FICCI, ASSOCHAM):** Hailed the ₹10 Lakh Crore infrastructure push, continuation of 50-year interest-free loans to states (₹1.3 Lakh Cr), and decriminalization of 3,400+ legal provisions.
* **Agriculture & Rural Economy:** Applauded the launch of the *Agriculture Accelerator Fund*, *PM-PRANAM* (alternative fertilizers), and credit target enhancement to ₹20 Lakh Crore.

---

## 🎯 Project Objectives
1. **Automated Data Extraction:** Fetch and parse the official 2023–24 Budget Speech PDF directly from the Government of India portal using `requests` and `pypdf`.
2. **Text Preprocessing & Custom Cleaning:** Tokenize text and filter out standard English stopwords, digits, punctuation, parliamentary honorifics (*Madam Speaker*, *Hon'ble*), and financial units (*crores*, *lakhs*) to build a clean analytical corpus.
3. **Thematic & Sectoral EDA:** Identify key unigrams, bigrams, and high-frequency terms mapped to the **7 Pillars (*Saptarishi*)** of the budget using WordClouds and Seaborn visualizations.
4. **Sentiment & Polarity Analysis:** Evaluate paragraph-level sentiment and polarity progression across the speech using `TextBlob` and hypothesis testing (two-sample T-test).
5. **Multi-Model LLM Evaluation:** Synthesize qualitative insights using local (Ollama: `Phi-3`, `Llama 3.1`, `Qwen2`) and cloud (`Google Gemini`) models.

---

## 🏛️ Domain Context: The *Saptarishi* (7 Priorities)
The 2023–24 Budget guided the country's economic blueprint through seven interconnected pillars:
* 🌾 **Inclusive Development:** Farmers, women, youth, OBCs, Scheduled Castes, Scheduled Tribes, and divyangjan.
* 📍 **Reaching the Last Mile:** Pradhan Mantri PVTG Development Mission for vulnerable tribal groups.
* 🏗️ **Infrastructure & Investment:** Capital investment outlay raised by 33% to ₹10 Lakh Crore (3.3% of GDP).
* ⚡ **Unleashing the Potential:** 39,000 compliances reduced; National Data Governance Policy introduced.
* 🌱 **Green Growth:** National Green Hydrogen Mission (₹19,700 Cr outlay); energy transition initiatives.
* 🚀 **Youth Power (*Amrit Peedhi*):** Pradhan Mantri Kaushal Vikas Yojana 4.0; 30 Skill India International Centres.
* 💳 **Financial Sector:** Revamped credit guarantee scheme for MSMEs with ₹9,000 Cr corpus infusion.

---

## 📊 Notebook Findings & Statistics

### 1️⃣ Top 10 Most Frequent Keywords
| Rank | Keyword | Frequency | Strategic Significance |
| :---: | :--- | :---: | :--- |
| 1 | `tax` | **76** | Re-structuring of direct income tax slabs & indirect duty relief |
| 2 | `income` | **53** | Personal income tax relief & rebate up to ₹7 Lakh |
| 3 | `development` | **36** | Rural, cooperative, and regional inclusive development |
| 4 | `duty` | **30** | Rationalization of customs duties on green mobility & electronics |
| 5 | `infrastructure` | **28** | Multi-modal logistics & urban infrastructure development fund |
| 6 | `india` | **28** | Position as bright star in global economic growth |
| 7 | `customs` | **27** | Phased manufacturing tariff adjustments |
| 8 | `capital` | **24** | Unprecedented ₹10 Lakh Crore public capital expenditure push |
| 9 | `shall` | **23** | Legislative and statutory enactments |
| 10 | `sector` | **21** | Priority focus on MSMEs, agriculture, and financial sector |

### 2️⃣ Top 10 Bigrams (Co-occurring Phrases)
| Rank | Bigram | Count | Domain Insight |
| :---: | :--- | :---: | :--- |
| 1 | `customs duty` | **15** | Tariff exemptions for battery cells, camera lenses, and lab-grown diamonds |
| 2 | `basic customs` | **10** | Basic customs duty rate rationalization |
| 3 | `income tax` | **10** | Personal tax overhaul and standard deduction extension |
| 4 | `amrit kaal` | **7** | Foundational vision for India @ 100 |
| 5 | `public infrastructure` | **6** | Expansion of digital public goods (UPI, DigiLocker, DPI) |
| 6 | `primary agricultural` | **6** | Computerization of 63,000 Primary Agricultural Credit Societies (PACS) |
| 7 | `capital expenditure` | **6** | ₹10 Lakh Crore capex engine for GDP multiplier |
| 8 | `urban infrastructure` | **6** | Urban Infrastructure Development Fund (UIDF) via NHB |
| 9 | `fiscal deficit` | **6** | Deficit glide path pegged at 5.9% of GDP |
| 10 | `capital gains` | **6** | Rationalization of capital gains exemptions on high-value properties |

### 3️⃣ Sentiment & Speech Tone Dynamics
* **Total Evaluated Units:** 1,246 Paragraphs
* **Mean Polarity:** `+0.032` (Balanced / Measured Optimism)
* **Standard Deviation:** `0.154`
* **First Half Sentiment (Vision & Schemes):** `+0.049`
* **Second Half Sentiment (Tax Clauses & Duties):** `0.014`
* **Two-Sample T-Test:** `t = 4.0165`, `p = 0.0001` ($p < 0.05$)
* **Inference:** A statistically significant shift from inspirational welfare announcements in Part A to highly technical, regulatory clauses in Part B.

---

## 🛠️ Tech Stack & Libraries
* **Language:** Python 3.10+
* **Data Manipulation & Stats:** `numpy`, `pandas`, `scipy`
* **Document Extraction:** `requests`, `pypdf`
* **NLP & Text Processing:** `nltk` (tokenizers, stopwords, ngrams), `textblob`
* **Data Visualization:** `matplotlib`, `seaborn`, `wordcloud`
* **AI & LLM Synthesis:** `google-genai` (Gemini), `ollama` (Phi-3, Llama 3.1, Qwen2)

---

## ⚙️ Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/union-budget-2023-24-nlp.git
2. **Create and activate a virtual environment:**
```bash
   python -m venv venv
   # Windows:
   venv\Scripts\activate
   # Linux/macOS:
   source venv/bin/activate

# **📊 Indian Union Budget 2023–2024**

An end-to-end Natural Language Processing (NLP) project that programmatically extracts, cleans, and analyzes the official **Union Budget Speech (2023–24)**—the *"First Budget of Amrit Kaal"*—to uncover dominant themes, sectoral priorities (*Saptarishi*), and sentiment trajectories directly from the parliamentary transcript.

---

## 🎯 Project Objectives
1. **Automated Data Extraction:** Fetch and parse the official 2023–24 Budget Speech PDF directly from the Government of India portal using `requests` and `pypdf`.
2. **Text Preprocessing & Custom Cleaning:** Tokenize text and filter out standard English stopwords, digits, punctuation, parliamentary honorifics (*Madam Speaker*, *Hon'ble*), and financial units (*crores*, *lakhs*) to build a clean analytical corpus.
3. **Thematic & Sectoral EDA:** Identify key unigrams, bigrams, and high-frequency terms mapped to the **7 Pillars (*Saptarishi*)** of the budget using WordClouds and Seaborn visualizations.
4. **Sentiment & Polarity Analysis:** Evaluate paragraph-level sentiment and polarity progression across the speech using `TextBlob` and LLM integrations.

---

## 🏛️ Domain Context: The *Saptarishi* (7 Priorities)
Budget 2023–24 was structured around seven core economic pillars:
* **Inclusive Development** (Farmers, Women, Youth, Marginalized sections)
* **Reaching the Last Mile** (Tribal welfare, Aspirational districts)
* **Infrastructure & Investment** (₹10 Lakh Crore CapEx push)
* **Unleashing the Potential** (Ease of doing business, Digital Public Infrastructure)
* **Green Growth** (National Green Hydrogen Mission, Net-Zero transition)
* **Youth Power (*Amrit Peedhi*)** (PMKVY 4.0, Skill Development)
* **Financial Sector** (MSME credit guarantees, Regulatory reforms)

---

## 🛠️ Tech Stack & Libraries
* **Language:** Python 3.x
* **Data Manipulation & Math:** `numpy`, `pandas`, `scipy`
* **Document Scraping & Parsing:** `requests`, `pypdf`, `python-docx`
* **NLP & Text Processing:** `nltk` (punkt, stopwords, ngrams), `textblob`
* **Data Visualization:** `matplotlib`, `seaborn`, `wordcloud`
* **AI / LLM Integrations:** `google-genai`, `groq`, `ollama`, `python-dotenv`

---

## ⚙️ Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-username/union-budget-2023-24-nlp.git](https://github.com/your-username/union-budget-2023-24-nlp.git)
   cd union-budget-2023-24-nlp

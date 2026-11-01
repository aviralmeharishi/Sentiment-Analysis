# 📌 About This Project, Data Sources & Disclaimer (Budget 2025–26)

---

### 👋 A Quick Note Before You Dive In
Hey there! As a data science enthusiast, I built this notebook to explore how **Natural Language Processing (NLP)** and modern **AI/LLMs** can help us unpack long, dense government speeches. Instead of relying purely on media headlines or 2-minute news summaries, I wanted to let the raw speech text speak for itself through data.

However, since economic speeches deal with real-world policies and public money, here is complete transparency about where the data comes from and how this analysis should be interpreted.

---

### 🏛️ Where Did This Data Come From? (Source & Attribution)
Every line of text analyzed in this notebook is 100% authentic and taken directly from official public records:

* **Official Document:** Union Budget Speech (2025–2026)
* **Delivered By:** Hon'ble Finance Minister, Smt. Nirmala Sitharaman
* **Date Presented:** February 1, 2025
* **Official Source:** Ministry of Finance, Government of India
* **Direct Download Link:** [Official India Budget Archives (PDF)](https://www.indiabudget.gov.in/doc/bspeech/bs2025_26.pdf)
* **How It Was Processed:** Extracted programmatically page-by-page from the official Parliamentary `.pdf` document using Python's `pypdf` library.

---

### ⚠️ Important Things to Keep in Mind (Disclaimer)

1. **Not Financial or Investment Advice:**  
   This analysis is purely an academic and portfolio project. Please do not use these charts, sentiment graphs, or AI summaries to make stock market trades, tax planning decisions, or financial investments.

2. **How NLP & AI Actually Work Here (Known Limitations):**  
   * **Sentiment Scores:** Tools like TextBlob evaluate whether words are positive or negative in a general English context. They can't fully grasp parliamentary context, diplomatic language, or conditional scheme outlays.
   * **Sector Keyword Matches:** When we count words like *"rail"*, *"farmer"*, or *"ai"*, it gives a great high-level snapshot of focus areas, but it doesn't automatically mean a bigger budget allocation in rupee terms.
   * **AI Summaries (Ollama / Gemini):** While I have strictly instructed the models to stick only to the speech text, language models can occasionally misinterpret complex legal clauses. Always double-check critical policy points with primary documents.

3. **The Final Source of Truth:**  
   If you ever notice any difference between what this notebook displays and the official government publications, **the official documents released by the Ministry of Finance are always the final and correct authority**. (Check out the *Annual Financial Statement* and *Finance Bill* on the budget portal).

4. **Independent Work:**  
   This is an independent personal project created for learning and demonstration. It has no official connection to, sponsorship from, or endorsement by the Government of India or the Ministry of Finance.

# 📌 About This Project, Data Sources & Disclaimer (Budget 2026–27)

---

### 👋 A Quick Note Before You Dive In
Hey there! The Union Budget speech is one of the most important economic documents in our country. Every year, it sets the tone for India's growth, taxes, and national priorities. But at 30 to 40 pages long, reading it manually can be overwhelming.

I created this project to bridge that gap—using **text mining, exploratory data analysis, and Large Language Models (LLMs)** to uncover key sectoral themes, sentiment shifts, and policy priorities straight from the authentic transcript.

Here is a quick look at where the data was sourced and a few important things to keep in mind while browsing this notebook.

---

### 🏛️ Where Did This Data Come From? (Source & Attribution)
This analysis uses zero third-party or unverified articles. Everything comes straight from the official government portal:

* **Official Document:** Union Budget Speech (2026–2027)
* **Delivered By:** Hon'ble Finance Minister, Smt. Nirmala Sitharaman
* **Date Presented:** February 1, 2026
* **Official Source:** Ministry of Finance, Government of India
* **Direct Download Link:** [Official India Budget Portal (DOCX)](https://www.indiabudget.gov.in/doc/budget_speech.docx)
* **How It Was Processed:** Downloaded directly as the authentic Word document (`.docx`) and extracted paragraph-by-paragraph using Python's `python-docx` library.

---

### ⚠️ Important Things to Keep in Mind (Disclaimer)

1. **For Educational & Portfolio Purposes Only:**  
   This notebook is built to showcase end-to-end data science, NLP, and GenAI workflows. It is **not** financial guidance, investment research, or tax advice. Please do not base personal financial decisions on the data visualisations or sentiment numbers shown here.

2. **The Reality of Automated Text Analysis:**  
   * **Cleaned Text:** To create clean WordClouds and bigrams, I have filtered out legal jargon, standard numbers, and common filler words (like *'crore'*, *'hon'ble'*, *'speaker'*). This makes the visualizations much clearer, but it means individual sentences are stripped of grammar.
   * **Sentiment & Sector Trends:** A higher frequency of a sector's name (e.g., *'Infrastructure'* vs *'Health'*) reflects parliamentary emphasis, but not necessarily actual fund allocation.
   * **LLM Interpretations (Ollama & Gemini):** The AI models in this notebook are prompted to stay grounded strictly in the speech text. However, LLMs can sometimes summarize things in their own words or miss subtle caveats, so treat their output as smart overviews, not statutory law.

3. **Official Documents Are the Ultimate Authority:**  
   In case of any doubt, discrepancy, or confusion, please refer directly to the official papers tabled in Parliament—specifically the *Budget at a Glance (BAG)* and the *Finance Bill 2026*.

4. **No Official Affiliation:**  
   This is a purely independent, non-commercial open-source project. It is not affiliated with, funded by, or representative of the Ministry of Finance or any department of the Government of India.

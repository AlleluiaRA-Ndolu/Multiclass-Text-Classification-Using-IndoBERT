# 📰 Multiclass Text Classification Using LLMs  

## 📌 Project Overview  
This project implements **multiclass text classification** of Indonesian sports news articles using **Large Language Models (LLMs)**, specifically **IndoBERT** from Hugging Face Transformers.  

The goal is to automatically classify news articles into 5 categories, while comparing two approaches:  

1. **1-Stage Classification** → directly classifies articles into 5 categories.  
2. **2-Stage Hierarchical Classification** → first distinguishes *football* vs *non-football*, then further classifies football into specific leagues.  

---

## ⚙️ Tech Stack  
- Python  
- Hugging Face Transformers (IndoBERT)  
- Scikit-learn  
- Pandas & NumPy  
- Matplotlib / Seaborn (visualization)  

---

## 🗂️ Dataset  
- News articles scraped from Indonesian media (e.g., Detik, Liputan6).  
- Categories:  
  - 🏸 Non-football sports  
  - ⚽ Liga Inggris  
  - 🇮🇩 Liga Indonesia  
  - 🇪🇸 Liga Spanyol  
  - 🇮🇹 Liga Italia  

---

## 🔬 Methodology  
1. **Data Collection** → Web scraping & manual labeling.  
2. **Text Preprocessing** → cleansing, tokenization, filtering, lemmatization/stemming.  
3. **Modeling** → Fine-tuned IndoBERT for classification.  
   - Model A: 1-stage, direct classification into 5 classes.  
   - Model B: 2-stage, hierarchical classification.  
4. **Evaluation** → Compared accuracy, precision, recall, and F1-score between both approaches.  

---

## 📊 Results  
- The **2-stage hierarchical classification** achieved better performance than the direct 1-stage approach.  
- Confusion matrices showed reduced misclassification for football categories.  
- Final model demonstrated improved accuracy and robustness across categories.  

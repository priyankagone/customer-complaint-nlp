# Customer Complaint Root-Cause Intelligence using NLP

## 📌 Project Overview
This project builds an **NLP-driven complaint intelligence system** to identify **root causes, emerging risks, and product-level deterioration trends** from real-world consumer complaint data.

Instead of focusing on sentiment analysis or deep learning models, this project emphasizes:
- Interpretable NLP
- Business-oriented insights
- Trend and risk analysis at scale

The analysis is performed on **800k+ real consumer complaints** published by the U.S. Consumer Financial Protection Bureau (CFPB).

---

## 🎯 Objectives
- Discover major **complaint themes (root causes)** using topic modeling
- Analyze how complaint topics **change over time**
- Identify **high-risk topics** with higher dispute rates
- Detect **products and issues showing deterioration**
- Translate NLP outputs into **actionable business insights**

---

## 📊 Dataset
**Source:** CFPB Consumer Complaints Database  
**Time Range:** Last 10 years  
**Records Used:** ~800k+ complaints  
**Key Feature:** Only complaints with narrative text (`Has narrative = true`)

### Key Columns Used
- Consumer complaint narrative
- Product / Sub-product
- Issue / Sub-issue
- Company
- Date received
- Submitted via
- Company response to consumer
- Timely response?
- Consumer disputed?

---

## 🧠 Methodology

### 1️⃣ Text Cleaning & Preparation
- Lowercasing, punctuation removal
- Stopword removal
- Length-based linguistic analysis

### 2️⃣ Exploratory Text Analysis
- Complaint length as a severity proxy
- Product-wise vocabulary differences
- Bigram (phrase-level) analysis
- Channel-based language variation

### 3️⃣ Topic Modeling (Root-Cause Discovery)
- TF-IDF vectorization (unigrams + bigrams)
- **Non-Negative Matrix Factorization (NMF)**
- Manual topic naming for business interpretability

### 4️⃣ Trend & Topic Drift Analysis
- Monthly topic share analysis
- Emerging issue detection
- Product-specific topic deterioration
- Dispute-rate–based risk prioritization

## 🔍 Key Insights
- A small number of complaint themes account for a majority of consumer issues, indicating systemic rather than isolated problems.
- Certain complaint topics show a **consistent increase over time**, acting as early warning signals for operational and compliance risks.
- Some products exhibit **significantly higher dispute rates** for specific complaint themes, highlighting areas requiring immediate attention.
- Longer and more detailed complaint narratives are more likely to escalate into formal disputes, suggesting complaint length can act as a proxy for severity.

---

## 🚀 Business Use Cases
- Monthly complaint monitoring and reporting dashboards
- Early warning systems for emerging consumer issues
- Product-level performance and risk benchmarking
- Regulatory risk identification and compliance monitoring
- Customer experience and process improvement initiatives

---

## ⚠️ Limitations & Future Work
- Topic modeling results depend on the quality and consistency of complaint narratives.
- Manual topic labeling introduces subjectivity, although it improves business interpretability.
- The analysis is based on historical data and does not include real-time monitoring.
- Future enhancements could include:
  - Sentence-level or hierarchical topic modeling
  - Automated alert generation for emerging issues
  - Integration with real-time complaint ingestion pipelines

---

## 📌 Conclusion
This project demonstrates how **interpretable and lightweight NLP techniques** can be applied at scale to transform unstructured consumer complaint text into **actionable business intelligence**.  
By combining topic modeling with trend and risk analysis, the system enables organizations to proactively identify emerging issues, prioritize high-risk areas, and improve customer experience and compliance outcomes.



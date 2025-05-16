# Identification-of-Adverse-Drug-Reactions

## 📌 Overview
This project aims to classify English-language tweets based on whether they mention **Adverse Drug Reactions (ADRs)**.

### Task
Given a tweet containing a drug name, classify it as:
- **1 (Positive)**: Mentions an ADR  
  *Example*: "Shouldn’t have taken the Vyvanse. Now I’m never sleeping."
- **0 (Negative)**: Does **not** mention an ADR  
  *Example*: "#Prozac come and help me please!"

---

## 📂 Dataset
- Provided by the **Biomedical Informatics Lab (DIEGO Lab)** at Arizona State University.
- Contains tweet IDs, user IDs, and labels.
- Tweet texts were retrieved via the Twitter API (many are no longer available).
- Class imbalance: ~90% of tweets belong to the **negative** class.

---

### 🔍 Evaluation
We use **F1 score (positive class)** as the main metric:
- **Precision**: True ADRs among predicted ADRs
- **Recall**: True ADRs identified
- **F1**: Harmonic mean of precision & recall

---

## ✅ Results
- Final model: Transformer-based (e.g., BERT variants)
- Best F1 (positive class): **0.5211**


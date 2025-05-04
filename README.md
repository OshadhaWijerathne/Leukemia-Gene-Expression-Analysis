# 🔬 Gene Expression Analysis in AML and ALL Leukemia

**Author:** R.K.A.O. Wijerathne (200721N)  
**Assignment:** Expression of Genes in AML and ALL Type Leukemia

## 📌 Overview

This project investigates gene expression data to distinguish between two types of leukemia: **Acute Myeloid Leukemia (AML)** and **Acute Lymphoblastic Leukemia (ALL)**. The analysis includes interpretable classification models and unsupervised clustering methods to identify key gene markers and understand the underlying data structure.

---

## 📁 Dataset

- **Samples:** 72 patient samples
- **Genes:** 7129 gene expression values per sample
- **Split:** 38 training samples, 34 testing samples
- **Preprocessing:** Metadata columns removed, data transposed, and normalized.

---

## 🧠 Classification Models

### ✅ Decision Tree Classifier

- **Criterion:** Gini
- **Max Depth:** 3  
- **Min Samples Leaf:** 1  
- **Min Samples Split:** 2  
- **Test Accuracy:** **91.2%**

🔎 *Provides a rule-based, interpretable path for classification.*

---

### ✅ L1-Regularized Logistic Regression

- **Penalty:** L1 (Lasso)
- **C (Inverse Regularization Strength):** 1
- **Solver:** liblinear
- **Max Iterations:** 10,000  
- **Test Accuracy:** **100%**

📌 **Chosen as the final model** due to perfect accuracy and clear gene relevance.

---

## 🧬 Key Predictive Genes

Top 15 genes identified based on scaled logistic regression coefficients:

M27891_at, M19507_at, Y00787_s_at, L06797_s_at, M28130_rna1_s_at,
M96326_rna1_at, U01317_cds4_at, M91438_at, M91036_rna1_at, M92287_at,
V00594_s_at, X82240_rna1_at, L13210_at, M84526_at, HG3576-HT3779_f_at

🧪 These genes are strong candidates as **biomarkers** for leukemia diagnosis and subtype differentiation.

---

## 🔍 Unsupervised Clustering Analysis

### 📊 K-Means Clustering
- **Clusters:** 2
- **Purity:** **0.763**

### 🌿 Hierarchical Clustering (Agglomerative)
- **Clusters:** 2
- **Purity:** **0.816**

---

## 📈 Summary of Results

| Task            | Method                     | Outcome           |
|-----------------|----------------------------|-------------------|
| Classification  | Logistic Regression (L1)   | ✅ 100% Accuracy   |
| Top Genes       | Logistic Coeff. Analysis    | 🔬 15 Genes Found  |
| Clustering      | Hierarchical Clustering     | 📊 Purity = 0.816 |

---

## 🛠️ Technologies Used

- Python
- Scikit-learn
- Pandas / NumPy
- Matplotlib / Seaborn

---

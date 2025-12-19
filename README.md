# Credit Card Fraud Detection

# Problem Statement
Credit card fraud causes significant financial losses and requires systems that can accurately identify fraudulent transactions while minimizing false alarms.  
This project focuses on building and evaluating a fraud detection system on **highly imbalanced transaction data**, where fraudulent cases form a very small fraction of total transactions.

---

#  Dataset Overview
- Public credit card transaction dataset
- Contains anonymized numerical features (V1–V28), `Time`, and `Amount`
- Target variable: `Class`
  - `0` → Legitimate transaction  
  - `1` → Fraudulent transaction
- Highly imbalanced dataset (fraud cases ≪ normal cases)

---

# Approach & Methodology

## Data Preprocessing
- Checked for missing and inconsistent values
- Applied feature scaling to normalize numerical features
- Addressed **class imbalance** using techniques such as:
  - Class weighting / resampling strategies
- Split data into training and testing sets to ensure fair evaluation

---

### Model Development
Implemented and compared multiple machine learning models, including:
- Logistic Regression
- Decision Trees / Random Forest (if applicable)

The goal was not only to achieve good performance, but also to understand **model behavior under imbalanced data conditions**.

---

### Evaluation Strategy
Instead of relying only on accuracy, the models were evaluated using:
- **Precision**
- **Recall**
- **F1-Score**
- **ROC-AUC**
- **Confusion Matrix**

This helped analyze trade-offs between detecting fraud correctly and avoiding false positives, which is critical in real-world financial systems.

---

## Results & Analysis
- Observed that accuracy alone is misleading due to severe class imbalance
- Precision–recall analysis provided better insight into fraud detection effectiveness
- Selected the model that offered the best balance between detecting fraudulent transactions and minimizing incorrect fraud flags

---

## Key Learnings
- Handling imbalanced data is crucial in real-world ML problems
- Evaluation metrics must align with the business objective
- Clear preprocessing and evaluation pipelines improve reproducibility and clarity
- Model selection involves trade-offs, not just maximizing a single metric

---

## Future Improvements
- Experiment with advanced imbalance handling techniques
- Add cross-validation for more robust evaluation
- Convert the notebook into modular Python scripts
- Explore deployment as a REST API for real-time fraud detection

---

## 🛠️ Technologies Used
- Python
- NumPy, Pandas
- Scikit-learn
- Matplotlib / Seaborn
- Jupyter Notebook

---

## ▶️ How to Run
1. Clone the repository  
2. Open the Jupyter Notebook  
3. Run all cells sequentially to reproduce results  

---


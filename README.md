# Credit Card Fraud Detection System

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![ML](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn-orange)
![XGBoost](https://img.shields.io/badge/XGBoost-Enabled-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

##  Overview
A Machine Learning system that detects fraudulent credit card transactions using multiple classification algorithms. The project addresses the **class imbalance problem** using SMOTE and compares 4 different models to find the best performer.

---

##  Problem Statement
Credit card fraud causes billions in losses globally every year. The challenge is identifying fraudulent transactions from a heavily imbalanced dataset where fraud cases are less than 0.2% of all transactions.

---

##  Project Structure
```
credit-card-fraud-detection/
│
├── credit_card_fraud_detection.ipynb   # Main notebook
├── README.md                           # Project documentation
├── requirements.txt                    # Dependencies
└── plots/                              # Generated visualizations
    ├── 01_class_distribution.png
    ├── 02_correlation_heatmap.png
    ├── 03_model_comparison.png
    ├── 04_confusion_matrices.png
    ├── 05_roc_curves.png
    └── 06_feature_importance.png
```

---

##  Models Used
| Model | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|---|---|---|---|---|---|
| Logistic Regression | ~85% | ~82% | ~79% | ~80% | ~88% |
| Decision Tree | ~88% | ~85% | ~81% | ~83% | ~85% |
| Random Forest | ~93% | ~91% | ~87% | ~89% | ~95% |
| **XGBoost**  | **~94%** | **~92%** | **~90%** | **~91%** | **~96%** |

> **Best Model: XGBoost** with 94% accuracy and 96% ROC-AUC

---

##  Tech Stack
- **Language:** Python 3.10
- **Libraries:** Pandas, NumPy, Scikit-Learn, XGBoost, Imbalanced-Learn
- **Visualization:** Matplotlib, Seaborn
- **Notebook:** Jupyter Notebook

---

##  Key Techniques
- **SMOTE** (Synthetic Minority Oversampling) to handle class imbalance
- **StandardScaler** for feature normalization
- **Cross-validation** for reliable performance estimates
- **ROC-AUC** as primary evaluation metric for imbalanced data
- **Feature Importance** analysis using Random Forest

---

##  Visualizations
- Class distribution pie chart
- Correlation heatmap of top features
- Model comparison bar chart
- Confusion matrices for all models
- ROC curves comparison
- Feature importance ranking

---

##  How to Run

```bash
# 1. Clone the repository
git clone https://github.com/bhanuprakash930/credit-card-fraud-detection.git
cd credit-card-fraud-detection

# 2. Install dependencies
pip install -r requirements.txt

# 3. Download the dataset
# Get creditcard.csv from: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud
# Place it in the project root folder

# 4. Launch Jupyter Notebook
jupyter notebook credit_card_fraud_detection.ipynb
```

---

## Dataset
- **Source:** [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Size:** 284,807 transactions | 492 fraud cases
- **Features:** 30 (V1–V28 are PCA components, Amount, Time)

---

##  Author
**Onteddu Bhanu Prakash**  
B.Tech CSE (AI & ML) — Mohan Babu University  
 bhanuprakash09871234@gmail.com  
 [LinkedIn](https://linkedin.com/in/onteddu-bhanu-prakash-reddy-1415ab2a1)

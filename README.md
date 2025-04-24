# 🧠 Fraud Detection in Blockchain Transactions using Machine Learning

This project explores the use of machine learning techniques to detect fraudulent Bitcoin transactions using the publicly available **Elliptic dataset**. The primary goal is to identify potentially illicit blockchain transactions with high precision and recall, supporting efforts in anti-money laundering and blockchain transparency.

---

## 📁 Project Structure
---

## 📊 Dataset

**Source**: [Elliptic Dataset on Kaggle](https://www.kaggle.com/datasets/ellipticco/elliptic-data-set)  
- 203,769 Bitcoin transactions  
- 166 anonymized features  
- Labels: `illicit`, `licit`, `unknown`  
- Only labeled subset was used for model training

---

## ⚙️ Methodology

Two classifiers were trained and evaluated:
- **Random Forest**
- **XGBoost (Gradient Boosted Trees)**

### Preprocessing:
- Removed `unknown` labels
- Relabeled: `illicit = 1`, `licit = 0`
- Used a 70/30 train/test split

---

## 📈 Results

| Metric        | Random Forest | XGBoost      |
|---------------|----------------|--------------|
| Accuracy      | 99%            | 99%          |
| Precision (1) | 100%           | 99%          |
| Recall (1)    | 87%            | **89%**      |
| F1-score (1)  | 93%            | **94%**      |

XGBoost showed a slight edge in recall and F1-score, making it the preferred model for detecting illicit transactions.

---

## 🧪 How to Run

1. Clone this repository:
```bash
git clone https://github.com/HtayNai00/blockchain-ml-final.git



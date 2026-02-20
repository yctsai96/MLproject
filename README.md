 # Income Prediction and Marketing Segmentation Analysis

This project builds machine learning models to identify high-income individuals and performs customer segmentation for marketing strategy.

---

## Project Overview

The objective of this project is to:

1. Predict whether an individual's income exceeds $50K (`classification.ipynb`)
2. Identify actionable population segments for marketing strategy (`segmentation.ipynb`)

---

## Project Structure
```
project/
├── EDA.ipynb
├── classification.ipynb
├── segmentation.ipynb
├── cleaned_df.pkl
└── README.md
```

---

## Environment Setup

Tested Python version:
- Python 3.11.14

Required packages:

```bash
pip install numpy pandas scipy scikit-learn xgboost==1.7.6 shap==0.43.0 kmodes matplotlib seaborn
```

---

## How to Run


### Step 1. Run classification

Open and run:

`classification.ipynb`

This notebook will:

- Load `cleaned_df.pkl`  
- Train multiple models  
- Select XGBoost based on ROC and PR performance  
- Optimize the decision threshold using cost-sensitive analysis  
- Generate confusion matrix and evaluation metrics  
- Produce SHAP explanations  

---

### Step 2. Run segmentation

Open and run:

`segmentation.ipynb`

This notebook will:

- Load `cleaned_df.pkl`  
- Perform feature engineering  
- Perform customer clustering (K-Modes)  
- Profile each segment  
- Generate business insights

# Water Quality Prediction using Random Forest

This repository contains a Jupyter Notebook that applies **Random Forest classification** to a **Water Quality dataset**.  
The goal is to predict whether water is **potable (safe for drinking)** or **non-potable** based on various chemical and physical parameters.

---

## 📊 Dataset

The dataset includes water quality indicators such as:
- pH
- Hardness
- Solids
- Chloramines
- Sulfate
- Conductivity
- Organic carbon
- Trihalomethanes
- Turbidity
- Potability (target variable)

> **Source**: Commonly used "Water Quality" dataset available on Kaggle and other open repositories.

---

## ⚙️ Methodology

1. **Data Preprocessing**
   - Handling missing values
   - Scaling/normalization
   - Train-test split

2. **Exploratory Data Analysis (EDA)**
   - Statistical summaries
   - Correlation heatmap
   - Distribution plots

3. **Modeling**
   - Random Forest Classifier
   - Hyperparameter tuning (if applied)
   - Cross-validation

4. **Evaluation**
   - Accuracy
   - Precision, Recall, F1-score
   - Confusion Matrix

---

## 📈 Results

- Achieved good classification accuracy for predicting potability.
- Identified key features influencing water quality.
- Model performance visualized using confusion matrix and metrics plots.

---

## 🛠️ Requirements

To run the notebook, install the dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn

# 💧 Water Quality Prediction with Random Forest

Hi, I’m **Swapnil Sudhakar Patil** 👋  

This project is a part of my learning journey as I transition into the field of **Data Analytics and Machine Learning**.  
Here, I explored how **Random Forest** can be used to predict whether water is **potable (drinkable)** or **not potable**, based on real-world chemical and physical parameters.

---

## 🌟 Why This Project?

Access to clean drinking water is one of the most important challenges in the world.  
I wanted to see how machine learning can assist in this — not by replacing traditional lab tests, but by giving **quick predictions** that could help in early decision-making.  

For me, this project was also a chance to:
- Practice **data preprocessing and cleaning**.
- Perform **Exploratory Data Analysis (EDA)** and visualization.
- Apply **Random Forest classification**.
- Interpret the results in a meaningful way.

---

## 📊 Dataset

The dataset contains important water quality indicators like:
- pH  
- Hardness  
- Solids  
- Chloramines  
- Sulfate  
- Conductivity  
- Organic carbon  
- Trihalomethanes  
- Turbidity  
- **Potability** (target variable: 1 = potable, 0 = not potable)  

> Dataset reference: "Water Quality" dataset, widely available on Kaggle and open-source repositories.

---

## ⚙️ What I Did

1. **Data Preprocessing**
   - Handled missing values
   - Standardized features where required
   - Split into training and test sets

2. **Exploratory Data Analysis**
   - Visualized distributions and correlations
   - Understood which features influence water quality most

3. **Modeling**
   - Built a **Random Forest Classifier**
   - Tuned hyperparameters for better accuracy
   - Compared metrics across models

4. **Evaluation**
   - Accuracy, Precision, Recall, F1-score
   - Confusion Matrix visualization
   - Feature importance analysis## 📈 Results

After training and testing the Random Forest model, here’s what I found:

- **Accuracy:** 88.0 %  
- **Precision:** 0.44  
- **Recall:** 0.20  
- **F1 Score:** 0.28  

**Confusion Matrix:**

|                | Predicted: 0 | Predicted: 1 |
|----------------|--------------|--------------|
| **Actual: 0**  | 1365         | 49           |
| **Actual: 1**  | 148          | 38           |

**Cross-Validation (GridSearchCV):**
- Best Score: ~90.1%  
- Hyperparameters tuned: `n_estimators`, `criterion`, `max_depth`, `min_samples_split`, `min_samples_leaf`, `max_features`

---

### 🔎 Interpretation

- The model is **very good at predicting non-potable water (class 0)** with high accuracy.  
- However, recall for **potable water (class 1)** is relatively low, meaning the model struggles to correctly identify all safe water samples.  
- With better feature engineering or advanced models (like **XGBoost**), performance on minority class can be improved.


---

## 📈 What I Learned

- Data cleaning is just as important as model building.  
- Random Forest is powerful for classification, but parameter tuning makes a huge difference.  
- Feature importance gives us real insight into **which water quality parameters matter most**.  

---

## 🛠️ How to Run

Clone the repo and open the notebook:

```bash
git clone https://github.com/your-username/water-quality-random-forest.git
cd water-quality-random-forest
jupyter notebook ANS_Water\ Quality\ dataset_Random_Forest_.ipynb

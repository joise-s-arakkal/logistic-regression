# 🩺 Task 4: Logistic Regression - Breast Cancer Classification
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1_EoyUQKJb487ZXa2KlItFkQ4m4r9a0o3?usp=sharing)

## 📌 Objective

The goal of this task is to **implement and understand logistic regression** for binary classification on the Breast Cancer Wisconsin dataset. We aim to predict whether a tumor is malignant or benign based on its features.

---

## 🛠 Tools & Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

---

## 📂 Dataset

Dataset: [`data.csv`](data.csv)  
Source: [Kaggle - Breast Cancer Wisconsin Dataset](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data)

**Target Variable**: `diagnosis`  
- `M` (malignant) mapped to `1`  
- `B` (benign) mapped to `0`

**Features** include:
- Cell nuclei measurements (radius, texture, perimeter, area, smoothness, concavity, symmetry, etc.)

---

## 🧪 Steps Performed

1. **Data Preprocessing**  
   - Loaded CSV data using Pandas  
   - Dropped columns `id` and `Unnamed: 32`  
   - Mapped target `diagnosis` to binary (M=1, B=0)

2. **Train-Test Split**  
   - Used 80% for training and 20% for testing  
   - Stratified split to maintain class balance  
   - Random seed set for reproducibility

3. **Feature Scaling**  
   - Applied `StandardScaler` for normalization

4. **Model Training**  
   - Fitted a `LogisticRegression()` model from `sklearn.linear_model`

5. **Evaluation Metrics**  
   - Confusion Matrix  
   - Precision  
   - Recall  
   - ROC-AUC Score  

6. **Visualization**  
   - Plotted the ROC curve  
   - Visualized the sigmoid function

---

## 📊 Results

| Metric        | Value           |
|---------------|-----------------|
| Precision     | 0.97            |
| Recall        | 0.92            |
| ROC-AUC       | 0.99            |

---

## 🔍 Key Learnings

- How to apply logistic regression to binary classification problems
- The interpretation of the sigmoid function in mapping probabilities
- The use of evaluation metrics such as precision, recall, and ROC-AUC
- How to visualize the ROC curve to interpret classifier performance
- The impact of feature scaling on convergence and model stability

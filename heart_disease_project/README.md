#  Heart Disease Prediction Project

This project aims to predict the presence of heart disease using clinical features from the UCI Heart Disease dataset. We explore three supervised machine learning models:  
- Logistic Regression  
- K-Nearest Neighbors (KNN)  
- Decision Tree Classifier  

---

## 📁 Dataset Information

- **Source**: UCI Machine Learning Repository  
- **Access**: Imported using `ucimlrepo`  
- **Attributes** include:
  - Age, Sex, Chest Pain Type (cp)
  - Resting Blood Pressure (trestbps)
  - Cholesterol (chol), Fasting Blood Sugar (fbs)
  - Rest ECG (restecg), Max Heart Rate (thalach)
  - Exercise-induced Angina (exang), ST Depression (oldpeak)
  - Slope, Major Vessels (ca), Thalassemia (thal)
  - **Target (num)** – presence or absence of heart disease

---

## 🧠 Models Used

| Model               | Description |
|--------------------|-------------|
| Logistic Regression | Linear model for binary classification |
| K-Nearest Neighbors | Distance-based classifier |
| Decision Tree       | Tree-structured non-linear model |

---

## ✅ Project Workflow

### Step 1: Data Acquisition & EDA  
- Fetch dataset using `ucimlrepo`  
- Perform exploratory data analysis (EDA)  
- Visualize feature distributions, boxplots, correlation heatmap  

### Step 2: Preprocessing  
- Handle missing values  
- Encode categorical variables (one-hot)  
- Scale numerical features using `StandardScaler`  
- Split data into training and testing sets (80:20)  

### Step 3: Model Training  
- Train three models (Logistic Regression, KNN with GridSearch, Decision Tree with tuning)  

### Step 4: Evaluation  
- Evaluate using Accuracy, F1-Score, ROC-AUC  
- Visualize Confusion Matrix and ROC Curves  

### Step 5: Interpretation  
- Analyze feature importance (coefficients for LR, feature_importances_ for DT)  
- Visualize Decision Tree  
- Discuss interpretability of all models  

---

## 📊 Final Comparison

| Model               | Accuracy | F1 Score | ROC AUC |
|--------------------|----------|----------|---------|
| Logistic Regression| ✅        | ✅        | ✅       |
| KNN                |          |          |         |
| Decision Tree      |          |          |         |

> ✅ Best Model: *Based on overall scores and interpretability*

---

## 📦 Requirements

Install dependencies with:

```bash
pip install -r requirements.txt
Just skip the jupyter text in reuirement.txt


---

## 🚀 How to Run the Notebook

1. **Clone this repository or download the ZIP**:
```bash
git clone https://github.com/tuhin-123/heart-disease-prediction.git
cd heart-disease-prediction

2. python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

3. pip install -r requirements.txt

4. jupyter notebook

5.Open and run the notebook file (e.g., heart_disease_analysis.ipynb) step-by-step.
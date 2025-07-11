# 📊 Summary Report: Heart Disease Prediction

---

## 🧾 Project Overview

This project aims to predict the **presence of heart disease** based on clinical and demographic data using machine learning models.  
By analyzing patterns in patient data, the system can help in **early diagnosis** and risk prediction — a vital step in preventive healthcare.

---

## 🧰 Tools & Technologies

- **Language**: Python 3.x  
- **Platform**: Jupyter Notebook  
- **Libraries**:  
  - Data: `pandas`, `numpy`  
  - Visualization: `matplotlib`, `seaborn`  
  - Modeling: `scikit-learn`  
  - Dataset: `ucimlrepo`  

---

## 📦 Dataset Details

- **Source**: UCI Machine Learning Repository  
- **Records**: 303 patients  
- **Target Variable**: `num` (0 = No heart disease, 1+ = Presence)  
- **Features**:
  - Demographic: `age`, `sex`
  - Clinical: `cp`, `trestbps`, `chol`, `fbs`, `restecg`, `thalach`, `exang`, `oldpeak`, `slope`, `ca`, `thal`

---

## 🔍 Key Questions Explored

- Which clinical features are most related to heart disease?
- What patterns or trends exist across heart disease-positive vs. negative groups?
- Which ML model performs best at prediction?
- Can we interpret the predictions and feature impacts?

---

## 🧪 Methodology

### 1️⃣ Data Acquisition & Exploration  
- Imported dataset using `ucimlrepo`  
- Visualized distributions, correlations, and outliers  

### 2️⃣ Data Preprocessing  
- Missing value handling  
- One-hot encoding of categorical variables  
- Feature scaling with `StandardScaler`  
- Train-test split (80:20)  

### 3️⃣ Model Development  
- **Logistic Regression**  
- **K-Nearest Neighbors (KNN)** with GridSearchCV for optimal `K`  
- **Decision Tree** with tuning of depth, split criteria  

### 4️⃣ Model Evaluation  
- Metrics: Accuracy, F1 Score, ROC-AUC  
- Visualizations: Confusion Matrix, ROC Curves  

### 5️⃣ Interpretation  
- Feature importance: Decision Tree & Logistic Regression  
- Tree structure visualization  
- Discussion on model explainability

---

## ✅ Model Comparison Results

| Model               | Accuracy | F1 Score | ROC AUC |
|--------------------|----------|----------|---------|
| Logistic Regression| **0.87** | **0.88** | **0.90** |
| KNN (k=9)           | 0.82     | 0.81     | 0.85     |
| Decision Tree       | 0.84     | 0.83     | 0.86     |

📌 **Conclusion**:  
**Logistic Regression** achieved the best performance while also offering better interpretability.

---

## 💡 Key Insights

- **Chest pain type**, **thalassemia**, **oldpeak**, and **max heart rate** were among the most important predictors.
- Patients with **higher ST depression** or **low thalach** are more likely to have heart disease.
- The **KNN model** performed well but is less interpretable.
- **Decision Trees** offer visual insights, but may overfit without tuning.

---

## 🛠 Recommendations

- Use **Logistic Regression** in clinical tools for risk screening.
- Further improve accuracy by combining models (ensemble techniques).
- Build a dashboard (e.g., with Streamlit) for doctor-facing prediction interface.
- Use SHAP or LIME for improved interpretability.

---

## 🧑‍💻 Author

**Tuhin Mondal**  
**Data Analysis Internship Certification Coursework – July 2025**  
📘 Project: Heart Disease Prediction
🔗 GitHub: [tuhin-123](https://github.com/tuhin-123)  
🔗 LinkedIn: [Tuhin Mondal](https://www.linkedin.com/in/tuhin-mondal)

---

## 📌 Status

✔️ Data cleaned and analyzed  
✔️ Models trained and evaluated  
✔️ Insights documented  
⏳ Deployment & dashboard integration – *optional future work*

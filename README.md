# 🧠 Breast Cancer Diagnosis Prediction using SVM

---

## 📌 Project Overview

This project is a Machine Learning model that predicts whether a breast tumor is **Malignant (Cancerous)** or **Benign (Non-Cancerous)** based on medical features.  
The model is built using **Support Vector Machine (SVM)** and achieves strong performance in classification tasks.

---

## 🎯 Objective

To build an accurate and reliable ML system that can assist in early detection of breast cancer, improving diagnosis support for healthcare applications.

---

## 📊 Dataset Information

- **Dataset:** Breast Cancer Wisconsin Dataset  
- **Total Features:** 30 numerical medical features  
- **Target Variable:**
  - `M` → Malignant (1)
  - `B` → Benign (0)

---

## 🛠️ Technologies Used

- Python 🐍  
- Pandas & NumPy  
- Scikit-learn (SVM, preprocessing, evaluation)  
- Matplotlib & Seaborn (visualization)  
- Joblib (model saving)  

---

## ⚙️ Machine Learning Pipeline

### 1. Data Preprocessing
- Removed irrelevant columns (`id`)
- Encoded target variable (`M → 1`, `B → 0`)
- Checked missing values
- Applied feature scaling using `StandardScaler`

---

### 2. Exploratory Data Analysis (EDA)
- Target distribution analysis  
- Correlation heatmap  
- Feature relationships visualization  

---

### 3. Model Training
- **Algorithm:** Support Vector Machine (SVM)  
- **Kernel:** RBF  
- **Hyperparameters:** C, gamma  

---

### 4. Model Optimization
- Used `GridSearchCV`  
- Optimized using **recall score** to reduce false negatives  

---

### 5. Evaluation Metrics
- Accuracy Score  
- Confusion Matrix  
- Classification Report  
- ROC Curve  
- AUC Score  

---

## 📈 Model Performance

- High accuracy on test data  
- Strong recall for detecting malignant cases  
- Reliable and stable classification performance  

---

## 💾 Model Saving

```python
joblib.dump(svm_model, "svm_breast_cancer_model.pkl")
joblib.dump(scaler, "scaler.pkl")

## 🔮 Prediction Example

The trained model can predict new patient data:

- **Input:** Medical features  
- **Output:**
  - Class Prediction → (0 = Benign, 1 = Malignant)
  - Probability Score  
```

---

## 📊 Visualizations

- Confusion Matrix  
- ROC Curve  
- Correlation Heatmap  
- Target Distribution Plot  

---

## 🚀 How to Run Project

### 1. Install dependencies
```bash id="md2"
pip install -r requirements.txt
```

## 🚀 How to Run Project

### 2. Run notebook
```bash id="mdfinal2"
jupyter notebook notebook/breast_cancer_classification_svm.ipynb
```

## 📁 Project Structure

```plaintext id="mdstruct2"
data/
├── raw/
models/
notebook/
visuals/
requirements.txt
README.md
```
## 📌 Future Improvements

- Apply Deep Learning models  
- Deploy using Streamlit or Flask  
- Feature selection optimization  
- Compare multiple ML algorithms  

---

## ⭐ Support

If you like this project, please consider giving it a ⭐ on GitHub. It helps support the project and motivates further improvements!

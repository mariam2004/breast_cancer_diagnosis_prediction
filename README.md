🧠 Breast Cancer Diagnosis Prediction using SVM
📌 Project Overview

This project is a Machine Learning model that predicts whether a breast tumor is Malignant (Cancerous) or Benign (Non-Cancerous) based on medical features.
The model is built using Support Vector Machine (SVM) and achieves strong performance in classification tasks.

🎯 Objective

To build an accurate and reliable ML system that can assist in early detection of breast cancer, improving diagnosis support for healthcare applications.

📊 Dataset Information
Dataset: Breast Cancer Wisconsin Dataset
Total Features: 30 numerical features
Target Variable:
M → Malignant (1)
B → Benign (0)
🛠️ Technologies Used
Python 🐍
Pandas & NumPy
Scikit-learn (SVM, preprocessing, evaluation)
Matplotlib & Seaborn (visualization)
Joblib (model saving)
⚙️ Machine Learning Pipeline
1. Data Preprocessing
Removed irrelevant columns (id)
Encoded target variable (M → 1, B → 0)
Checked missing values
Applied feature scaling using StandardScaler
2. Exploratory Data Analysis (EDA)
Target distribution analysis
Correlation heatmap
Feature relationships visualization
3. Model Training
Algorithm: Support Vector Machine (SVM)
Kernel: RBF
Hyperparameters: C, gamma
4. Model Optimization
Used GridSearchCV
Optimized using recall score to reduce false negatives
5. Evaluation Metrics
Accuracy Score
Confusion Matrix
Classification Report
ROC Curve
AUC Score
📈 Model Performance
High accuracy on test data
Strong recall for detecting malignant cases
Reliable classification performance
💾 Model Saving

The trained model and scaler are saved using joblib:

joblib.dump(svm_model, "svm_breast_cancer_model.pkl")
joblib.dump(scaler, "scaler.pkl")
🔮 Prediction Example

The model can predict new patient data:

Input: Medical features
Output:
Class (0 = Benign, 1 = Malignant)
Probability score
📊 Visualizations
Confusion Matrix
ROC Curve
Correlation Heatmap
Target Distribution Plot
🚀 How to Run Project
1. Install dependencies
pip install -r requirements.txt
2. Run notebook
jupyter notebook notebook/breast_cancer_classification_svm.ipynb
📁 Project Structure
data/
models/
notebook/
visuals/
requirements.txt
README.md
📌 Future Improvements
Try deep learning models
Deploy using Streamlit or Flask
Feature selection optimization
Compare multiple ML algorithms
👩‍💻 Author

Mariam Ahmed

⭐ If you like this project

Give it a ⭐ on GitHub to support the work!

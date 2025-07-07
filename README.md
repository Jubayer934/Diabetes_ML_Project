
# Diabetes Prediction ML Project

This project is a machine learning pipeline for predicting whether a person has diabetes using a dataset with medical features.

## 📁 Dataset
- File: `diabetes.csv`
- Source: Pima Indian Diabetes Dataset
- Features:
  - Pregnancies
  - Glucose
  - BloodPressure
  - SkinThickness
  - Insulin
  - BMI
  - DiabetesPedigreeFunction
  - Age
- Target:
  - Outcome (0 = No Diabetes, 1 = Diabetes)

## 🧪 ML Steps
1. **Data Preprocessing**:
   - Replace invalid 0s with NaN in Glucose, BloodPressure, SkinThickness, Insulin, BMI
   - Fill missing values using median

2. **Train-Test Split**:
   - 80% training, 20% testing

3. **Model Used**:
   - RandomForestClassifier from scikit-learn (diabetes)
   - GradientBoostingClassifier from sklearn (diabetes(1))

4. **Evaluation**:
   - Accuracy score 74%(diabetes) and 76%(diabetes(1))
   - Classification report (Precision, Recall, F1)
   - Confusion matrix heatmap

5. **Single Patient Prediction**:
   - Manually input values to predict diabetes outcome
   - And Check the probability score at diabetes(1)

## 🛠️ How to Run (Google Colab)
1. Upload `diabetes.csv` file using:
```python
from google.colab import files
files.upload()
```

2. Paste the provided code blocks for:
   - Data processing
   - Model training
   - Evaluation
   - Single patient prediction

## ✅ Requirements
- Python
- pandas, numpy
- scikit-learn
- seaborn, matplotlib

## 📌 Notes
- No backpropagation or epochs needed (not a neural network)
- Missing values handled via median imputation
- Good beginner-friendly ML project

## Link  

[Kaggle Dataset](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database/code)

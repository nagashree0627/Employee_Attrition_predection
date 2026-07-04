# Employee Attrition Prediction using Machine Learning

## 📌 Project Overview

Employee attrition is a major challenge for organizations as it increases recruitment costs, training expenses, and productivity loss. This project uses Machine Learning to predict whether an employee is likely to leave the company based on factors such as job satisfaction, salary, work-life balance, years at the company, and other HR-related attributes.

The objective is to help HR teams identify employees who may be at risk of leaving and support data-driven retention strategies.

---

## 🎯 Objectives

- Analyze employee attrition patterns.
- Clean and preprocess HR data.
- Perform Exploratory Data Analysis (EDA).
- Build and compare multiple Machine Learning models.
- Identify the key factors influencing employee attrition.
- Provide actionable business recommendations for HR.

---

## 📂 Dataset

**Dataset:** IBM HR Analytics Employee Attrition Dataset

- Source: https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset
- Records: **1,470**
- Features: **35**

The target variable is:

- **Attrition**
  - Yes → Employee Left
  - No → Employee Stayed

---

## 🛠 Technologies Used

- Python
- Jupyter Notebook / Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## 📊 Project Workflow

### 1. Data Loading
- Imported dataset using Pandas.
- Explored dataset structure.
- Checked dataset dimensions.
- Calculated employee attrition rate.

### 2. Data Preprocessing
- Checked for missing values.
- Removed irrelevant columns:
  - EmployeeCount
  - EmployeeNumber
  - Over18
  - StandardHours
- Converted Attrition into binary values.
- Applied One-Hot Encoding for categorical features.
- Standardized numerical features using StandardScaler.

### 3. Exploratory Data Analysis
Analyzed employee attrition with respect to:

- Department
- Job Role
- Monthly Income
- Work-Life Balance
- Years at Company

Generated business insights based on the observed patterns.

### 4. Model Building

The following classification models were trained and compared:

- Logistic Regression
- Random Forest Classifier
- Gradient Boosting Classifier

Class imbalance was handled using:

```python
class_weight='balanced'
```

---

## 📈 Model Evaluation

Models were evaluated using:

- Precision
- Recall
- F1 Score
- ROC-AUC Score
- Confusion Matrix

The best-performing model was selected based on its overall performance.

---

## 📉 Visualizations

The project includes the following visualizations:

- Attrition Rate by Department
- Monthly Income vs Attrition
- Confusion Matrix
- Top 10 Feature Importances
- ROC Curve Comparison

---

## 🔍 Key Findings

- Sales department has the highest employee attrition.
- Sales Representatives show the highest turnover among all job roles.
- Employees with lower monthly income are more likely to leave.
- Poor work-life balance is associated with higher attrition.
- Most employees who leave do so within their first few years at the company.

---

## 💼 Business Recommendations

- Prioritize retention efforts for the Sales department.
- Improve onboarding and mentoring programs for new employees.
- Review compensation policies for lower-income employees.
- Promote work-life balance initiatives to improve employee satisfaction.
- Conduct regular employee engagement and retention discussions.

---

## 📁 Project Structure

```
EmployeeAttrition/
│
├── analysis.ipynb
├── WA_Fn-UseC_-HR-Employee-Attrition-selected-columns.csv
├── README.md
│
├── charts/
│   ├── attrition_vs_departmentdepartment.png
│   ├── attrition_vs_monthlyincome.png
│   ├── ROC_curve.png
│   ├── confusion_matrix.png
│   └── top_10_feature_imp.png
│
└── summary.docx
```

---

## 🚀 How to Run

1. Clone the repository

```bash
git clone https://github.com/your-username/Employee-Attrition-Prediction.git
```

2. Install the required libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

3. Open the notebook

```bash
jupyter notebook analysis.ipynb
```

or upload the notebook to Google Colab.

---

## 📌 Future Improvements

- Apply Hyperparameter Tuning using GridSearchCV.
- Handle class imbalance using SMOTE.
- Perform cross-validation for improved model reliability.
- Deploy the model using Flask or Streamlit.
- Develop an interactive HR dashboard for real-time predictions.

---

## 👨‍💻 Author

**Naga Shree Satya Haritha Pampana**

Machine Learning Intern

---

## ⭐ Acknowledgements

- IBM HR Analytics Dataset
- Kaggle
- Scikit-learn Documentation

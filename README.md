# Loan-default-prediction-autoAI-model
Predicts if a loan applicant is likely to default using income, credit history, and loan details for risk analysis.

# 🏦 Loan Default Prediction using IBM Watson AutoAI

Built an ML model using **IBM Watson Studio's AutoAI** to predict whether a loan applicant will default. AutoAI automates the end-to-end machine learning pipeline including data preprocessing, feature engineering, model selection, and hyperparameter tuning. This project demonstrates how fast and efficient automated machine learning (AutoML) can be for solving real-world classification problems.

---

## 📚 Table of Contents
- [About the Project](#about-the-project)
- [Dataset](#dataset)
- [Technologies Used](#technologies-used)
- [AutoAI Workflow](#autoai-workflow)
- [Results](#results)
- [How to Run](#how-to-run)
- [Screenshots (Optional)](#screenshots-optional)
- [Credits](#credits)

---

## 📌 About the Project

This machine learning project leverages **IBM Watson Studio's AutoAI** to build a predictive model for loan default risk based on applicant information. With **minimal manual coding**, AutoAI handles:
- Data cleaning and transformation
- Feature engineering
- Model training and selection
- Hyperparameter tuning

The project shows how AutoAI can accelerate ML development and provide strong baseline models for credit risk prediction.

---

## 📂 Dataset

- **Name**: Loan Default Dataset  
- **Source**: (Use your dataset URL or describe how it was uploaded to IBM Watson Studio)  
- **Description**: The dataset contains borrower information used to predict loan default status.

| Column Name         | Description                              |
|---------------------|------------------------------------------|
| Loan_ID             | Unique Loan Identifier                   |
| Gender              | Male / Female                            |
| Married             | Yes / No                                 |
| Dependents          | Number of dependents                     |
| Education           | Graduate / Not Graduate                  |
| Self_Employed       | Yes / No                                 |
| ApplicantIncome     | Applicant's income                       |
| CoapplicantIncome   | Co-applicant's income                    |
| LoanAmount          | Loan amount requested                    |
| Loan_Amount_Term    | Loan term (in months)                    |
| Credit_History      | 1 = Good, 0 = Bad Credit History         |
| Property_Area       | Urban / Rural / Semiurban                |
| Loan_Status         | Target variable: Y = Approved, N = Defaulted |

---

## 🛠 Technologies Used

- IBM Watson Studio  
- AutoAI (AutoML tool by IBM)  
- IBM Cloud Object Storage  
- Python (for scoring and integration)  
- Jupyter Notebooks / Google Colab (optional)

---

## ⚙️ AutoAI Workflow

1. Upload the **Loan Default Dataset (train.csv)** to your IBM Watson Studio project.
2. Create a new **AutoAI experiment** and attach the dataset.
3. Select **target column**: `Loan_Status`
4. AutoAI performs:
   - Automated data cleaning and preprocessing
   - Feature transformation and encoding
   - Model generation using algorithms like XGBoost, Random Forest, etc.
   - Hyperparameter optimization
   - Leaderboard evaluation for model comparison
5. The **best model** is chosen based on accuracy, F1-score, and other metrics.
6. Export or deploy the model for API-based predictions.

---

## 📈 Results

- **Target Column**: Loan_Status  
- **Best Performing Model**: XGBoostClassifier (may vary based on dataset)  
- **Accuracy Achieved**: ~82–85% (varies with data quality)  
- **Key Predictors Identified by AutoAI**:
  - Credit_History
  - ApplicantIncome
  - LoanAmount
  - Property_Area
  - Education

AutoAI also provides model explainability and a leaderboard of all trained models for comparison.

---

## ▶️ How to Run

1. **Sign up** at [IBM Watson Studio](https://dataplatform.cloud.ibm.com).
2. Create a new **project**.
3. Upload the **loan dataset (train.csv)** to the project.
4. Click **Add to project → AutoAI experiment**.
5. Select your uploaded dataset and choose `Loan_Status` as the target column.
6. Run the AutoAI experiment.
7. View and compare model performance via the **leaderboard**.
8. Export or deploy the best model using REST API or Python scoring script.

---

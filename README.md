# 🏦 Beta Bank Customer Churn Prediction

## 📖 Project Overview
Beta Bank has been experiencing a steady decline in their customers. To reduce churn, the bank wants to identify customers at risk of leaving in advance. This project focuses on building a machine learning classification model that predicts customers churn based on historical behavior data. The project's main goal is to achieve the highest possible F1 score, with a minimum passing threshold of 0.59. Additionally, the AUC-ROC metric is used to evaluate the model's performance across different classification thresholds.

## 📌 Table of Contents
  - Project Description
  - Data Description
  - Installation
  - Project Workflow
  - Key Results
  - Lessons Learned
  - Credits

## 📁 Dataset Description
### Features
- `RowNumber`: Index of the row
- `CustomerId`: Unique customer ID
- `Surname`: Customer's surname
- `CreditScore`: Credit score
- `Geography`: Country of residence
- `Gender`: Customer gender
- `Age`: Age
- `Tenure`: Years with the bank
- `Balance`: Account balance
- `NumOfProducts`: Number of bank products
- `HasCrCard`: Has credit card (0/1)
- `IsActiveMember`: Activity flag
- `EstimatedSalary`: Estimated income
### Target
- `Exited`: 1 if the customer left, 0 otherwise

## ⚙️ Installation
1. Clone the repository:
   ```bash
   https://github.com/your-username/beta-bank-churn.git
   cd beta-bank-churn
2. Install required libraries:
   ```bash
   pip install -r requirements.txt
3. Run the notebook or script to train and evaluate the models.

## 🧪 Project WorkFlow
  - Exploratory Data Analysis (EDA)
  - Model Training
  - Handling Imbalance
  - Model Tuning
  - Final Testing

## 📈 Key Results
  - Among all models, best model is Random Forest Classifier. 
  - Best F1 Score on Test Set: 0.599
  - Best AUC-ROC Score on Test Set: 0.856
  - Model generalizes well with minimal overfitting.
  - Upsampling and `class_weight` tuning significantly improved performance.

## 📚 Lessons Learned
  - Feature scaling was not required for all models (e.g., decision trees).
  - Class imbalance wasn’t severe, but addressing it helped boost performance.
  - It’s important to balance model accuracy and interpretability, especially in real-world deployment.

## 🤝 Credits
This project was created as part of the TripleTen Data Science program - Supervised Learning course. Special thanks to:
  - TripleTen instructors and peers for ongoing support and feedback. 

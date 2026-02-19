# Buy-Now-Pay-Later-BNPL-Risk_Prediction
""Buy Now, Pay Later" (BNPL) risk prediction project, your GitHub description should communicate both the technical approach and the business impact"
<img src="https://github.com/rpjinu/Buy-Now-Pay-Later-BNPL-Risk_Prediction/blob/main/project_image.png">

📌 Project Overview

Pay Now & Pay Later is a Machine Learning project designed to predict customer repayment behavior in a Buy Now Pay Later (BNPL) system.

The model classifies customers into three categories:

🔴 Defaulted

🟡 Late Payment

🟢 Paid On Time

The goal of this project is to help financial institutions identify risky customers early and reduce credit loss.

🎯 Problem Statement

Financial institutions offering BNPL services face risk when customers fail to repay on time.

This project builds a multi-class classification model to predict the repayment status of customers based on financial and behavioral features.

🧠 Problem Type

Machine Learning Type: Supervised Learning

Task: Multi-Class Classification

Target Variable: Repayment_Status

Target Encoding
0 → Defaulted
1 → Late Payment
2 → Paid On Time

📊 Dataset Information
🔹 Total Records:

50,000+

🔹 Features:

7 independent variables (financial & demographic features)

🛠️ Project Workflow
1️⃣ Data Preprocessing

Identified categorical and numerical features

Applied Label Encoding for categorical columns

Saved encoders using joblib for future transformations

Split dataset into training and testing sets (80-20 split)

2️⃣ Exploratory Data Analysis (EDA)

Performed:

📊 Count plots for categorical features

📈 Distribution plots for numerical features

📉 Correlation heatmap

⚖️ Class imbalance analysis

EDA helped understand feature distribution and imbalance issues.

3️⃣ Handling Class Imbalance

The dataset was highly imbalanced.

To improve minority class detection, SMOTE (Synthetic Minority Oversampling Technique) was applied:

🤖 Models Used
1️⃣ Logistic Regression

Used as a baseline model.

2️⃣ Random Forest Classifier

Used with class weighting and SMOTE.

3️⃣ XGBoost (Recommended)

Best suited for structured tabular data and imbalance handling.

📈 Model Performance Comparison
🔹 Before SMOTE

Accuracy: 75%

Default Recall: 0.06

Macro F1-score: 0.35

Problem:
Model mostly predicted majority class (Paid On Time).

🔹 After SMOTE

Accuracy: 61%

Default Recall: 0.30

Macro F1-score: 0.41

Improvement:

Better minority class detection

More balanced predictions

Improved macro F1-score

Although accuracy decreased, minority class recall significantly improved — which is critical in financial risk prediction.

📊 Evaluation Metrics Used

Accuracy

Precision

Recall

F1-score

Macro Average

Weighted Average

Confusion Matrix

⚠️ Accuracy alone was misleading due to class imbalance.

📂 Project Structure:-

Pay-Now-Pay-Later/
│
├── data/
├── notebook.ipynb
├── label_encoders.pkl
├── repayment_model.pkl
├── README.md
└── requirements.txt

🎯 Business Impact

This model can help:

Detect potential defaulters early

Reduce financial losses

Improve BNPL approval decision-making

Strengthen credit risk management strategy

🧑‍💻 Author

Ranjan
Machine Learning & Data Science Enthusiast


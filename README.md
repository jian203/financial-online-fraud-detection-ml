# Financial Fraud Detection: Cost-Sensitive Machine Learning

## 📌 Project Overview
Digital financial fraud is a growing global challenge. This project builds an automated fraud detection system using ensemble Machine Learning algorithms (Random Forest, XGBoost, and LightGBM) trained on a synthetic financial dataset of over 6.3 million records. 

Beyond standard accuracy metrics, this project focuses on **cost-sensitive decision-making** and critically evaluates **dataset artifacts (data leakage)** to bridge the gap between theoretical machine learning and real-world business impact.

## 🎯 Key Highlights
* **Business Impact First:** Optimized model thresholds to minimize real-world financial risk, bringing the financial risk down to **Rp 21 Million** from potential hundreds of millions.
* **Critical Data Evaluation:** Identified `amount_vs_balance_orig` as a dataset artifact within the PaySim synthetic data, proving the necessity of behavioral features (like `transaction_hour`) for production environments.
* **Memory Optimization:** Performed targeted datatype downcasting (`int64` to `int32`/`int8`), drastically reducing RAM usage for handling millions of rows.
* **Explainable AI:** Utilized SHAP (SHapley Additive exPlanations) to interpret model behavior and ensure trust for non-technical stakeholders.

## 🛠️ Tech Stack
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Machine Learning:** Scikit-learn, XGBoost, LightGBM
* **Explainability:** SHAP
* **Visualization:** Matplotlib, Seaborn

## 📂 Repository Contents
* `fraud_detection_model.py`: The complete Python script detailing the pipeline from memory optimization and time-based splitting to model training and SHAP analysis.
* `Fraud_Detection_Case_Study.pdf`: A comprehensive presentation deck summarizing the methodology, evaluation metrics, and business recommendations.

## 🚀 How to Use
1. Clone this repository:
   ```bash
   git clone [https://github.com/jian203/financial-fraud-detection-ml.git](https://github.com/jian203/financial-fraud-detection-ml.git)
2. The dataset used in this project is the Online Payment Fraud Detection Dataset from Kaggle. (https://www.kaggle.com/datasets/jainilcoder/online-payment-fraud-detection)
3. Download and extract the dataset, then ensure the onlinefraud.csv file is placed in the correct directory (or update the file path in the Python script) before running the code.

## 📝 License
This project is licensed under the MIT License - see the LICENSE file for details.

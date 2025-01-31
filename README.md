**#  Fraud Detection in E-Commerce Transactions  

##  Project Overview  
This project implements a **fraud detection system** using **machine learning techniques** to identify fraudulent transactions in e-commerce platforms. The system leverages **Logistic Regression, Decision Trees, and Random Forests** to classify fraudulent and non-fraudulent transactions. Key challenges addressed include **class imbalance, evolving fraud tactics, and large-scale deployment integration**.  

Dataset  
The dataset used in this project is sourced from Kaggle:  
 **[Fraudulent E-Commerce Transactions Dataset](https://www.kaggle.com/datasets/shriyashjagtap/fraudulent-e-commerce-transactions/data)**  

## 🛠️ Installation & Setup  
To run this project locally, follow these steps:  

#1️⃣ Clone the Repository**  
bash
git clone https://github.com/Lokesh-Murugesh/Fraud-Detection.git
cd fraud-detection-ml
2️⃣ Install Dependencies
bash
pip install -r requirements.txt
3️⃣ Run the Jupyter Notebook
jupyter notebook
# Open Fraud_Detection.ipynb and execute cells
🔍 Exploratory Data Analysis (EDA)
Key fraud patterns identified:
📊 Class Imbalance: Fraud cases are significantly lower than non-fraud cases
💳 Transaction Amount: Higher-value transactions have a higher fraud probability
🕒 Fraud by Time: Certain hours of the day have higher fraud occurrences
📌 Fraud by Payment Method: Credit cards show a higher fraud rate

🏆 Model Training, Evaluation & Hyperparameter Tuning
1️⃣ Models Implemented
Logistic Regression
Decision Tree
Random Forest
2️⃣ Model Evaluation
Each model is evaluated based on Precision, Recall, F1-score, and ROC-AUC curves.

Model	Precision	Recall	F1 Score	ROC-AUC
Logistic Regression	0.96	0.12	0.21	0.559
Decision Tree	0.92	0.27	0.41	0.611
Random Forest	0.94	0.15	0.26	0.574
🔹 Conclusion: Random Forest balances fraud detection with minimal false positives.

3️⃣ Hyperparameter Tuning (GridSearchCV)
The Random Forest model was optimized using GridSearchCV with:

Best Parameters Selected:
max_depth: 10
n_estimators: 100
Post-Tuning Performance:
Accuracy: 96%
Precision: 0.96
Recall: 0.15
F1-Score: 0.61
ROC AUC Score: 0.57

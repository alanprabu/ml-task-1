📊 Customer Churn Prediction using Machine Learning
A Machine Learning project that predicts whether a customer is likely to churn based on customer information and subscription details. This project uses Python, Pandas, Scikit-learn, and a Random Forest Classifier to build and evaluate the prediction model.

📌 Project Overview
Customer churn prediction helps businesses identify customers who are likely to stop using their services. By predicting churn in advance, companies can take proactive steps to improve customer retention.

This project follows a complete Machine Learning pipeline from data preprocessing to model evaluation.

🎯 Objective
The objective of this project is to build a machine learning model that predicts customer churn using customer demographic and subscription-related features.

📂 Dataset
The dataset contains customer information such as:

Customer ID
Age
Gender
Subscription Type
Contract Length
Total Spend
Other customer-related attributes
Churn (Target Variable)
⚙️ Technologies Used
Python
Google Colab
NumPy
Pandas
Matplotlib
Seaborn
Scikit-learn
🧠 Machine Learning Workflow
1. Import Libraries
Imported required libraries for data analysis, visualization, and machine learning.

2. Load Dataset
Loaded the customer churn dataset using Pandas.

dataset = pd.read_csv("customer_churn_dataset-training-master.csv")
3. Data Preprocessing
Checked dataset information
Handled missing values
Converted numerical columns
Filled missing values using the median
Encoded categorical variables using LabelEncoder
4. Exploratory Data Analysis (EDA)
Performed data visualization using:

Churn Distribution Count Plot
Dataset Information
Statistical Summary
Libraries used:

Matplotlib
Seaborn
5. Feature Engineering
Selected input and target variables.

Features (X):
Customer Information

Target (y):
Churn
6. Train-Test Split
The dataset was divided into:

80% Training Data
20% Testing Data
using train_test_split().

7. Model Training
The project uses the Random Forest Classifier.

from sklearn.ensemble import RandomForestClassifier

clf = RandomForestClassifier(random_state=42)
clf.fit(X_train, y_train)
8. Model Prediction
Predictions are generated using:

y_pred = clf.predict(X_test)
9. Model Evaluation
The model performance is evaluated using Accuracy Score.

from sklearn.metrics import accuracy_score

accuracy = accuracy_score(y_test, y_pred)
print(accuracy)
📁 Project Structure
Customer-Churn-Prediction/
│
├── ML_Project_1.ipynb
├── customer_churn_dataset-training-master.csv
├── README.md
└── requirements.txt
📦 Required Libraries
Install the required packages using:

pip install numpy pandas matplotlib seaborn scikit-learn
Or install from requirements.txt:

pip install -r requirements.txt
🚀 How to Run
Clone this repository
git clone https://github.com/Rabinson-20/Customer-Churn-Prediction.git
Open the notebook in:
Google Colab
Jupyter Notebook
Install dependencies.

Run all notebook cells.

📈 Results
The Random Forest model successfully predicts customer churn after preprocessing and feature encoding.

Model evaluation is performed using the Accuracy Score.

🔮 Future Improvements
Hyperparameter Tuning
Cross Validation
Feature Importance Analysis
Model Deployment using Flask or Streamlit
Compare multiple ML algorithms (Decision Tree, XGBoost, SVM, Logistic Regression)

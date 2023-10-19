# Bank-Customer-Loyalty-Predictive-Analysis

Overview:
Implemented predictive modeling to identify bank customers likely to churn, contributing to the design of targeted retention campaigns. Utilized machine learning algorithms, data exploration, and feature engineering for enhanced model performance.

Project Details:

#1. Data Loading and Preliminary Analysis:
   - Loaded Bank Customer Churn dataset using pandas.
   - Conducted exploratory data analysis (EDA) to assess dataset cleanliness and structure.
   - Handled categorical variables, evaluated the need for scaling, and set customer_id as the index.

#2. Data Exploration:
   - Visualized the count of the target variable (churn) to identify data imbalance.
   - Explored the distribution of continuous and discrete variables.
   - Plotted heatmaps and pairplots to understand variable relationships.

#3. Split in Train and Test Set and Build ML Models:
   - Split the dataset into train and test sets using scikit-learn.
   - Implemented machine learning models (Logistic Regression, SVM, Random Forest, XGBoost) for binary classification.
   - Evaluated model performance using accuracy, AUC, recall, and F1 Score.

#4. Feature Engineering and Imbalance Correction:
   - Scaled numerical variables between 0 and 1 and performed one-hot encoding for gender and country.
   - Addressed data imbalance using undersampling.
   - Improved model performance for RandomForest and XGBoost.

#5. Predict which Customers to Target:
   - Selected XGBoost as the final model for its superior performance.
   - Used the trained classifier with `predict_proba` to identify customers with a 90% or higher chance of churn.
   - Prepared recommendations for targeting customers to retain.


Technologies Used:
Python, pandas, scikit-learn, seaborn, XGBoost, RandomForest

Conclusions and Key Findings:

- Identified key factors influencing customer churn, including age, product usage, and account balances.
- Discovered a significant improvement in model performance after addressing data imbalance and applying feature engineering techniques.
- Established XGBoost as the optimal model, offering the highest accuracy and reliability for predicting customer churn.
- Proposed future improvements, including addressing zero balances and exploring additional features for further model enhancement.
- The predictive models can be leveraged to proactively target high-churn-risk customers for retention efforts, ultimately reducing customer attrition.

This project has demonstrated the feasibility of using machine learning to predict bank customer churn. The XGBoost model achieved the best performance, with an accuracy of 90%. This suggests that machine learning can be used to identify customers who are at risk of churning, and that this information can be used to develop targeted interventions to retain these customers.

Future Improvements:
   - Address the presence of balances at 0 in the dataset.
   - Explore additional features for further model enhancement.
   - Conduct cross-validation for model validation.

Implications for Banks

The findings of this project have implications for banks in two main ways. First, machine learning can be used to identify customers who are at risk of churning. This information can then be used to develop targeted interventions to retain these customers. For example, banks could offer these customers special discounts or promotions, or they could reach out to them to understand their concerns and offer solutions.

Second, machine learning can be used to improve the effectiveness of marketing campaigns. Banks can use machine learning to segment their customers based on their risk of churning, and then target them with relevant marketing messages. For example, a bank could target customers who are at risk of churning with a message about a new product or service that is designed to meet their needs.


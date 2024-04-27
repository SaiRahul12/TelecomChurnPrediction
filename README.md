# Telecom Customer Churn Prediction

## Project Overview
This project focuses on predicting customer churn in the telecom industry using machine learning techniques. Customer churn, which refers to the loss of customers, is a critical problem that telecom companies face, and its prediction can aid in implementing effective retention strategies. The project utilizes a dataset from Kaggle, named "Telco Customer Churn," which provides valuable insights into customer behavior.

## Dataset
The dataset encompasses 21 features, including:

- `customerID`: Unique customer identifier
- `gender`: Customer's gender (Male/Female)
- `SeniorCitizen`: Binary indicator for seniority
- `Partner`: Binary indicator for having a partner
- `Dependents`: Binary indicator for having dependents
- `tenure`: Duration of customer subscription
- `PhoneService`: Binary indicator for having phone service
- `MultipleLines`: Binary indicator for multiple phone lines
- `InternetService`: Type of internet service (DSL, Fiber optic, None)
- `OnlineSecurity`: Binary indicator for online security subscription
- `OnlineBackup`: Binary indicator for online backup subscription
- `DeviceProtection`: Binary indicator for device protection subscription
- `TechSupport`: Binary indicator for tech support subscription
- `StreamingTV`: Binary indicator for streaming TV subscription
- `StreamingMovies`: Binary indicator for streaming movies subscription
- `Contract`: Type of customer contract (Month-to-month, One year, Two years)
- `PaperlessBilling`: Binary indicator for paperless billing
- `PaymentMethod`: Payment method (Electronic check, Mailed check, Bank transfer, Credit card)
- `MonthlyCharges`: Monthly charges incurred by the customer
- `TotalCharges`: Total charges incurred over the tenure
- `Churn`: Binary indicator for customer churn (Yes/No)

## Data Preparation
The data preparation phase includes several steps to ensure data quality and relevance for machine learning tasks:

1. **Data Cleaning**: Conversion of the 'TotalCharges' column to numerical format, removal of rows with null values, and removal of duplicate records.
2. **Handling Outliers**: Identification and replacement of outliers in the 'TotalCharges' column for churned customers.
3. **Dealing with Null Values**: Identification and imputation of missing values using appropriate strategies or removal of affected records.
4. **Encoding Categorical Variables**: Transformation of categorical variables using LabelEncoder to convert them into numerical format.
5. **Scaling Continuous Variables**: Utilization of MinMaxScaler to scale continuous variables ('tenure', 'MonthlyCharges', 'TotalCharges') to a standardized range.

## Data Visualization
The data visualization process, primarily conducted using Power BI, includes:

1. **Exploratory Data Analysis (EDA)**: In-depth exploration of data patterns, trends, and relationships, including visualization of class distribution before and after oversampling.
2. **Statistical Analysis**: Implementation of various statistical analyses, such as distributions, central tendency, hypothesis testing, and z-score, through visualizations.
3. **Boxplots for Outlier Detection**: Identification of outliers in relevant features, specifically focusing on 'TotalCharges' concerning customer churn.

## Model Training and Evaluation
The project employs various machine learning algorithms for telecom churn prediction, including:

- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting
- Extreme Gradient Boosting (XGBoost)
- AdaBoost
- K-Nearest Neighbors (KNN)
- Support Vector Machines (SVM)
- Naive Bayes

Model training involves curating a diverse dataset, partitioning it for training and testing sets, and employing these algorithms. Feature engineering and hyperparameter tuning are performed to optimize model performance.

Rigorous model evaluation is conducted using techniques such as:

- K-fold cross-validation
- Confusion matrices
- Calculation of performance metrics (e.g., accuracy, precision, recall)

## Results
The top-performing models in terms of accuracy were:

- Random Forest: 89.73%
- XGBoost: 88.78%
- Decision Tree: 87.14%

Cross-validation further validated the generalization abilities of these models, with Random Forest exhibiting the highest average cross-validation score of 90.30%.

## Conclusion
Churn prediction in the telecom industry is crucial for proactive customer retention strategies, revenue augmentation, and fostering long-term customer loyalty. This project demonstrates the application of machine learning techniques to tackle customer churn, providing telecom companies with valuable insights and predictive models to identify and mitigate potential churn effectively.

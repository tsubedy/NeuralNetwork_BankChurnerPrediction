# NeuralNetwork_BankChurnerPrediction

### Project Summary
This project focuses on building a neural network model to predict bank customer churn. Churn prediction is crucial for identifying customers likely to leave and helping the bank retain them by understanding factors driving their behavior. The project explores various features related to customers' demographics, transactions, credit card usage, and other banking interactions, using a neural network model optimized for recall.

### Key Aspects of the Project
- **Dataset**: The dataset includes various features such as customer age, income, transaction count, and credit limit, which help capture customer profiles and their likelihood to churn.
- **Primary Goal**: Predict the churn status of each customer accurately to aid retention strategies.
- **Model Selection**: Focused on maximizing recall, ensuring the model captures as many true churn cases as possible to minimize the cost of missing a customer likely to leave.

### Statistical Analysis
- **Exploratory Data Analysis (EDA)**: 
  - Conducted univariate and bivariate analyses to understand feature distributions and relationships with churn.
  - Key features analyzed include transaction count, transaction amount, credit limit, and inactivity months. 
  - The feature importance analysis revealed that transaction count, transaction amount, revolving balance, count change (Q4 to Q1), and amount change (Q4 to Q1) were among the most influential features for predicting churn.

- **Correlation Analysis**:
  - Some weak correlations were observed among features, such as a positive correlation between balance and churn. However, several features did not show strong predictive power independently.

### Data Processing and Model Building
- **Data Preprocessing**:
  - Features were encoded and scaled as necessary.
  - The dataset was balanced using SMOTE (Synthetic Minority Over-sampling Technique) to handle class imbalance.
  - Redundant features were removed, and new features were engineered to capture meaningful patterns related to churn.

- **Model Building**:
  - A neural network model was designed with SMOTE-balanced data to handle the imbalanced churn data.
  - **Model Evaluation**: Recall was chosen as the primary evaluation metric to ensure that the model minimizes false negatives in churn prediction. By focusing on recall, the model is designed to identify potential churners effectively.

### Takeaways from the Project
- **Insights for Retention Strategy**: The project highlighted key factors driving customer churn, such as transaction count and credit usage patterns, providing actionable insights for targeted retention strategies.
- **Model Performance**: A high-recall model was achieved, ensuring the identification of most churn cases, which is crucial for proactive customer retention.
- **Challenges and Improvements**: Imbalanced data required careful handling, highlighting the importance of using techniques like SMOTE for class balancing and choosing metrics aligned with business goals (e.g., recall in churn prediction).

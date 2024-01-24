Objective

The purpose of this code and analysis is to identify and predict customer churn for a bank. Churn refers to customers discontinuing their services with a company. 
* With the help of the model the bank and their marketing team can identify customers in the risk of churning and focus their marketing efforts towards these customer instead of marketing for all.
* Decreasing customer churn rate will lead to savings in the form of not having to attain new customers.
* By preventing churn the bank can both avoid the costs of new customers acquisition and also increase the overall customer lifetime value.
* This will also help the bank to use their marketing budget in the most efficient manner 


Methodologies
1. Descriptive Analysis and Exploratory Data Analysis
* Conduct descriptive analysis to understand the basic statistics of the dataset, including mean, standard deviation, minimum, and maximum values.
* Explore the distribution of categorical and continuous variables.
* Visualize the distribution of each variable using histograms and correlation heatmaps.
* Examine relationships between churn and other variables, such as salary, number of products used, age, account balance, number of usage years, and credit score.

2. Train-Test Split data
Split the dataset into training and testing sets to train and evaluate machine learning models. Standardize feature values using StandardScaler to ensure that features are on the same scale.

4. Building and Evaluating Models
* **Logistics Regression**: Simple and interpretable. Can serve as a baseline model
* **Decision Tree**: Simple and interpretable, and easy to visualize for presenting result
* **Random Forest**:  Ensemble method, Resistant to overfitting
* **Support Vector Machine**: Able to find complex decision boundaries and able to handle non-linear relationships

5. Model processing:
* Run 4 models on original dataset and rebalanced data set (with SMOTE)
* Each model get optimized to reach highest performance
** Hyperparameter tuning is done for Decision tree, Random Forest and SVM
** Regularization is done for Logistic Regression
* Best model is selected based on the combination of metrics including precision, recall, F1-score and accuracy

6. Model Evaluation
Evaluate the models by comparing confusion matrices, ROC curves, and AUC scores and focus on recall as it measures the ability to predict true positives (churn cases).


# Loan Repayment Prediction Using Ensemble Learning  

## **Project Overview**  
This project uses ensemble machine learning methods to predict whether a loan applicant is likely to fully repay their loan. By analyzing features like credit policy, interest rate, income, and financial history, the model provides insights to help banks and financial institutions make informed lending decisions.  

## **Objective**  
The goal of this project is to classify loan applicants into two categories:  
1. Fully repaid loans.  
2. Not fully repaid loans.  

The prediction is achieved using various ensemble learning algorithms, such as Decision Trees, Random Forest, Bagging, AdaBoosting, and Gradient Boosting.  

## **Dataset**  
- The dataset consists of 9,578 entries with 14 features, including credit policy, loan purpose, interest rate, FICO score, debt-to-income ratio (DTI), and more.  
- **Target Variable**: `not.fully.paid` (binary: 0 for repaid, 1 for not repaid).  
- No missing values were found in the dataset, ensuring consistency in analysis.  

## **Tools and Libraries Used**  
- **Programming Language**: Python  
- **Libraries**:  
  - Data manipulation: `pandas`, `numpy`  
  - Visualization: `matplotlib`, `seaborn`  
  - Machine Learning: `sklearn`  

## **Workflow**  

### 1. **Data Preprocessing**  
- Encoded categorical variables (e.g., `purpose`) using `LabelEncoder`.  
- Visualized key relationships between features and target variable (e.g., FICO score vs. repayment).  

### 2. **Exploratory Data Analysis (EDA)**  
- Analyzed feature distributions and correlations using heatmaps and scatter plots.  
- Identified strong predictors, such as FICO score, credit policy, and interest rate.  

### 3. **Model Development**  
- Split the data into training (70%) and testing (30%) sets.  
- Trained the following models:  
  - **Decision Tree**: Achieved ~84.58% accuracy.  
  - **Random Forest**: Identified as the best-performing model with ~85% accuracy.  
  - **Bagging and Boosting Algorithms**: Bagging and AdaBoost provided comparable results, with ~84-85% accuracy.  

### 4. **Evaluation Metrics**  
- Used accuracy, precision, recall, and F1-score to evaluate model performance.  
- Random Forest outperformed others with the best combination of metrics.  

## **Results**  
- The Random Forest model achieved the highest accuracy of 85%, making it the most reliable for predicting loan repayment.  
- Insights from the analysis indicated that higher FICO scores and lower interest rates correlate strongly with successful loan repayments.  

## **Key Challenges**  
- Balancing the dataset to handle class imbalance for the `not.fully.paid` target variable.  
- Ensuring robust feature selection to improve model generalization.  

## **Conclusion**  
This project highlights the power of ensemble learning techniques in financial risk assessment. By implementing advanced machine learning workflows, financial institutions can mitigate risks and make more informed lending decisions.  

## **Usage**  
- Clone the repository:  
  ```bash  
  git clone <repository_url>  
  ```  
- Run the Python script to preprocess data, train models, and evaluate predictions.  

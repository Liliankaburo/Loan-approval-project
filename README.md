

# BANK LOAN APPROVAL CLASSIFICATION PROJECT




![image](https://github.com/user-attachments/assets/d442592b-7300-435e-ae29-e0243155fe20)


# OVERVIEW

In today's fast-paced financial world, banks and lenders face mounting pressure to make quick and accurate decisions about loan applications. The old-school method of manually evaluating loans, which relies heavily on human judgment and subjective criteria, tends to be slow, prone to mistakes, and inconsistent. To tackle these issues, many financial institutions are now embracing data-driven strategies, particularly machine learning, to streamline and improve the loan approval process.

The Bank Loan Approval Classification Project is designed to develop a machine learning model that predicts whether a loan application should be approved or rejected based on a set of features related to the applicant's financial history, personal information, and other relevant criteria. The objective is to build a classification model that can assist bank decision-makers by providing quick, objective, and accurate recommendations for loan approval.


# BUSINESS UNDERSTANDING

## Stakeholders

1. Banks/ lending institution

2. Risk management department

3. Loan Officers/ Underwriting Team

4. Customers/ Loan Applicants

5. External Regulators (government agencies)

## Business Problem

1. What is the main challenge of this project?---How can we create a predictive model to classify loan applications as either approved or denied?

2. What key factors should the model take into account when deciding on loan approvals?---How can we include various factors such as income, credit score, loan amount, and employment status into the model to mirror the bank’s decision-making process?

3. What data do we have available for training the model?---What features of the loan applicants (e.g., age, education level, credit history) are present in the dataset, and how do they correlate with loan approval status (approved or denied)?

4. How can machine learning techniques be applied to address this issue?---How can we utilize machine learning methods to develop a model that accurately predicts whether a new loan application will be approved or denied?

5. What is the main objective of this project?---How can we automate the loan approval decision-making process by developing a predictive model, and what level of accuracy is necessary for practical implementation?


# DATA UNDERSTANDING

## Data Source

The Dataset we are using is obtained from https://www.kaggle.com/datasets/. The Bank loan approval dataset contains information about the loan Applicants that will be used to determine if they get approved for a new loan or not.

we are going to use this dataset to;

1. Develop predictive models to classify loan applications as approved or denied.

2. Analyze key factors that influence loan approval decisions.

3. Improve the efficiency and accuracy of loan approval processes through data-driven insights.

4. We are going to use python pandas,numpy and other python libraries to explore and understand the data more.

## Data Description

The Loan approval dataset has 45,000 rows and 13 columns some of which are numerical and others categorical. We are going to use the 'loan_status' column as the target(y-variable) and the rest as features (exogenous variables) in our model.

# EXPLORATORY DATA ANALYSIS

## 1. Investigating the correlation of our features in the dataset

![image](https://github.com/user-attachments/assets/9bee27a1-b71f-4093-bdc5-81cfb541ea35)

## 2. Distribution of loan_status (target variable)

![image](https://github.com/user-attachments/assets/3e4ad18d-d262-480f-be54-72afdbb4114d)

## 3. Investigating how loans were awarded across different genders

![image](https://github.com/user-attachments/assets/3c4309f4-cb50-4c79-9ff3-6dee7fee412e)

## 4.  Investigating if personal education Determines the loan status

![image](https://github.com/user-attachments/assets/ac4adff8-c397-4f0c-9f00-c69a2dd97da1)


# DATA PREPROCESSING

1. Handling categorical Variables
2. Handling high correlation
3. Feature scaling
4. Data splitting

# BUILDING THE MODELS

## Models built
1. Logistic Regression model
2. decision Tree
3. RandomForestClassifier
4. KNearestNeighbours
5. GradientBoosting Model

# CONCLUSION

By leveraging machine learning models for loan approval classification, financial institutions can improve the speed, accuracy, and fairness of their loan decision-making process. The chosen model will provide a reliable and scalable way to assess loan applications, ultimately benefiting both the bank and its customers by enhancing decision-making efficiency and reducing risks associated with loan defaults.

# RECOMMENDATIONS

## Best model recommendations based on performance

1. Random Forest performs the best in terms of accuracy (92.81%), precision (90%), recall (77%), and F1-Score (83%). This makes it the most balanced model for loan approval recommendations, providing a strong prediction for loan approvals while minimizing false positives.

2. Gradient Boosting is a close second. Its accuracy (92.19%), precision (87%), and recall (76%) are also very strong, but it slightly lags behind Random Forest in recall for class 1.

3. The Decision Tree model has a slightly lower precision (78%) and F1-score (78%) for class 1, meaning it might predict more false positives. However, it still performs well in recall (77%) for class 1.

4. KNN shows the lowest recall (70%) for class 1, meaning it misses many loan approvals. It performs well in terms of precision, but the lower recall makes it less ideal for prioritizing loan approvals.

##  Business Recommendations on the models

A primary business goal is to approve loans for as many deserving applicants as possible (minimize false negatives), while maintaining reasonable control over the number of wrongly approved loans (minimize false positives).Given the goal of loan approval prediction, the business objective is likely to prioritize approving loans for suitable applicants while minimizing financial risk.

1. Objective: Prioritize Loan Approvals

Random Forest strikes a good balance between precision (90%) and recall (77%) for loan approvals, ensuring that it doesn't      miss many potential loan approvals while still keeping false approvals (false positives) under control.
High Accuracy: With an accuracy of 92.81%, it performs reliably across the board.
Specificity: With a 97% specificity, it effectively minimizes false positives, ensuring fewer loans are wrongly approved.Ideal for businesses aiming to prioritize loan approvals without overly compromising on quality.
   
2. Objective: Minimize Financial Risk (Reduce False Approvals)

Gradient Boosting has High Specificity (97%): Like Random Forest, Gradient Boosting has excellent specificity, meaning fewer false positives and ensuring the model is cautious about approving loans.
Good Precision (87%): While its precision is slightly lower than Random Forest, it still provides strong performance in correctly identifying loan approvals.

Lower Recall for Class 1: If minimizing false approvals is more important than identifying every single potential loan-approved applicant, Gradient Boosting is an excellent choice due to its conservative approach.Ideal for businesses that want to ensure a higher level of certainty in loan approvals, even if it means missing some approvals.

3. Objective: Simplicity and Ease of Use

If the business wants a simpler, less computationally expensive model, KNN can be considered.It is relevant in smaller businesses, startups where interpretability and simplicity are paramount.

KNN is easy to understand and doesn’t require complex tuning or heavy computational resources.
Moderate Precision (81%): KNN is decent in precision but struggles with lower recall (70%), meaning that it misses a significant number of loan approvals.
Accuracy: With 89.71% accuracy, KNN works reasonably well, but its lower recall for loan approvals makes it less ideal for scenarios where maximizing loan approvals is important.
Ideal for businesses with resource constraints and a need for simplicity, but less ideal for businesses where accuracy and minimizing missed opportunities are critical.

# REFERENCES

1. W3schools https://www.w3schools.com/

2. Datacamp https://www.datacamp.com/

3. Moringa School Instructure Canvas(you have to be a student at Moringa to access this)

4. YouTube tutorials https://www.youtube.com/watch?v=XmSlFPDjKdc&t=905s

5. Github Repositories https://github.com/

6. kaggle datasets and kaggle code https://www.kaggle.com/

7. Python Documentations https://docs.python.org/3/

8. Chatgpt 4.0 https://chatgpt.com/ (when all else fail get this tool to debug)




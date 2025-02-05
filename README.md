# Predicting-Credit-Worthy-Applicants-With-Python
Machine learning, Big Data Analysis

Overview

This project aims to develop a predictive model to determine which credit applicants should be approved for a loan. Using machine learning techniques, specifically Decision Tree and Naive Bayes classifiers, the model helps bank managers make informed lending decisions.

Team Members

Aidan Kowolik - Data Exploration and Preparation

Matthew Lee - Predictive Modeling (Decision Tree)

Kai Lu - Predictive Modeling (Naive Bayes) and Further Exploratory Analysis

Problem Statement

Which credit customers should get approval for a loan?

Task

Recommend a strategy based on available attributes to assist bank managers in deciding whether to approve a loan for new applicants.

Conclusion

The WEKA-based Naive Bayes model using four attributes performed the best while satisfying model objectives.

Data Exploration and Preparation

Check for missing data

Complete distributional analysis

Detect and handle notable data outliers

Data Preparation Highlights

Most fields in the dataset are qualitative despite their quantitative nature.

Focused on preparing data for numeric fields.

Outliers in Credit Amount were removed from the dataset.

Predictive Modeling Approach

Conservative approach: Prioritize precision to reduce the risk of approving bad credit applicants.

Minimizing data fields: Limiting the number of fields allows for faster response times.

Predictive Modeling Methods

Decision Tree Method

Predicts the value of a target variable using decision rules inferred from data features.

Key predictive variables:

Account balance

Value of savings/stocks

Payment status of previous credit

Duration of credit

Age

Guarantors

Naive Bayes Method

Uses conditional probability to predict class labels.

Key predictive variables:

Account balance

Payment status of previous credit

Duration of credit

Predictive Modeling Results

Model

Precision

Accuracy

Recall

Pre-prepared data (Baseline, n=300)







Decision Tree

0.70

0.65

0.80

Naive Bayes

0.76

0.75

0.90

Prepared data (n=293)







Decision Tree

0.82

0.75

0.81

Naive Bayes

0.84

0.76

0.81

Removing outliers improved precision.

Naive Bayes slightly outperformed Decision Tree.

Model Refinement

The best-performing model used four key variables:

Account Balance

Duration of Credit

Payment Status of Previous Credit

Value Savings/Stocks

Recommendations

Apply Naive Bayes classification based on the key variables.

Further training of the model is required.

Expand the dataset with more numeric fields to allow the model to optimize classification performance.

Model Development and Selection Process

Run Decision Tree and Naive Bayes classifiers using the WEKA application.

Train and test the model using a 70/30 train-test split on raw and prepared datasets.

Choose the classification model and refine it by reducing variables where possible.

Evaluation Metrics

Precision was prioritized due to the risk-averse nature of traditional loan businesses.

True Positive (TP) and False Positive (FP) rates were key considerations.

Linear Regression analysis was performed but was deemed unsuitable due to a low R-squared value.

Exploratory Analysis

Correlation Matrix (sk-learn): Identified the most relevant attributes related to credit approval.

Linear Regression (R Studio): Used to explore variable relationships but not selected for the final model.

Technologies Used

Python (for data analysis and modeling)

WEKA (for Naive Bayes and Decision Tree classifiers)

R Studio (for linear regression analysis)

scikit-learn (for correlation matrix and exploratory analysis)

Future Improvements

Incorporate more diverse data points to improve model robustness.

Experiment with additional machine learning models (e.g., Random Forest, SVM).

Fine-tune hyperparameters to further optimize predictive performance.


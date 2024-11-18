# credit-risk-classification

# Overview of the Analysis
What was the purpose?

The purpose of this analysis was to create and evaluate machine learning modules to classify loans as either healthy loans (0) or high-risk loans (1) based on the provided historical financial data. I aimed to assist financial institutions in identifying potentially high-risk loans to reduce financial losses. 

The dataset contains different types of financial information; loan performance metrics and borrower details. I primarily wanted to predict whether a loan would be healthy or high-risk based on these features. 

Here are the target variables: 
-0: Healthy Loan
-1: High-Risk Loan

The Machine Learning Process:
My machine learning pipeline followed these stages-

-Data Preparation: Cleaning and preproccessing the dataset. This includes scaling features and splitting data into training and testing sets.

-Model Selection: Logistic Regression is the primary algorithm that was used due to its simplistic nature and interpretability for binary classifications.

-Evaluation: I assessed the model's performance using a confusion matrix, classification report, and metrics like accuracy, precision, recall, and F-1 score.


# Results

Machine Learning Model : Logistic Regression
-Accuracy: 99.4%
-Precision:
    -For 0 (healthy loans): 99.8%
    -For 1 (high-risk loans): 84.1%
-Recall:
    -For 0: 99.4%
    -For 1: 94.2%
-F-1 Score:
    -For 0: 100% 
    -For 1: 89%

Other Observations:
The model performed well overall, with high accuract and recall for both classes. But precision for 1 (high-risk loans), was slightly lower and indicates that the model tends to classify some healthy loans as high-risk.


# Summary
Best performing Model?
The logistic regression model performed very well and is definitely recommended for use. It has the ability to identify high-risk loans (1) with 94.2% recall. This makes it a valuable model for minimizing finanical losses by identifying the most risky loans.

Target Classes?
Since the primary goal is to avoid financial losses, predicting high-risk loans (1), is more critical. This would mean that the recall for 1 is the most important piece of information to look at. If we want to avoid unnecessary loan rejections, improving the precision for 1 should be looked at first.

Recommendations!
The logistic regression model is suitable for the task at hand. But depending on the institution's most critical tasks, cost-sensitive learning or precision tuning could provide further effectiveness for the model on high-risk loan predictions.
# employee-leaving-prediction
Employee Retention Analysis
This project aims to understand the factors influencing employee retention using a dataset of employee attributes. We perform exploratory data analysis (EDA) and apply logistic regression to identify the key variables impacting whether employees leave the company or stay.

Table of Contents
Dataset
Preprocessing
Exploratory Data Analysis
Logistic Regression Model
Evaluation
Results
Dependencies
Usage
Conclusion
Dataset
The dataset contains information on 14,999 employees with the following columns:

satisfaction_level: Employee satisfaction level (float)
last_evaluation: Last evaluation score (float)
number_project: Number of projects (int)
average_montly_hours: Average monthly working hours (int)
time_spend_company: Years spent in the company (int)
Work_accident: Whether the employee had a work accident (int, binary)
left: Whether the employee left the company (int, binary)
promotion_last_5years: Whether the employee was promoted in the last five years (int, binary)
Department: Employee's department (categorical)
salary: Employee's salary level (categorical)
Preprocessing
Convert categorical variables (Department and salary) into dummy/indicator variables.
Standardize the feature variables to ensure they are on a similar scale.
Split the data into training and testing sets.
Exploratory Data Analysis
We performed EDA to understand the distribution and relationships of various features. Key analyses include:

Summary statistics and data type checks.
Histograms and boxplots for univariate analysis.
Boxplots and countplots for bivariate analysis with the target variable left.
Correlation matrix to identify relationships between numeric variables.
Logistic Regression Model
We applied a logistic regression model to predict employee retention:

Fit the model on the training data.
Extract and interpret the model coefficients to understand the impact of each feature.
Evaluation
We evaluated the model using various metrics:

Accuracy: Proportion of correct predictions.
Precision: Proportion of positive identifications that were actually correct.
Recall: Proportion of actual positives that were correctly identified.
ROC-AUC Score: Area under the receiver operating characteristic curve.
Confusion Matrix: To visualize true positives, true negatives, false positives, and false negatives.
Results
Key findings from the logistic regression model:

satisfaction_level: Negative correlation with leaving, indicating higher satisfaction reduces turnover.
average_montly_hours: Positive correlation with leaving, indicating higher working hours increase turnover.
time_spend_company: Slight positive correlation with leaving, suggesting longer tenure slightly increases turnover.
Department_sales: Employees in sales are more likely to leave compared to the reference department.
Dependencies
The project requires the following Python packages:

pandas
numpy
matplotlib
seaborn
scikit-learn
Usage
Ensure all dependencies are installed.
Load the dataset into a pandas DataFrame.
Run the preprocessing steps.
Perform exploratory data analysis.
Fit the logistic regression model.
Evaluate the model's performance.
Interpret the results and make actionable insights.
Conclusion
This analysis helps in understanding the factors affecting employee retention. By focusing on key areas such as employee satisfaction and workload management, companies can develop strategies to reduce turnover and improve employee retention.

By following this README, you can reproduce the analysis and gain insights into employee retention factors.

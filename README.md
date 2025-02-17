# Retail-Sales-Prediction-

# Problem Statement
Rossmann operates over 3,000 drug stores across 7 European countries. Currently, store managers rely on their own predictions for daily sales, leading to varying levels of accuracy. The objective of this project is to develop a machine-learning model that can forecast the "Sales" column for the test set. The dataset provided includes historical sales data for 1,115 Rossmann stores, taking into account factors such as promotions, competition, school and state holidays, seasonality, and store locality. It is worth noting that some stores in the dataset were temporarily closed for refurbishment.

# Project Summary
The Rossman Sales Prediction project involved extensive data analysis, feature engineering, and model selection to accurately forecast sales. Here is a brief overview of the project steps and key findings:

- Data Gathering and Cleaning:
Collected historical sales data for Rossmann stores, including competitor details, holidays, customer count, and daily sales.
Performed data cleaning to handle missing values and ensure data consistency.
Merged relevant datasets to enhance the feature set.

- Exploratory Data Analysis (EDA):
Conducted in-depth EDA by exploring univariate, bivariate, and multivariate relationships.
Generated insightful visualizations to uncover patterns and trends in the data.
Extracted meaningful insights to inform future decision-making in the machine learning pipeline.

- Feature Engineering and Preprocessing:
Created additional features such as PromoDuration and CompetitionDuration to capture relevant information.
Addressed multicollinearity among independent variables using variance inflation factor (VIF) analysis.
Detected and treated outliers using the Interquartile Range (IQR) technique.
Encoded categorical variables using One-Hot Encoding for compatibility with machine learning algorithms.
Applied various transformation techniques to achieve normal distribution of data.

- Model Selection and Training:
Split the preprocessed data into training and testing sets.
Utilized a variety of machine learning algorithms, including linear regression, decision trees, random forests, and XGBoost.
Evaluated model performance using metrics such as R-squared score, accuracy, and mean absolute percentage error (MAPE).
Employed regularization techniques (e.g., Lasso, Ridge, Elastic Net) for improved model performance.
Identified XGBoost as the optimal model due to its high accuracy, with a MAPE of only 2% and an R-squared score of 0.94.

- Conclusion:
In Linear Regression we got the accuracy of ~93% and the model is capturing 75% of variance even after using regularization techniques that means our data is not perfectly linearly dependent with target variable(Sales).
For Decsion Tree we have achieved ~96.3% accuracy with maximum depth of 18 and on increasing the depth over it we are falling towards overfitting and MAPE of 3.6% which ultimately increases the mean absolute percentage error.
Giving preference to each of the variable always results in better accuracy as small subsets can provide significant accuracy percentage. Ensemble technique i.e Random Forest has given the accuray of ~96.96% with total trees of 100 in the forest with hyperparameter tuning.
At last we have implemented our final model i.e XGboost and achieved the accuracy of 97% with mean absolute percentage error of only 2%. Also we got the mean and median of residuals at 0.09 which is indicating towards excellent residual plot.

This project showcases the effective utilization of data analysis, feature engineering, and machine learning techniques to solve a real-world forecasting problem. The insights gained from the analysis provide valuable information for decision-making within the retail industry.

For complete project video explaination and to downoad the dataset: https://drive.google.com/drive/folders/1BzDNIaN6IDLr3u58tUhfwHV5-bIs8GYG?usp=drive_link

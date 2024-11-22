# Project Overview

This project aims to analyze the relationship between fields of study and occupations, focusing on predicting job changes. The analysis leverages machine learning techniques to build a predictive model that can assist in HR analytics and career development.

Objectives

Explore feature engineering techniques to understand factors influencing job changes.
Build predictive models to analyze career development trends.
Enhance machine learning skills through practical application.

Dataset Description

The dataset used for this analysis is titled "Career Change Prediction Dataset". It contains various features related to individuals' fields of study, current occupations, demographic information, and factors influencing career changes. Key features include:
Field of Study
Current Occupation
Age
Gender
Years of Experience
Education Level
Industry Growth Rate
Job Satisfaction
Work-Life Balance
Job Opportunities
Salary
Job Security
Career Change Interest
Skills Gap
Family Influence
Mentorship Available
Certifications
Freelancing Experience
Geographic Mobility

Methodology

Data Preprocessing

Loading the Dataset: The dataset was loaded using Pandas.
2. Handling Missing Values: Missing values were filled using forward fill (ffill) to ensure continuity in the dataset.
3. Encoding Categorical Variables: Categorical variables were converted to numerical format using one-hot encoding to facilitate model training.
Feature Engineering
New features were created based on existing data, such as converting categorical variables into numerical representations.
The target variable, "Likely to Change Occupation," was ensured to be in numeric format.

Exploratory Data Analysis (EDA)

Visualizations were created to understand the distribution of occupations and the likelihood of changing occupations based on gender.
Key insights were drawn from the visualizations to inform feature selection for the model.

Model Building

The dataset was split into training and testing sets (80% training, 20% testing).
A Random Forest Classifier was chosen as the predictive model due to its robustness and ability to handle categorical data effectively.
The model was trained on the training dataset.

Model Evaluation

The model's performance was evaluated using metrics such as precision, recall, F1-score, and accuracy.
A confusion matrix was generated to visualize the model's predictions.

Results

The model achieved the following performance metrics:
              precision    recall  f1-score   support

           0       1.00      1.00      1.00      3212
           1       1.00      1.00      1.00      4477

    accuracy                           1.00      7689
   macro avg       1.00      1.00      1.00      7689
weighted avg       1.00      1.00      1.00      7689

Confusion Matrix:
[[3211    1]
 [   0 4477]]

Interpretation of Results

The model achieved perfect precision, recall, and F1-scores for both classes, indicating that it correctly classified all instances in the test set.
The accuracy of the model was 100%, suggesting that the model is highly effective in predicting whether individuals are likely to change occupations.

Conclusion

The analysis successfully demonstrated the relationship between fields of study and occupations, with a highly accurate predictive model. The results indicate that the model can be a valuable tool for HR analytics and career development.

Future Work

Explore additional machine learning algorithms to compare performance.
Investigate the impact of additional features or external datasets on model accuracy.
Conduct a deeper analysis of the factors influencing job changes to provide actionable insights for career development.

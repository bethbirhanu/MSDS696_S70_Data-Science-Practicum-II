# MSDS696_S70_Data-Science-Practicum-II

## Abstract
This project uses traffic crash data provided by the Colorado Department of Transportation, covering the years 2007 to 2022. The aim is to employ advanced data analytics and machine learning techniques to identify patterns, predict crash severities, and recommend interventions for improving road safety. Through comprehensive data manipulation, feature engineering, and predictive modeling, this study provides insights into the factors contributing to traffic accidents and proposes data-driven solutions to mitigate them.
## Introduction
Road safety is a major concern globally, with traffic accidents leading to significant human and economic losses. This project aims to analyze detailed traffic crash data to understand the dynamics and causes of road accidents in Colorado. By applying data science techniques, the study seeks to uncover underlying patterns that could inform better traffic management and safety measures.
## Data Description
The dataset consists of traffic crash records from 2007 to 2022, including over 1.5 million individual records. Each record contains details such as the date, time, location, severity of the crash, weather conditions, road conditions, and involved entities like vehicles and pedestrians and a lot more. 
## Methodology
### Data Preparation
The data was first cleaned and preprocessed, which included handling missing values, removing duplicates, and correcting inconsistencies in the dataset structures between different years. Key steps included:
- Merging datasets from 2007-2020 and 2021-2022 after aligning their structures to use the first set of datasets which is from 2007-2020 for model training and the other for model testing.
- Renaming and one-hot encoding categorical variables for consistency.
- Addressing class imbalances using the Synthetic Minority Over-sampling Technique (SMOTE).
### Exploratory Data Analysis (EDA)
- Generated visualizations such as bar charts and graphs to understand the frequency and nature of crashes by various dimensions such as time, weather conditions, and road types.
### Predictive Modeling
Deployed several machine learning models to predict crash severity:
- Decision Tree: Utilized for its strength and ability to handle unbalanced data.
- Logistic Regression: Provided a baseline for performance comparison.
- LightGBM and Decision Tree Classifier: Explored for their efficiency and interpretability.
- Naive Bayes: Tested for its simplicity and speed in baseline modeling.
### Model Evaluation
- Conducted a thorough evaluation using metrics such as accuracy, precision, recall, F1-score, and ROC curves.
- Performed hyperparameter tuning using RandomizedSearchCV to optimize model performance.
## Challenges and Solutions
### Data Inconsistency and Missing Values
Challenge: The datasets from different years had inconsistent formats and significant missing values, which complicated preprocessing and time consuming.
Solution: Standardized the data structure across all years and applied multiple imputation techniques to handle missing data effectively.
### Class Imbalance
Challenge: The severe imbalance between different severity classes of crashes skewed initial model predictions towards the majority class.
Solution: Implemented SMOTE to artificially balance the dataset, which enhanced model performance in predicting minority classes.
### High Dimensionality
Challenge: The initial feature set was very large, leading to model overfitting.
Solution: Utilized feature selection techniques like SelectKBest based on the ANOVA F-test to identify and retain the most impactful features.
## Results and Mitigations
The analysis revealed several key insights:
- Temporal Patterns: Higher crash frequencies during peak hours and summer months.
- Weather and Road Conditions: Most crashes occurred under clear weather conditions, contradicting the expected higher incidence in adverse conditions.
- Impact of Alcohol and Drugs: Significant correlation between alcohol involvement and crash severities.
## Recommended Mitigations Based on Analysis
- Enhanced Monitoring and Enforcement: Increased surveillance and law enforcement during peak times and months identified as high-risk.
- Public Awareness Campaigns: Targeted campaigns to raise awareness about the risks of driving under clear weather conditions and the significant impact of alcohol and drug use on road safety.
- Infrastructure Improvements: Modifications in road design and maintenance, especially in high-risk areas, to improve safety.
- Policy Adjustments: Implement stricter regulations and penalties for DUI offenses as part of a broader strategy to reduce alcohol-related crashes.
## Conclusion
This project demonstrated the applicability of data science in improving road safety through detailed data analysis and predictive modeling. By integrating various data science techniques, it was possible to derive actionable insights and develop models that can predict crash severity with high accuracy, thereby supporting the implementation of effective road safety measures.
Future Work
Further research could explore the integration of real-time data for dynamic risk assessment and the use of more granular geographic data to enhance predictive accuracies. Additionally, deploying these models in a real-time predictive system could be explored to provide immediate insights for traffic management and emergency response teams.


![Picture1](https://github.com/bethbirhanu/MSDS696_S70_Data-Science-Practicum-II/assets/110367402/a23b1853-8360-4d99-987a-3a9857541116)
![Fatalities](https://github.com/bethbirhanu/MSDS696_S70_Data-Science-Practicum-II/assets/110367402/72c32e5f-0b89-4a76-bf53-ee45468aa978)
![by crash type](https://github.com/bethbirhanu/MSDS696_S70_Data-Science-Practicum-II/assets/110367402/776842a8-7a40-4593-845b-2ea66c010139)
![3](https://github.com/bethbirhanu/MSDS696_S70_Data-Science-Practicum-II/assets/110367402/0aca20fc-0c60-43bf-90de-027513279504)
![2](https://github.com/bethbirhanu/MSDS696_S70_Data-Science-Practicum-II/assets/110367402/c1c037f2-efcd-4437-bed2-29f9d986c581)
![1](https://github.com/bethbirhanu/MSDS696_S70_Data-Science-Practicum-II/assets/110367402/63b0895e-c44b-43fb-a37b-070c2fc0dadc)



![day distribution 2021-2022](https://github.com/bethbirhanu/MSDS696_S70_Data-Science-Practicum-II/assets/110367402/a2488c08-ea3d-458e-9236-100d7cd0c66b)
![day distribution 2007-2020](https://github.com/bethbirhanu/MSDS696_S70_Data-Science-Practicum-II/assets/110367402/8abdac0e-e06c-4a55-a4b4-1a31aa91369c)
![weather 2021-2022](https://github.com/bethbirhanu/MSDS696_S70_Data-Science-Practicum-II/assets/110367402/53a59fb2-e244-42e4-97dd-6ddc08fc123b)
![weather 2007-2020](https://github.com/bethbirhanu/MSDS696_S70_Data-Science-Practicum-II/assets/110367402/d1d30bce-72e0-4ca0-91ea-79ca774fa92b)
![system type 2021-2022](https://github.com/bethbirhanu/MSDS696_S70_Data-Science-Practicum-II/assets/110367402/48beac6e-c2e8-4785-849f-129562b301fb)
![system type 2007-2020](https://github.com/bethbirhanu/MSDS696_S70_Data-Science-Practicum-II/assets/110367402/15313aa1-d6dc-4500-b810-bdb8437fbf39)
![Road condition 2021-2022](https://github.com/bethbirhanu/MSDS696_S70_Data-Science-Practicum-II/assets/110367402/a8d1630d-984f-445b-9282-6cda4015e10f)
![Road condition 2007-2020](https://github.com/bethbirhanu/MSDS696_S70_Data-Science-Practicum-II/assets/110367402/4dcc0ed3-0fdd-4680-83ad-b162fb2f7ba0)
![Lighting 2021-2022](https://github.com/bethbirhanu/MSDS696_S70_Data-Science-Practicum-II/assets/110367402/f4161a42-d485-44f8-adfd-cc15c21e89c1)
![Lighting 2007-2020](https://github.com/bethbirhanu/MSDS696_S70_Data-Science-Practicum-II/assets/110367402/0ec07d09-a921-44cb-8283-775fc359b51a)



References

- Colorado Department of Transportation: Traffic Crash Data
- Scikit-Learn Documentation
- LightGBM Documentation




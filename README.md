# Microsoft : Classifying Cybersecurity Incidents with Machine Learning

## Project Objective

This project aims to enhance the efficiency of SOCs by developing a machine learning model capable of accurately predicting the triage grade of cybersecurity incidents. By leveraging the comprehensive GUIDE dataset, the model will classify incidents into three categories: True Positive (TP), Benign Positive (BP), and False Positive (FP). This classification will empower guided response systems to provide SOC analysts with precise, context-rich recommendations, ultimately improving incident response times and the overall security posture of enterprise environments.

## Methodology

**Data Exploration and Understanding:**
  Initial Inspection: Load and examine the train dataset (train.csv) to understand the structure, data types, and distribution of the target variable.

**Data Preprocessing:**
  Cleaning and transforming raw data into useful features for model training.

**Exploratory Data Analysis (EDA):**
  Visualizations and statistical summaries to identify patterns, correlations, and potential anomalies in the data.

**Encoding Categorical Variables:**
  Converting categorical features into numerical representations using techniques like one-hot encoding, label encoding, depending on the nature of the feature and its relationship with the target variable.

## Model Building

**Train-Validation Split:**
  Split the data into training and validation sets for effective model evaluation.
  
**Model Selection and Training:**
  Experimentation with various machine learning algorithms (Baseline Model - Logistic Regression, Advanced Model - Decision Tree Classifier, XGBClassifier).
  Hyperparameter tuning to optimize model performance.

## Model Evaluation:

Evaluation of model performance on the test set using key metrics:

**Macro-F1 Score:** Measures the overall accuracy of the model across all classes (TP, BP, FP).

**Precision:** Measures the proportion of true positives among all predicted positives.

**Recall:** Measures the proportion of true positives1 that the model correctly identified.

## Results and Discussion

## Model Performance

The XGBoost model demonstrated the best overall performance on the test set, achieving the following results:

Macro-F1 Score: 0.9158

Precision: 0.9157

Recall: 0.916

## Interpretation of Results

The high F1-score, precision, and recall values indicate that the XGBoost model effectively distinguishes between true positive, benign positive, and false positive incidents. 
This suggests that the model can significantly assist SOC analysts in prioritizing their investigations and reducing the time spent on false alarms.


## Business Use Cases

The developed solution can significantly improve multiple areas of cybersecurity operations:

  1. Security Operations Centers (SOCs): Automates the triage process and enhances analysts' decision-making.
  2. Incident Response Automation: Provides SOCs with faster, data-driven insights and recommended actions.
  3. Threat Intelligence: Increases the precision of detecting true and false positives using historical data.
  4. Enterprise Security Management: Reduces false positives, improves threat detection, and ensures swift incident response.

## Conclusion

This project successfully developed a machine learning model that can accurately predict the triage grade of cybersecurity incidents. The model demonstrates the potential to significantly improve the efficiency and effectiveness of SOC operations by:

  1. Reducing the time spent on investigating false alarms.
  2. Enabling SOC analysts to prioritize critical incidents.
  3. Providing valuable insights into the nature and characteristics of different types of incidents.

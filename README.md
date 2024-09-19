# Income Classification Project

## Problem Statement

Demographers analyze income data to study demographic changes and their societal impact. Migration patterns often correlate with income level shifts. To understand which individuals are more likely to migrate based on income, this project aims to classify whether an adult's income exceeds $50K.

## Data

The dataset used is `adult.csv`, which includes 32,561 records and 15 attributes such as age, workclass, education, marital status, occupation, and income.

## Exploratory Data Analysis (EDA)

- **Missing Values**: Handled by dropping and filling in missing values.
- **Duplicate Values**: Removed duplicate entries.
- **Data Cleaning**: Filtered out records with missing or invalid values and non-relevant entries.
- **Correlation Analysis**: Explored correlations between numeric features.

## Data Preprocessing

- **Encoding**: Categorical variables were one-hot encoded.
- **Splitting**: Data was split into training and test sets (80% training, 20% test).

## Models

### Random Forest Classifier

- **Accuracy on Training Data**: 86.64%
- **Accuracy on Test Data**: 86.35%
- **Key Metrics**: Precision, Recall, F1-score

### XGBoost Classifier

- **Accuracy on Training Data**: 86.84%
- **Accuracy on Test Data**: 87.51%
- **Key Metrics**: Precision, Recall, F1-score

### Hyperparameter Tuning

- **Best Model**: XGBoost with GridSearchCV
- **Best F1 Score**: 71.47%

## Results

- **Feature Importance**: Plotted using XGBoost and Random Forest models.
- **Confusion Matrices**: Visualized for both models.
- **Additional Insights**:
  - Number of female employees with income > $50K: 1,127
  - Country with the highest number of employees earning > $50K: United States
  - Percentage of people with advanced education earning > $50K: 47.03%

## Conclusion

XGBoost performed slightly better than Random Forest in terms of accuracy and other metrics. The analysis provides valuable insights into income distribution and demographic factors.

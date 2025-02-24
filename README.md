# Visa Prediction and Analysis : End to End Data Science Or Machine Learning project

## Project Overview

Visa Prediction and Analysis is an end-to-end Data Science/Machine Learning project that predicts the approval status of visa applications. This project involves building an end-to-end pipeline, including data preprocessing, exploratory data analysis (EDA), feature engineering, and model selection to identify patterns in visa application decisions.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Scikit-learn
- SMOTE (Synthetic Minority Over-sampling Technique)
- Chi-Square Test
- Random Forest, SVM, Logistic Regression

## Dataset Overview

The dataset consists of 25,480 rows and 12 columns, including:

- **Case ID** (Unique identifier, dropped for modeling)
- **Continent** (Origin of employees)
- **Education Level**
- **Job Experience** (Yes/No)
- **Job Training Requirement** (Yes/No)
- **Number of Employees**
- **Year of Establishment**
- **Region of Employment**
- **Prevailing Wage Unit**
- **Full-time Position** (Yes/No)
- **Case Status** (Target variable: Certified or Not Certified)

## Data Preprocessing

1. Checked for null values (None found).
2. Separated categorical and numerical columns.
3. Dropped **Case ID** (not useful for prediction).
4. Analyzed value distributions.
5. Identified outliers in numerical features.

## Exploratory Data Analysis (EDA)

- **Univariate Analysis**: Found skewness in numerical data, indicating outliers.
- **Categorical Analysis**: Identified imbalanced data distributions.
- **Multivariate Analysis**:
  - Checked correlation of numerical columns (found independence).
  - Used Chi-Square test on categorical columns (found job training requirement independent).
- **Case Status Visualization**:
  - 66.79% of applications were **Certified**.
  - 33.21% of applications were **Not Certified**.
- **Outlier Handling**: Used **Quantile method, Capping, and Trimming**.

## Feature Engineering

- Handled categorical data using **Label Encoding and One-Hot Encoding**.
- Addressed class imbalance using **SMOTE**.

## Model Selection and Training

1. **Train-Test Split**: Split dataset into training and testing.
2. **Standardization**: Used **StandardScaler** to normalize features.
3. **Model Comparisons**:
   - Logistic Regression
   - Support Vector Machine (SVM)
   - Random Forest
4. **Evaluation Metrics**:
   - Accuracy Score
   - Cross-Validation Score
5. **Best Model**:
   - **Random Forest** outperformed other models with the highest accuracy.

## Conclusion

This project provides insights into visa approvals by analyzing various factors. Random Forest proved to be the best-performing model for classification.

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/Ayankhan404/visa-prediction.git
   ```
2. Run the notebook:
   ```bash
   jupyter notebook
   ```
3. Follow the steps in the notebook to preprocess, analyze, and train the model.

## Future Improvements

- Use additional models like XGBoost and Neural Networks.
- Improve feature selection and hyperparameter tuning.
- Deploy the model using Flask or FastAPI.

## Author

[Ayan Khan](https://github.com/Ayankhan404)

## Connect with Me

[LinkedIn](https://www.linkedin.com/in/ayan-khan-917611250/)

# Bank Marketing Campaign Analysis and Prediction

This project aims to analyze and predict the outcomes of a bank marketing campaign using machine learning techniques. The data is obtained from a direct marketing campaign of a Portuguese banking institution. The goal is to predict whether a client will subscribe to a term deposit based on various attributes.

## Project Overview

### Problem Definition
The objective is to develop a predictive model to determine whether a client will subscribe to a term deposit based on demographic and campaign-related features.

### Data
The dataset used in this project is the `bank-full.csv` file, which contains 21 columns, including both categorical and numerical features.

## Workflow Stages

### Question or Problem Definition
Define the problem and objectives of the analysis.

### Acquire Training and Testing Data
Load the dataset for analysis and modeling.

### Wrangle, Prepare, and Cleanse the Data
Handle missing values, encode categorical variables, and scale numerical features.

### Analyze, Identify Patterns, and Explore the Data
Perform exploratory data analysis (EDA) to understand data distributions and relationships.

### Model, Predict, and Solve the Problem
Build and evaluate machine learning models to predict term deposit subscriptions.

### Visualize, Report, and Present the Problem-Solving Steps and Final Solution
Use visualizations to communicate findings and model performance.

### Supply or Submit the Results
Document and report the results of the analysis and modeling.

## Exploratory Data Analysis (EDA)

### Column Descriptions
- `age`: Age of the client.
- `job`: Type of job (categorical).
- `marital`: Marital status (categorical).
- `education`: Education level (categorical).
- `default`: Credit default status (binary).
- `housing`: Housing loan status (binary).
- `loan`: Personal loan status (binary).
- `contact`: Contact communication type (categorical).
- `month`: Last contact month of the year (categorical).
- `day_of_week`: Last contact day of the week (categorical).
- `duration`: Last contact duration, in seconds (numeric).
- `campaign`: Number of contacts performed during this campaign (numeric).
- `pdays`: Number of days since the client was last contacted (numeric).
- `previous`: Number of contacts performed before this campaign (numeric).
- `poutcome`: Outcome of the previous marketing campaign (categorical).
- `emp.var.rate`: Employment variation rate (numeric).
- `cons.price.idx`: Consumer price index (numeric).
- `cons.conf.idx`: Consumer confidence index (numeric).
- `euribor3m`: Euribor 3-month rate (numeric).
- `nr.employed`: Number of employees (numeric).
- `y`: Subscription to term deposit (binary target variable).

## Data Visualization
- **Age Distribution**: Shows the distribution of client ages.
- **Job Distribution**: Reveals the diversity and frequency of client occupations.
- **Marital Status Distribution**: Displays the distribution of clients' marital status.
- **Age and Campaign Outcome Relationship**: Boxplot illustrating age distribution by campaign outcome.

## Data Preparation
- **Missing Values**: Checked for and handled missing values in the dataset.
- **Feature Selection**: Dropped irrelevant features for modeling.
- **Encoding Categorical Variables**: Converted categorical variables to numerical using one-hot encoding.
- **Scaling**: Scaled numerical features for model compatibility.

## Model Selection and Evaluation

### DecisionTreeClassifier
- **Training and Testing**: Split the data into training and testing sets.
- **Model Performance**: Evaluated using precision, recall, and F1-score.
- **Confusion Matrix**: Analyzed true positives, false positives, true negatives, and false negatives.

### SGDClassifier
- **Training and Testing**: Similar approach as the DecisionTreeClassifier.
- **Model Performance**: Evaluated using precision, recall, and F1-score.
- **Confusion Matrix**: Provided insights into model performance on the test set.

### Cross-Validation
- **5-Fold Cross-Validation**: Performed to assess model stability and average performance.

### Hyperparameter Tuning
- **GridSearchCV**: Used to find the best hyperparameters for the DecisionTreeClassifier.

## Conclusion and Recommendations
- **Model Performance**: The SGDClassifier outperformed the DecisionTreeClassifier in terms of mean accuracy during cross-validation.
- **Class Imbalance**: Noted the class imbalance issue and suggested strategies to handle it.
- **Feature Engineering**: Recommended further feature engineering to improve model performance.
- **Feature Scaling**: Ensured all features are on the same scale to enhance model performance.

This project provides a comprehensive approach to analyzing and predicting the outcomes of a bank marketing campaign using machine learning techniques.

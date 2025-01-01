
# Universal Bank Loan Prediction

This project uses Support Vector Machines (SVM) to predict customer likelihood to accept a personal loan offer.

## Data

The data used in this project is `UniversalBank.csv`. It contains information about customers including demographics, financial information, and whether they accepted a previous loan offer.

## Methodology

1. **Data preprocessing:**
    - Irrelevant columns (`ID` and `ZIP Code`) are removed.
    - Categorical features are converted to the category data type.

2. **Data splitting:** The data is split into training and testing sets (70% train, 30% test).

3. **Model training:**
    - Two SVM models are trained:
        - Linear kernel SVM
        - RBF kernel SVM
    - Hyperparameter tuning using GridSearchCV is performed on the RBF model.

4. **Evaluation:**
    - Models are evaluated based on confusion matrices, classification reports, and ROC curves.

## Results

The project evaluates the performance of linear and RBF kernel SVMs and presents the performance metrics. Hyperparameter tuning is used to identify the best settings for the RBF kernel.

## Dependencies

- pandas
- scikit-learn
- matplotlib

## Usage

1.  Place the `UniversalBank.csv` in the same directory as this notebook.

2. Run the code.

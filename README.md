# Heart-Disease-Risk-Prediction-Model

## Overview
This project focuses on predicting the risk level of heart disease using a dataset containing various health metrics. The goal is to classify patients into three risk categories: Low, Moderate, and High. The project involves data analysis, preprocessing, and training a Logistic Regression model to achieve accurate predictions.

## Dataset
The dataset used in this project is `Heart_Attack_Risk_Levels_Dataset.csv`, which contains the following features:
- **Age**: Age of the patient.
- **Gender**: Gender of the patient (0 or 1).
- **Heart rate**: Heart rate measurement.
- **Systolic blood pressure**: Systolic blood pressure measurement.
- **Diastolic blood pressure**: Diastolic blood pressure measurement.
- **Blood sugar**: Blood sugar level.
- **CK-MB**: Creatine kinase-MB enzyme level.
- **Troponin**: Troponin protein level.
- **Result**: Binary result (positive/negative for heart disease).
- **Risk_Level**: Risk level classification (Low, Moderate, High).
- **Recommendation**: Recommended action based on risk level.

## Key Steps
1. **Data Loading and Exploration**:
   - Loaded the dataset and performed initial analysis to understand its structure and statistics.
   - Checked for missing values and examined the distribution of risk levels.

2. **Data Preprocessing**:
   - Mapped categorical risk levels (`Low`, `Moderate`, `High`) to numerical values (0, 1, 2).
   - Dropped the `Recommendation` column as it was not needed for model training.
   - Used `LabelEncoder` to encode categorical features and `StandardScaler` to standardize numerical features.

3. **Model Training**:
   - Split the dataset into training (80%) and testing (20%) sets.
   - Trained a Logistic Regression model with the following parameters:
     - Solver: `lbfgs`
     - Maximum iterations: 1000
     - Penalty: `l2`
     - Regularization strength (C): 1.0

4. **Evaluation**:
   - Achieved a training accuracy of **96.5%** and a test accuracy of **97.7%**, indicating strong performance.

## Results
The Logistic Regression model demonstrated high accuracy in predicting heart disease risk levels. The confusion matrix and classification report (not shown in the notebook) would provide further insights into the model's performance across different risk categories.

## How to Use
1. **Prerequisites**:
   - Python 3.x
   - Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

2. **Steps**:
   - Clone the repository or download the notebook.
   - Ensure the dataset `Heart_Attack_Risk_Levels_Dataset.csv` is placed in the correct directory.
   - Run the notebook cells sequentially to reproduce the results.

## Future Improvements
- Experiment with other classification algorithms (e.g., Random Forest, SVM) to compare performance.
- Perform hyperparameter tuning to optimize the model further.
- Include additional features or datasets to enhance prediction accuracy.

## Author
ScaRDrago9  
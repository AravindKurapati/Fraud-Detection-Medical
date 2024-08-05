# Fraud-Detection-Medical

This project aims to detect medical fraud using machine learning techniques. The notebook includes data preprocessing, exploratory data analysis, model training, and evaluation.

## Files
- `medical-fraud-detection.ipynb`: Jupyter notebook containing the entire analysis and model development.

## Requirements
- Python 3.6+
- Libraries: pandas, numpy, sklearn, matplotlib, seaborn

## Data Preprocessing
1. **Loading Data**: Load the training and testing datasets.
2. **Handling Missing Values**: Identify and impute missing values.
3. **Encoding Categorical Variables**: Convert categorical features into numerical values.
4. **Merging Columns**: Combine related columns to create new features.
5. **Grouping Data**: Aggregate data based on key features (e.g., provider ID).
6. **Feature Scaling**: Normalize features using standard scaling.
7. **Dimensionality Reduction**: Apply PCA to reduce the number of features.
8. **Splitting Data**: Split the data into training and testing sets.

## Modeling
1. **Training Models**: Train various machine learning models.
2. **Evaluation**: Evaluate models using accuracy, F1-score, precision, recall, and AUC.
3. **Feature Importance**: Determine the most important features in predicting fraud.

## Predictions
1. **Predict on Test Data**: Use the trained model to predict fraud on test data.
2. **Threshold Tuning**: Adjust decision thresholds for optimal performance.
3. **Visualizations**: Plot ROC curves, precision-recall curves, and other visualizations.

## Results
- The notebook provides a detailed analysis of model performance and feature importance.
- Final predictions on the test set are provided, along with evaluation metrics.

## How to Run
1. Clone the repository.
2. Install the required libraries.
3. Open the Jupyter notebook and run all cells.

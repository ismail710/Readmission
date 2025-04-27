# Data Readmission Analysis

This project analyzes a dataset containing information about patient hospitalizations, including demographics, medical history, and readmission status. The goal is to predict whether a patient will be readmitted based on the available features.

## Project Structure

- **`traitement.ipynb`**: Jupyter Notebook containing the data analysis, feature selection, model training, and evaluation.
- **`train.csv`**: Dataset used for analysis and modeling.
- **Generated Visualizations**:
  - Distribution of readmissions (pie chart).
  - Distribution of time spent in the hospital (histogram).
  - Number of procedures by readmission status (boxplot).
  - Correlation matrix (heatmap).
  - Confusion matrix (heatmap).

## Tools and Libraries Used

- **Data Manipulation and Analysis**:
  - `pandas`: For loading, cleaning, and analyzing the dataset.
- **Data Visualization**:
  - `matplotlib`: For creating plots and visualizations.
  - `seaborn`: For advanced visualizations like heatmaps and boxplots.
- **Machine Learning**:
  - `scikit-learn`: For model training, hyperparameter tuning, and evaluation.
  - `GridSearchCV`: For hyperparameter optimization.
- **Metrics**:
  - Accuracy, precision, recall, F1-score, and confusion matrix.

## Steps Performed

1. **Data Exploration**:
   - Loaded the dataset and displayed general information.
   - Checked for missing values and calculated descriptive statistics.
   - Visualized the distribution of key features and the target variable.

2. **Feature Selection**:
   - Removed features with low impact or high missing rates.
   - Dropped sparse features where less than 1% of samples had a "True" value.

3. **Correlation Analysis**:
   - Generated a correlation matrix to understand relationships between numerical features.

4. **Model Training and Evaluation**:
   - Trained Random Forest and Decision Tree models.
   - Tuned hyperparameters (`max_depth`, `min_samples_split`, `min_samples_leaf`) using `GridSearchCV`.
   - Evaluated the best model using accuracy, confusion matrix, and classification report.

## Results

- **Best Model**: Random Forest with optimized parameters.
- **Test Accuracy**: 62%.
- **Classification Report**:

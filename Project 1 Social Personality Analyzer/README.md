# Social Personality Analyzer

This project predicts personality types (Extrovert or Introvert) using social and behavioral data. It compares several machine learning models to find the most accurate approach.

## Project Overview

The goal is to classify individuals as Extrovert or Introvert based on features such as stage fear, time spent alone, social event attendance, and more. The project uses Python and popular data science libraries.

## Models Used and Rationale

The following models were used to compare performance:

- **Logistic Regression**: A simple, interpretable baseline for binary classification.
- **Decision Tree**: Captures non-linear relationships and feature interactions.
- **Random Forest**: An ensemble of decision trees that improves accuracy and reduces overfitting.
- **Gradient Boosting**: Builds trees sequentially to correct previous errors, often yielding high accuracy.
- **K-Nearest Neighbors (KNN)**: Classifies based on similarity to nearby data points.
- **Support Vector Machine (SVM)**: Effective for high-dimensional spaces and clear margin separation.

These models were chosen to provide a mix of simplicity, interpretability, and predictive power, allowing for a robust comparison.

## Project Structure

- `Social Personality Analyzer.ipynb`: Main notebook with all code, analysis, and results.

## Requirements

- Python 3.x
- pandas
- matplotlib
- seaborn
- scikit-learn

Install dependencies with:
```sh
pip install pandas matplotlib seaborn scikit-learn
```

## Usage

1. Place your dataset at `/content/personality_dataset.csv` or update the path in the notebook.
2. Open `Social Personality Analyzer.ipynb` in Jupyter or VS Code.
3. Run all cells to:
   - Clean and preprocess the data
   - Visualize distributions and correlations
   - Train and evaluate all models
   - Compare model accuracies and view the confusion matrix for the best model

## Output

- Accuracy and classification report for each model
- Bar plot comparing model accuracies
- Confusion matrix for the best-performing model

## Notes

- Categorical features are label-encoded.
- Missing values are handled appropriately.
- The target variable is `Personality` (0 = Extrovert, 1 = Introvert).

---

Feel free to modify the notebook and dataset path as needed.
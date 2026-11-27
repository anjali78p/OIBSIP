# Iris Flower Classification

**Oasis Infobyte SIP — Data Science, Task 1**

Classifies iris flowers into *Setosa*, *Versicolor* or *Virginica* from sepal and petal measurements.

## What's inside
- `Iris_Classification.ipynb` — full notebook (EDA, visualisations, feature discussion, 4 models, evaluation)

## Approach
1. Load the Iris dataset from `sklearn.datasets` (150 samples, 4 features, 3 balanced classes)
2. EDA: shape, dtypes, null check, descriptive statistics
3. Visualisations: pairplot, box plots, correlation heatmap
4. Feature discussion: petal length and petal width are the most discriminative
5. 80/20 stratified train/test split
6. Models: Logistic Regression, K-Nearest Neighbours, Decision Tree, Random Forest
7. Evaluation: accuracy, confusion matrix, classification report, 5-fold cross-validation

## Results
| Model | Test Accuracy | 5-Fold CV |
|---|---|---|
| Logistic Regression | 0.9667 | 0.9733 |
| K-Nearest Neighbours | 1.0000 | 0.9733 |
| Random Forest | 0.9000 | 0.9667 |
| Decision Tree | 0.9333 | 0.9533 |

**Best model:** K-Nearest Neighbours (tied with Logistic Regression on cross-validation).

## Run it
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
jupyter notebook Iris_Classification.ipynb
```

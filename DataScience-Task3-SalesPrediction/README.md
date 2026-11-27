# Sales Prediction Using Python

**Oasis Infobyte SIP — Data Science, Task 5**

Predicts product sales from advertising spend on TV, Radio and Newspaper.

## Files
- `Sales_Prediction.ipynb` — full notebook (EDA, plots, 3 models, evaluation, interpretation)
- `Advertising.csv` — dataset (200 markets; spend and sales in thousands)

## Approach
1. Load data, check nulls and duplicates, descriptive statistics, pairplot
2. Scatter plots of Sales vs TV / Radio / Newspaper, correlation heatmap
3. 80/20 train/test split
4. Models: Linear Regression (baseline), Polynomial Regression (degree 2), Random Forest
5. Metrics: MAE, RMSE, R², plus 5-fold cross-validated R²
6. Residual plot for the best model, coefficient and feature-importance analysis

## Results
| Model | MAE | RMSE | R² | CV R² |
|---|---|---|---|---|
| Polynomial Regression (deg 2) | 0.53 | 0.64 | 0.987 | 0.984 |
| Random Forest | 0.63 | 0.76 | 0.982 | 0.976 |
| Linear Regression | 1.46 | 1.78 | 0.899 | 0.887 |

**Best model:** Polynomial Regression (degree 2).
**Highest-impact channel:** TV overall, Radio per dollar spent, Newspaper has almost no effect.

## Run it
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
jupyter notebook Sales_Prediction.ipynb
```
Keep `Advertising.csv` in the same folder as the notebook.

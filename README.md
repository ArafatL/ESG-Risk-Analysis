# ESG Risk Analysis - S&P 500

## Problem
Predict and classify ESG risk levels (Negligible / Low / Medium / High / Severe) for 503 S&P 500 companies across 11 sectors and 108 industries.

## Dataset
S&P 500 ESG Risk Ratings from Kaggle. Features include Environmental, Social, Governance risk scores, Controversy Level, Full-Time Employees, and ESG Risk Level classification.

## What I Built
- Data cleaning: missing value imputation, outlier removal (407 clean records retained)
- Exploratory analysis: sector-wise bar charts, pairwise scatter plots, US state choropleth map, industry word cloud, top-10 performer rankings
- Feature engineering: one-hot encoding, percentile grouping (179 features)
- Random Forest Classifier with GridSearchCV (750 fits across 5-fold cross-validation)
- Feature importance analysis identifying top predictors

## Results
| Metric | Value |
|--------|-------|
| Baseline accuracy | 56% |
| Best accuracy (after GridSearchCV) | 59% |
| Best parameters | criterion=gini, max_depth=8, n_estimators=400 |
| Top predictor | Environment Risk Score (54.5% importance) |

## Tech Stack
`Python` `pandas` `scikit-learn` `RandomForestClassifier` `GridSearchCV` `Matplotlib` `Seaborn` `Plotly` `WordCloud`

## Files
- `ESG.ipynb` — full analysis notebook
- `SP_500_ESG_Risk_Ratings.csv` — dataset

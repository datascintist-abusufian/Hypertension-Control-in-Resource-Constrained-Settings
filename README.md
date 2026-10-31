# Bridging the Gap in Hypertension Management in Resource-Constrained Settings

This project uses machine learning to predict blood-pressure control status from patient factors and to understand the predictions. The factors include demographics, socioeconomic status, comorbidities, treatment and lifestyle. The aim is to support targeted hypertension management where clinical resources are limited.

## Data

`Expanded_Hypertension_Dataset_2.xlsx` holds 100,000 records with 21 variables:

- **Demographic and socioeconomic:** age, sex, education, occupation, monthly income, residence
- **Clinical:** systolic and diastolic blood pressure, elevated creatinine, diabetes, cholesterol, left ventricular hypertrophy, ischaemic heart disease, cardiovascular disease, retinopathy, family history
- **Behavioural and treatment:** smoking, physical activity, treatment type
- **Target:** blood-pressure control status

> **Synthetic data notice.** This dataset is a computer-generated (synthetic) expansion of a smaller cohort. Its records do not describe real patients.

## Method

The notebook `Bridging_the_Gap_in_Hypertension_Management_.ipynb` runs these steps:

1. Preprocesses the data with a ColumnTransformer: scaling and one-hot encoding.
2. Compares logistic regression, k-nearest neighbours, random forest, gradient boosting, AdaBoost and XGBoost.
3. Runs subgroup analysis by treatment type.
4. Explains the models with SHAP and LIME, and fits statistical models with statsmodels.

## Running it

```bash
pip install pandas numpy scikit-learn xgboost shap lime statsmodels seaborn tabulate
```

## Licence

No licence has been declared yet.

## Author

Md Abu Sufian - ORCID [0009-0007-3503-6942](https://orcid.org/0009-0007-3503-6942)

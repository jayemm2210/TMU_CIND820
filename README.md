# Labour Market Integration of Immigrants in Canada Post-Pandemic (2021)

## Overview
This project examines whether employment outcomes in Canada can be predicted using observable demographic, education-related, and geographic characteristics, and whether differences between immigrant and non-immigrant groups persist across comparable subgroups.

The analysis combines predictive modelling with descriptive subgroup analysis using aggregated 2021 Census data from Statistics Canada.

## Research Questions
- To what extent can employment outcomes in Canada be predicted using observable demographic, education-related, and geographic characteristics?
- Do age, education, gender, and geography help explain differences in employment outcomes across immigrant and non-immigrant groups?
- Which modelling approach provides the strongest balance of effectiveness, efficiency, and stability for predicting employment status using the available features?
- What do the remaining employment gaps suggest about structural or institutional barriers not captured in the dataset?

## Data Source
The project uses Statistics Canada Table 98-10-0442-01, based on the 2021 Census of Population. The dataset is aggregated, meaning each row represents a grouped combination of characteristics rather than an individual person.

## Methods
Two models were used:
- Logistic Regression
- Random Forest

Model evaluation includes:
- Accuracy
- Precision
- Recall
- F1 Score
- Training time
- Prediction time
- Cross-validation stability

Descriptive subgroup analysis compares employment outcomes across:
- age
- education
- gender
- geography

## Main Findings
Both models showed weak predictive performance, with accuracy and F1 scores close to 0.50. This suggests that observable demographic, education-related, and geographic variables are not sufficient for strong prediction of employment status on their own.

The descriptive analysis shows that age, education, gender, and geography are associated with employment outcomes, but they do not fully explain the persistent differences between immigrant and non-immigrant groups. These remaining gaps suggest the importance of broader structural and institutional factors such as credential recognition, language proficiency, Canadian work experience, and regional labour market conditions.

## Files
- `final_results.ipynb` – main analysis notebook
- `Muththalagan_Jananee_FinalReport.docx` – final report
- `model_comparison_results.csv` – model performance summary
- `model_stability_results.csv` – cross-validation results
- `logistic_feature_importance.csv` – Logistic Regression feature results
- `random_forest_feature_importance.csv` – Random Forest feature results

## Reproducibility
To reproduce the analysis:
1. Place the raw dataset in the expected data directory.
2. Open `final_results.ipynb`.
3. Run the notebook cells in order.
4. Review the exported figures and CSV outputs.

## Limitations
This project uses aggregated cross-sectional Census data rather than individual-level data. As a result, the findings reflect group-level associations and should not be interpreted as causal relationships.

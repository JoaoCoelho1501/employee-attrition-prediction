# Employee Attrition Prediction — Machine Learning and Fairness Analysis

A binary classification project comparing machine-learning models for employee attrition, with a focus on validation, class imbalance, and performance differences across demographic groups.

**Academic context:** MSc in Business Intelligence & Analytics, ISCAP (2025/26)  
**Authors:** Beatriz Teixeira and João Coelho

## Project objective

The project explores whether patterns in an employee dataset can be used to estimate attrition risk. The intended analytical use is to understand workforce patterns and evaluate model behaviour, not to automate employment decisions.

## Methodology

1. **Exploratory data analysis:** inspect distributions, relationships with the target, correlations, and potential train/test data drift.
2. **Preprocessing:** apply feature engineering and scikit-learn pipelines, including methods to address class imbalance.
3. **Model comparison:** evaluate Logistic Regression as a baseline alongside Random Forest, Gradient Boosting, neural networks, and K-Nearest Neighbours.
4. **Validation:** use stratified cross-validation and classification metrics suitable for imbalanced outcomes.
5. **Fairness analysis:** compare predictions and error patterns across groups such as gender and age bands.

## Results

Gradient Boosting was selected as the final model in the reported experiment, achieving the highest ROC-AUC among the evaluated candidates and good recall for the minority class.

The analysis highlighted variables associated with attrition in this dataset, including compensation, tenure, overtime, and job role. These associations should not be interpreted as causal effects.

## Technology stack

- Python and pandas
- scikit-learn
- Matplotlib
- Jupyter Notebook / Google Colab

**Dataset:** [Kaggle Playground Series — Season 3, Episode 3](https://www.kaggle.com/competitions/playground-series-s3e3)

## Reproducing the analysis

1. Download the competition dataset from Kaggle.
2. Place the files in the location expected by the notebook or update the data-loading paths.
3. Install the Python dependencies used in the notebook.
4. Run the analysis from data exploration through model evaluation and fairness checks.

## Responsible use and limitations

- The results are specific to the competition dataset and its target definition.
- Demographic group comparisons can be affected by sample size, label quality, and threshold choice.
- Fairness metrics can conflict; no single metric establishes that a model is fair.
- Predictions should not be used to make or automate hiring, promotion, performance, or termination decisions.
- Human review, transparency, privacy protection, and ongoing bias monitoring are essential in any real HR analytics setting.

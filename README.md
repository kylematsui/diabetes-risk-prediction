# Diabetes Risk Prediction

This project explores how well health, socioeconomic, and lifestyle factors can predict diabetes status. Using data from the [Diabetes Health Indicators Dataset](https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset), based on the CDC's 2015 Behavioral Risk Factor Surveillance System (BRFSS), the analysis involves data preparation, exploratory data analysis (EDA), and predictive modeling using logistic regression, lasso regression, and random forest.

## 📊 Objective

Build and compare supervised machine learning models that classify whether a survey respondent has diabetes or prediabetes based on indicators such as BMI, blood pressure, general health, physical activity, age, and income.

## 🎓 Project Information

This project was completed through **DataSC** at the **University of Southern California**. Our team analyzed 253,680 survey responses with 21 input features, applying data visualization and machine learning techniques to a public health dataset.

## 🧰 Tools & Libraries

- Python
- Jupyter Notebook
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`

## 📁 Files

- `weekly_progress/`: Notebooks, code, and analysis documenting five weeks of project work
- - `diabetes_binary_health_indicators_BRFSS2015.csv`: Dataset containing health, lifestyle, socioeconomic, and demographic indicators (source: Kaggle)
- `diabetes_presentation.pdf`: Summary slide deck presenting the methodology, model results, and conclusions
- `diabetes_risk_analysis.ipynb`: Main analysis notebook containing data preparation, exploratory analysis, model comparisons, and interpretation of results.

## 🔍 Key Steps

- **Data Preparation**: Inspected data types, missing values, and the distribution of the target variable.
- **EDA**: Used distributions, bar charts, and a correlation heatmap to explore relationships between diabetes status and health indicators.
- **Logistic Regression**: Estimated the probability of diabetes or prediabetes from the survey features.
- **Lasso Regression**: Applied an L1 penalty to logistic regression to shrink coefficients and simplify the model.
- **Random Forest**: Combined decision trees to capture more complex relationships between predictors.
- **Evaluation**: Compared accuracy, precision, and recall to assess performance and understand prediction errors.

## 📌 Findings

- Respondents with diabetes or prediabetes tended to have higher BMI. Median BMI was approximately 31 in the positive group, compared with 27 in the negative group.
- The positive-class rate was approximately 27% among respondents with high blood pressure, compared with 7% among those without it.
- Poorer self-reported general health was associated with higher positive-class rates, while higher income and more physical activity were associated with lower rates.
- LASSO had the highest reported accuracy, precision, and recall, although all three models performed similarly overall.

| Model | Accuracy | Precision | Recall |
| --- | ---: | ---: | ---: |
| Logistic Regression | 74.8% | 31.7% | 69.8% |
| Lasso Regression | 76.2% | 33.4% | 71.6% |
| Random Forest | 74.4% | 31.5% | 71.0% |

The models identified approximately 7 in 10 positive cases, but only about 1 in 3 positive predictions was correct. This highlights the limitations of predicting diabetes status from survey responses alone. The observed relationships describe associations, and the models have not been validated for clinical use.

## 📎 Data Source

- [Diabetes Health Indicators Dataset on Kaggle](https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset)
- Original survey: CDC's 2015 Behavioral Risk Factor Surveillance System (BRFSS)
- Target: `Diabetes_binary`, where `0` = no diabetes and `1` = prediabetes or diabetes

## 👤 Author

Kyle, Bo, Bryan, Hanwen, Isabel, Jyaan, and Tram

## 📝 License
This project is licensed under the [MIT License](LICENSE).

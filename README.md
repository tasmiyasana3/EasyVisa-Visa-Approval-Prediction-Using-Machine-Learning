# EasyVisa Visa Approval Prediction using Machine Learning

Machine Learning project focused on predicting US visa approval outcomes using classification models and data-driven business insights.

This project analyses visa application data processed by the Office of Foreign Labor Certification (OFLC) and develops predictive models to identify whether a visa application is likely to be certified or denied. The project aims to support faster and more efficient visa screening processes using Machine Learning techniques.

---

## Project Overview

The increasing number of US visa applications makes manual evaluation difficult and time-consuming. This project uses Machine Learning models to analyse applicant and employer-related factors that influence visa approval decisions.

The project includes:
- Exploratory Data Analysis (EDA)
- Data preprocessing and feature engineering
- Multiple classification models
- Oversampling and undersampling techniques
- Hyperparameter tuning
- Model comparison and final model selection
- Business insights and recommendations

---

## Business Objective

The goal of this project is to:
- Predict whether a visa application will be Certified or Denied
- Identify the key factors influencing visa approval
- Help streamline the visa screening process
- Support data-driven decision-making for EasyVisa and OFLC

---

## Dataset Information

The dataset contains:
- **25,480 visa application records**
- **12 features**
- Binary target variable:
  - `Certified`
  - `Denied`

### Important Features
- Continent
- Education level
- Job experience
- Job training requirement
- Number of employees
- Year of company establishment
- Region of employment
- Prevailing wage
- Wage unit
- Full-time position
- Visa case status (target)

---

## Technologies & Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Imbalanced-learn (SMOTE)
- Jupyter Notebook

---

## Exploratory Data Analysis (EDA)

### Key Insights

- Around **66.8%** of visa applications were certified
- Applicants with higher education had significantly better approval rates
- Experienced applicants showed higher chances of visa approval
- Full-time and yearly-paid positions had better certification rates
- Asia contributed the highest number of applications
- Hourly-paid positions showed lower approval rates
- Doctorate and Master's degree holders had the highest visa approval rates

---

## Data Preprocessing

### Steps Performed
- Removed unnecessary identifier column (`case_id`)
- Treated negative values in `no_of_employees`
- Checked missing and duplicate values
- Converted object data types into categorical variables
- Label encoding
- One-hot encoding
- Outlier detection using boxplots and IQR method
- Train-validation-test split
- Feature scaling where required

---

## Machine Learning Models

The following classification models were built and evaluated:

### Base Models
- Decision Tree (DT)
- Random Forest (RF)
- AdaBoost
- Gradient Boosting (GB)
- XGBoost (XGB)

---

## Handling Class Imbalance

### Oversampling
SMOTE (Synthetic Minority Oversampling Technique) was applied to improve minority class representation.

### Undersampling
Random undersampling techniques were also tested to compare model performance.

---

## Hyperparameter Tuning

Hyperparameter tuning was performed using:
- GridSearchCV
- Cross-validation techniques

### Tuned Models
- Tuned Random Forest
- Tuned Gradient Boosting
- Tuned AdaBoost
- Tuned XGBoost

---

## Model Evaluation Metrics

Models were evaluated using:
- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC Score
- Confusion Matrix

---

## Final Model Selection

After comparing all tuned models, the **Tuned Random Forest Model** was selected as the final model based on:
- Strong validation performance
- Better generalisation ability
- Balanced precision and recall
- Reduced overfitting

---

## Key Business Insights

### Factors Increasing Visa Approval Chances
- Higher educational qualifications
- Prior job experience
- Full-time employment
- Yearly salary structure
- Stable employment profiles

### Factors Associated with Visa Denial
- Hourly wage structures
- Lower educational qualifications
- Lack of experience
- Certain regional and employment patterns

---

## Business Recommendations

- Prioritise applicants with specialised educational backgrounds
- Improve screening efficiency using predictive analytics
- Focus on stable employment indicators during evaluation
- Use ML-assisted shortlisting for faster processing
- Monitor high-risk application profiles more carefully

---

## Project Structure

- `ML-2_BUSINESSREPORT_TS_final compressed.pdf` — Detailed business report
- `ML_2_PROJECT_TS.ipynb` — Complete implementation notebook
- `EasyVisa.csv` — Dataset csv file
- `README.md` — Project documentation

---

## Author

Tasmiya Sana

---

## Conclusion

This project demonstrates how Machine Learning can support visa approval prediction by identifying patterns associated with successful and unsuccessful applications. By leveraging predictive analytics, organisations can improve decision-making efficiency, reduce processing time, and support scalable visa evaluation systems.

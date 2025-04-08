Preprocessing Workflow for the Students Depression Dataset
The Students Depression dataset underwent a structured preprocessing workflow to enhance data quality and improve interpretability.

1. Handling Missing Values
Affected Attributes:
Numerical Features: Financial Stress
Categorical Features: Family History of Mental Illness, Depression
Imputation Methods:
Mean Imputation for numerical features
Mode Imputation for categorical features
Effect on Dataset Size:
Before: 27,901 rows
After: 27,878 rows (after removing extreme outliers)
2. Outlier Detection and Removal
Method Used: Interquartile Range (IQR)
Attributes Affected: Age, Academic Pressure, Work Pressure, CGPA
Outcome:
Removed extreme values to improve consistency
Majority of students aged 18-35, with fewer in older age groups
3. Data Standardization & Encoding
Numerical Feature Normalization:
Applied MinMaxScaler to Age, Academic Pressure, Work Pressure, CGPA, Study Satisfaction, Job Satisfaction, Work/Study Hours
Ensured all features contribute equally to analysis
Skewness Analysis:
CGPA: Right-skewed (majority of students had high GPAs)
Work/Study Hours: Showed variation, reflecting different academic workloads
Categorical Encoding:
Converted categorical features (Gender, Family History of Mental Illness, Dietary Habits) into numerical values for machine learning compatibility
4. Feature Selection
Techniques Used:
L1 Regularization (Lasso Regression) → Identified key predictors
Variance Thresholding → Removed low-impact features
Key Predictors of Depression:
Strongest Indicators:
“Have you ever had suicidal thoughts?”
Financial Stress
Additional Factors:
Gender
Sleep Duration
Family History of Mental Illness
Dietary Habits (Moderate and Unhealthy categories)
5. Statistical Insights
Descriptive Statistics:

Mean Age: 25.82 years
Average CGPA: 7.65
Work/Study Hours: Varied significantly, showing diverse academic pressures
Depression Scores: Bimodal distribution (students either had very low or very high scores)
Key Visual Insights:

Sleep Duration vs. Depression Score:
Students sleeping less than 5 hours per night had higher depression scores
Age Distribution:
Peak in younger students (18-35 years old)
CGPA:
Skewed toward higher scores
Study & Job Satisfaction:
Mixed responses, showing both highly satisfied and dissatisfied students
Work/Study Hours:
Showed a wide range of academic stress levels
This preprocessing workflow has refined the dataset for further analysis, providing a solid foundation for machine learning models and insights into the impact of academic stress, financial strain, and sleep deprivation on student mental health.

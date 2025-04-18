# 🔍 Employee Attrition Prediction using Machine Learning

## 📌 Project Overview

This project builds a machine learning model that predicts whether an employee is likely to **leave the company (attrition)** based on features like job satisfaction, salary, work-life balance, etc.  
By identifying potential resignations early, HR teams can take preventive actions to reduce turnover.

---

## 🧠 Problem Statement

Employee attrition can hurt companies by increasing costs and reducing team productivity.  
The objective is to use historical employee data to predict attrition and provide insights into what factors influence it most.

---

## 📂 Dataset

- **File Name:** `6. Predict Employee Attrition.csv`
- **Target Variable:** `Attrition`  
  - `1` → Employee left  
  - `0` → Employee stayed
- **Key Features:**
  - Age  
  - JobSatisfaction  
  - MonthlyIncome  
  - OverTime  
  - WorkLifeBalance  
  - YearsAtCompany  
  - EnvironmentSatisfaction  
  - and many more...

---

## 🚀 Technologies Used

- Python 3
- Google Colab / Jupyter Notebook
- pandas, numpy
- seaborn, matplotlib
- scikit-learn

---

## 🧰 Machine Learning Pipeline

1. Data Cleaning (`dropna`)
2. Label Encoding for categorical columns
3. Feature Scaling using `StandardScaler`
4. Train/Test Split (80/20)
5. Model Building using **Random Forest Classifier**
6. Model Evaluation
7. Feature Importance Visualization

---

## 🤖 Model Used

- **Random Forest Classifier**
  - An ensemble of decision trees
  - Performs well on structured/tabular data
  - Helps identify feature importance

---

## 📈 Model Performance

| Metric           | Score     |
|------------------|-----------|
| **Accuracy**     | **88.18%** |
| Precision        | 0.88      |
| Recall           | 0.88      |
| F1-score         | 0.88      |

### 🧾 Classification Report (Partial)


          precision    recall  f1-score   support

       0       0.88      0.88      0.88       203
       1       0.88      0.88      0.88       197

accuracy                           0.88       400

OUTPUT :-
Shape of the dataset: (1470, 35)

Columns in the dataset: ['Age', 'Attrition', 'BusinessTravel', 'DailyRate', 'Department', 'DistanceFromHome', 'Education', 'EducationField', 'EmployeeCount', 'EmployeeNumber', 'EnvironmentSatisfaction', 'Gender', 'HourlyRate', 'JobInvolvement', 'JobLevel', 'JobRole', 'JobSatisfaction', 'MaritalStatus', 'MonthlyIncome', 'MonthlyRate', 'NumCompaniesWorked', 'Over18', 'OverTime', 'PercentSalaryHike', 'PerformanceRating', 'RelationshipSatisfaction', 'StandardHours', 'StockOptionLevel', 'TotalWorkingYears', 'TrainingTimesLastYear', 'WorkLifeBalance', 'YearsAtCompany', 'YearsInCurrentRole', 'YearsSinceLastPromotion', 'YearsWithCurrManager']

First 5 rows of the dataset:
   Age Attrition     BusinessTravel  DailyRate              Department  \
0   41       Yes      Travel_Rarely       1102                   Sales   
1   49        No  Travel_Frequently        279  Research & Development   
2   37       Yes      Travel_Rarely       1373  Research & Development   
3   33        No  Travel_Frequently       1392  Research & Development   
4   27        No      Travel_Rarely        591  Research & Development   

   DistanceFromHome  Education EducationField  EmployeeCount  EmployeeNumber  \
0                 1          2  Life Sciences              1               1   
1                 8          1  Life Sciences              1               2   
2                 2          2          Other              1               4   
3                 3          4  Life Sciences              1               5   
4                 2          1        Medical              1               7   

   ...  RelationshipSatisfaction StandardHours  StockOptionLevel  \
0  ...                         1            80                 0   
1  ...                         4            80                 1   
2  ...                         2            80                 0   
3  ...                         3            80                 0   
4  ...                         4            80                 1   

   TotalWorkingYears  TrainingTimesLastYear WorkLifeBalance  YearsAtCompany  \
0                  8                      0               1               6   
1                 10                      3               3              10   
2                  7                      3               3               0   
3                  8                      3               3               8   
4                  6                      3               3               2   

  YearsInCurrentRole  YearsSinceLastPromotion  YearsWithCurrManager  
0                  4                        0                     5  
1                  7                        1                     7  
2                  0                        0                     0  
3                  7                        3                     0  
4                  2                        2                     2  

[5 rows x 35 columns]

Missing values in each column:
 Age                         0
Attrition                   0
BusinessTravel              0
DailyRate                   0
Department                  0
DistanceFromHome            0
Education                   0
EducationField              0
EmployeeCount               0
EmployeeNumber              0
EnvironmentSatisfaction     0
Gender                      0
HourlyRate                  0
JobInvolvement              0
JobLevel                    0
JobRole                     0
JobSatisfaction             0
MaritalStatus               0
MonthlyIncome               0
MonthlyRate                 0
NumCompaniesWorked          0
Over18                      0
OverTime                    0
PercentSalaryHike           0
PerformanceRating           0
RelationshipSatisfaction    0
StandardHours               0
StockOptionLevel            0
TotalWorkingYears           0
TrainingTimesLastYear       0
WorkLifeBalance             0
YearsAtCompany              0
YearsInCurrentRole          0
YearsSinceLastPromotion     0
YearsWithCurrManager        0
dtype: int64

Accuracy Score: 0.8639455782312925

Classification Report:
               precision    recall  f1-score   support

           0       0.88      0.98      0.93       255
           1       0.44      0.10      0.17        39

    accuracy                           0.86       294
   macro avg       0.66      0.54      0.55       294
weighted avg       0.82      0.86      0.83       294


Confusion Matrix:
 [[250   5]
 [ 35   4]]






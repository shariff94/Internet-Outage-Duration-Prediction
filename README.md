# Internet Outage Duration Prediction

## 1. Libraries Used

- numpy
- pandas
- matplotlib
- seaborn
- functools
- sklearn
- xgboost
- imblearn
- torch
- pytorchtools

---

## 2. EDA

- Basic EDA was performed on the dataset
- Data Wrangling performed to aid model building
- Answered the questions using visualizations
- Found class imbalance in the train dataset

---

## 3. Machine Learning Methods

### 3.1 Preprocessing

- Merging of the datasets was performed
- Train and Validation split
- Pipeline for preprocessing categorical and numerical features

### 3.2 Model Building

|        Model        | Train Score | Validation Score | Test Score |
|:-------------------:|:-----------:|:----------------:|:----------:|
| Logistic Regression |     75%     |        67%       |     57%    |
|    KNN Classifier   |     79%     |        69%       |     58%    |
|    SVM Classifier   |     88%     |        70%       |     59%    |
|    Random Forest    |     97%     |        76%       |     65%    |
|       XGBoost       |     90%     |        77%       |     65%    |

---

## 4. Machine Learning Methods with SMOTE

### 4.1 Preprocessing

- Merging of the datasets was performed
- Dropped the area_code as a feature
- Upsampling the non-majority classes
- Train and Validation split
- Pipeline for preprocessing categorical and numerical features

### 4.2 Model Building

|         Model         | Train Score | Validation Score | Test Score |
|:---------------------:|:-----------:|:----------------:|:----------:|
|  Logistic Regression  |     69%     |        67%       |     57%    |
|     KNN Classifier    |     83%     |        78%       |     59%    |
|     SVM Classifier    |     66%     |        67%       |     60%    |
| Bagged SVM Classifier |     66%     |        67%       |     62%    |
|     Random Forest     |     86%     |        82%       |     65%    |
|        XGBoost        |     91%     |        87%       |     66%    |

---
 
## 5. Deep learning method with SMOTE

### 5.1 Preprocessing

- Merging of the datasets was performed
- Dropped the area_code as a feature
- Upsampling the non-majority classes
- Train and Validation split
- Pipeline for preprocessing categorical and numerical features

### 5.2 Model Building

- Attempt 1 -> 63% on test
- Attempt 2 -> 66% on test
- Attempt 3 -> 65% on test
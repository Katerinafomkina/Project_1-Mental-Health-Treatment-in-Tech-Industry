# Project_1-Mental-Health-Treatment-in-Tech-Industry. Classification Problem
Analyze and Predict whether the individual needs treatment based on certain factors...

This data is from Open Source Mental Illness (OSMI) using survey data from years 2016, 2017, 2018 and 2019, 2020. Each survey measures and attitudes towards mental health and frequency of mental health disorders in the tech workplace.

The main goal of the work is to study mental health disorders and predict the treatment of employees in the tech industry.

Steps.
What I did in my project to study mental health treatment:
1. I classified and then combined the data from surveys from 2017 to 2020 years. 
2. Cleaned data, deleted misspelling mistakes, deleted not correct information.
3. Filled the columns with missing values. I used mode for categorical features and median for numerical features.
4. Mapped columns with multiple categories.
5. I used label encoding for categorical features, because most of them are ordinal.
6. Scaled Age-column using  MinMaxScaler().
7. Created new column age-range to make an exploratory analysis.
8. I provided Exploratory Data Analysis and made key insights.
9. Dropped country column, because its high cardinality.
10. Target feature was imbalanced. I used SMOTE()+Tomek Links to balance it.
11. Models, that I trained: Logistic regression, Decision tree, Random Forest, CatBoost, AdaBoost with base model Decision Tree, Adaboost with based model Extra Tree, XGBoost. I tuned every model with hyperparameters using GridSearchCV and Cross-Validation.
12. I created Dashboard to clearly see insights and make inferences.

The final prediction consists of 0 and 1. 0 means the person is not needed any mental health treatment and 1 means the person is needed mental health treatment.


Using Employee records, I built various machine learning models, along with that I draw some insights from the data via data analysis and visualization.



╒═════════════════════════════╤═════════════╤══════════╤════════════╤═══════════╕
│ Name                        │   Precision │   Recall │   F1-Score │   Roc-Auc │
╞═════════════════════════════╪═════════════╪══════════╪════════════╪═══════════╡
│ Decision Tree               │        0.86 │     0.78 │       0.82 │      0.79 │
├─────────────────────────────┼─────────────┼──────────┼────────────┼───────────┤
│ Logistic Regression         │        0.85 │     0.85 │       0.85 │      0.81 │
├─────────────────────────────┼─────────────┼──────────┼────────────┼───────────┤
│ Random Forest               │        0.88 │     0.83 │       0.86 │      0.83 │
├─────────────────────────────┼─────────────┼──────────┼────────────┼───────────┤
│ CatBoost Classifier         │        0.87 │     0.85 │       0.86 │      0.83 │
├─────────────────────────────┼─────────────┼──────────┼────────────┼───────────┤
│ AdaBoost base Decision Tree │        0.83 │     0.85 │       0.84 │      0.8  │
├─────────────────────────────┼─────────────┼──────────┼────────────┼───────────┤
│ AdaBoost base Extra Tree    │        0.84 │     0.85 │       0.84 │      0.8  │
├─────────────────────────────┼─────────────┼──────────┼────────────┼───────────┤
│ XGB                         │        0.84 │     0.83 │       0.84 │      0.8  │
______________________________________________________________________________________

Dataset is highly imbalanced, so Accuracy metric is irrelevant here. The main metric for the project is Recall, because it is very important to find the problem with mental health as soon as possible, so we need to decrease the number of false negatives predictions. 

From all the models, CatBoost Classifier, Adaboost Classifier and Logistic Regression achieved achieved a Recall of 85%. The CatBoost classifier has higher Precision compared to the models.
 
 Conclusion:
 It is very important to have a good mental health. An employer or managers should talk to employees about their mental health and benefits to prevent problems and help employees find information and receive timely mental health treatment. 
 

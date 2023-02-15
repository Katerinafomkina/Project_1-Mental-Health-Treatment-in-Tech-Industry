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

Outputs of Models:

1. Logistic Regression Model
train_score--> 0.86
test_score--> 0.8245
mean_accuracy--> 0.8548
roc_auc_score--> 0.8171

    Confusion Matrix          
    -----------------
   |        |       |
   | 0.78   |  0.22 |
    -----------------
   |        |       |
   | 0.15   |  0.85 |
    -----------------
    
2. Decision Tree Classifier
train_score--> 0.8541
test_score--> 0.8323
mean_accuracy--> 0.84
roc_auc_score--> 0.8343

    Confusion Matrix          
    -----------------
   |        |       |
   | 0.84   |  0.16 |
    -----------------
   |        |       |
   | 0.17   |  0.83 |
    -----------------
    
3. Random Forest Classifier
train_score--> 0.8622
test_score--> 0.8363
mean_accuracy--> 0.8615
roc_auc_score--> 0.8422

    Confusion Matrix          
    -----------------
   |        |       |
   | 0.87   |  0.13 |
    -----------------
   |        |       |
   | 0.19   |  0.81 |
    -----------------
    
 4. CatBoost Classifier
train_score--> 0.9681
test_score--> 0.8343
mean_accuracy--> 0.8711
roc_auc_score--> 0.8334

    Confusion Matrix          
    -----------------
   |        |       |
   | 0.83   |  0.17 |
    -----------------
   |        |       |
   | 0.16   |  0.84 |
    -----------------
    
5. AdaBoost Classifier with base model Extra Tree
train_score--> 0.9948
test_score--> 0.8008
mean_accuracy--> 0.88
roc_auc_score--> 0.7901

    Confusion Matrix          
    -----------------
   |        |       |
   | 0.74   |  0.26 |
    -----------------
   |        |       |
   | 0.16   |  0.84 |
    -----------------
    
6. XGBoost Classifier
train_score--> 0.9985
test_score--> 0.8225
mean_accuracy--> 0.8711
roc_auc_score--> 0.8195

    Confusion Matrix          
    -----------------
   |        |       |
   | 0.80   |  0.20 |
    -----------------
   |        |       |
   | 0.17   |  0.83 |
    -----------------
    
 As we can see Random Forest does a good job as well as almost all trained models.
 
 Conclusion:
 It is very important to have a good mental health. An employer or managers should talk to employees about their mental health and benefits to prevent problems and help employees find information and receive timely mental health treatment. 

**Practical Application III: Comparing Classifiers**    

Overview: In this practical application, goal is to compare the performance of the classifierd, namely K Nearest Neighbor, Logistic Regression, Decision Trees, and Support Vector Machines.

We will utilize a dataset related to marketing bank products over the telephone. 

This activity focuses on the CRISP-DM methodolgy

**Business Objective :**

The increasingly vast number of marketing campaigns over time has reduced its effect on the general public. Furthermore, economical pressures and competition has led marketing managers to invest on directed campaigns with a strict and rigorous selection of contacts. Such direct campaigns can be enhanced through the use of Business Intelligence (BI) and Data Mining (DM) techniques. This paper describes an implementation of a DM project based on the CRISP-DM methodology. Real-world data were collected from a Portuguese marketing campaign related with bank deposit subscription.

The business goal is to find a model that can explain success of a contact, i.e. if the client subscribes the deposit.

Such model can increase campaign efficiency by identifying the main characteristics that affect success, helping in a better management of the available resources (e.g. human effort, phone calls, time) and selection of a high quality and affordable set of potential buying customers

**Steps in CRISP-DM methodology**

(1) Data Understanding 
(2) Data Processing    
(3) Trail Model Run using Linear Regressions
(4) Setting up the target accuracy, recall and precision definintions 
(5) Using KNN, Decision Trees and SVM methods to compare the accuracy  
(6) Trying out the feature engineering and checking the results  
(7) Using the various hyperparameters and evaluating the results    
(8) Selecting the appropriate methods and proposing classifier to the customer         

**Initial Results**

| Classifier         |   Train Time(s) |   Train Accuracy |   Test Time(s) |   Test Accuracy |   Recall |   Precision |  
|--------------------|-----------------|------------------|----------------|-----------------|----------|-------------|
| LogisticRegression |       0.320297  |            90.21 |     0.0075016  |           89.55 |    41.44 |       65.67 |   
| KNN                |       0.0407088 |            92.1  |     1.47039    |           88.77 |    42.07 |       59.75 |     
| DecTree            |       0.325899  |           100    |     0.00997543 |           87.55 |    53.53 |       52.15 | 
| SVM                |      17.1152    |            91.62 |     6.02164    |           89.59 |    40.3  |       66.53 | 


**After feature engineering and Hyper parameter tuning**
  
| Classifier         |   Train Time(s) |   Train Accuracy |   Test Time(s) |   Test Accuracy |   Recall |   Precision |  
|--------------------|-----------------|------------------|----------------|-----------------|----------|-------------|
| Logistic_WithHyper |        100.585  |            92.27 |     0.0119815  |           91.11 |    42.57 |       67.12 | 
| KNN_WithHypTuning  |         25.4254 |            92.27 |     2.06553    |           90.51 |    41.39 |       62.32 |
| DecTree_WithHyper  |         16.7037 |            92.27 |     0.00868821 |           91.5  |    54.22 |       65.08 |
| SVM_WithHypTuning  |        506.523  |            92.27 |     9.46171    |           91.2  |    43.32 |       67.5  |

**Conclusion**
    
From the above results, its clear that with some feature engineering and hyper parameter tuning, the accuracy, precision and recall results have improved. For the current application, based on results, I will recommend Decision Tree algorithm with specific hyper parameters to the customerd

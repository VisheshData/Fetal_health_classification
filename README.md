# Fetal_health_classification
Cardiotocograms (CTGs) are a simple and cost accessible option to assess fetal health, allowing healthcare professionals to take action in order to prevent child and maternal mortality. The equipment itself works by sending ultrasound pulses and reading its response, thus shedding light on fetal heart rate (FHR), fetal movements, uterine contractions and more.

The dataset contains 2126 records of features extracted from Cardiotocogram exams, which were then classified by three expert obstetritians into 3 classes:

Normal
Suspect
Pathological

Citation
Ayres de Campos et al. (2000) SisPorto 2.0 A Program for Automated Analysis of Cardiotocograms. J Matern Fetal Med 5:311-318 link- https://lnkd.in/d_PChBEh

I proceeded on this project by looking at the data set and seeing missing values, duplicate rows. 
After cleaning up the data we started with basic Univariate Analysis and found that there were outliers. 
There are 22 features in the dataset. I didn't go for any outlier treatment or dimension reduction because I don't have any medical data basis for the treatment,
hence I started thinking of machine learning models which are less effected by outliers and no. of features in the dataset. Hence I started building decision tree model, 
random forest techniques like bagging, boosting, XGboost. During this process I found that the dataset was imbalanced. Normal occupied large proportion of data than susceptible 
and pathological. Hence we used oversampling techniques like SMOTE. After doing all this XGboosting gave great result which I had the target. I got 98% recall for normal, 
97% recall for Susceptible and 99% recall for Pathological. Overfitting was an issue but we used max depth parameter in order to control in order to get f1 score of test and 
training prediction quite close to each other.

Please give your upvotes on this code. Comment how we can improve this result.

# Credit_Risk_Analysis
### Overview
##### I was tasked with evaluating machine learning techniques to recommend whether they should be used to predict credit risk.
##### Using imbalanced-learn and scikit-learn libraries I built and evaluated six machine learning models. I then ran data generated by LendingClub, a peer-to-peer lending services company, through each model. These techniques were: random oversampling, SMOTE, under sampling, SMOTEENN (oversampling and under sampling), a balanced random forest classifier, and an easy ensemble classifier. Each of these techniques I evaluated with an accuracy score to determine which, if any, should be used to determine credit risk. In making my recommendation I will look at four results from the models. 

##### The first is the accuracy score of the model, which is the fraction of predictions our model got correct. The second is the precision score of the model, which is the number of true positives divided by the total number of positive predictions. The third is the recall score, which is the number of true positive divided by the total number of true positives and false negatives. The fourth criteria is the F1 score, which is a combination of precision and recall. 
   
#### Results
##### The results of my analysis follows:
* The accuracy score for random oversampling was 0.6605446354972261. The precision score is 0.01, a recall score of 0.68, and an F1 score of 0.02.

![Alttext]( https://github.com/GaryG484/Credit_Risk_Analysis/blob/main/images/naive_oversampling_results.JPG)

* The accuracy score for SMOTE oversampling was 0.6546563712732358. The precision score is 0.01, a recall score of 0.61, and an F1 score of 0.02.

![Alttext]( https://github.com/GaryG484/Credit_Risk_Analysis/blob/main/images/SMOTE_oversampling_results.JPG)

* The accuracy score for under sampling using clustercentroids was 0.5442661782548694. The precision score is 0.01, a recall score of 0.69, and an F1 score of 0.01.

![Alttext]( https://github.com/GaryG484/Credit_Risk_Analysis/blob/main/images/undersampling_results.JPG)

* The accuracy score for SMOTE was 0.6421290486158064. The precision score is 0.01, a recall score of 0.71, and an F1 score of 0.02.

![Alttext]( https://github.com/GaryG484/Credit_Risk_Analysis/blob/main/images/SMOTE_oversampling_results.JPG)

* The accuracy score for a balanced random forest classifier was 0.7885466545953005. The precision score is 0.03, a recall score of 0.70, and an F1 score of 0.06.`
 
![Alttext]( https://github.com/GaryG484/Credit_Risk_Analysis/blob/main/images/balanced_random_forest_results.JPG)

* The accuracy score for an easy ensemble classifier using AdaBoost was 0.9316600714093861. The precision score is 0.09, a recall score of 0.92, and an F1 score of 0.16.

![Alttext]( https://github.com/GaryG484/Credit_Risk_Analysis/blob/main/images/adboost_results.JPG)

#### Summary
##### The highest accuracy score as the easy ensemble classifier with AdaBoost, which was around 0.93, meaning that for every 100 predictions the model made 93 of them were correct. The next highest score was around 0.79 with the balanced random forest classifier. The next in order of highest accuracy score was random oversampling with 0.66, SMOTE oversampling with 0.65, SMOTE was 0.64, and under sampling was 0.54. Since only the easy ensemble classifier with AdaBoost and the balanced random forest classifier are above three-fifths correct, then only these two could be recommended as the rest would be only slightly more accurate than random guessing. 

##### The easy ensemble classifier with AdaBoost had a precision score of 0.09, meaning that of the 100 loan applications that were flagged to be bad only 9 were bad. The balanced random forest classifier had a precision score of 0.03, which is even worse than the AdaBoost. The recall score of the easy ensemble classifier with AdaBoost is 0.92, meaning it detected 92% of the bad loan applications. The recall score of the balanced random forest classifier is 0.70. The easy ensemble classifier with AdaBoost had an F1 score of 0.16, as it has a low precision score. The balanced random forest classifier has an F1 score of 0.06, as its precision score is even lower than the ensemble classifier with AdaBoost.

##### The easy ensemble classifier with AdaBoost is the clear choice for which of these models I would recommend, as it has the highest accuracy score and the highest recall score. The precision score is on 0.09 which is a little low for commercial use so I would recommend looking at other models if they are available, but of these six I would recommend the easy ensemble classifier with AdaBoost. 


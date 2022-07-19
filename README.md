# Credit_Risk_Analysis
#### *Utilized Python's imbalance-learn and scikit-learn libraries to predict credit risk using several machine learning models.*

## Overview of Analysis - Supervised Machine Learning

Objective of this project was to use machine learning models to analyze credit risk to provide a more reliable and quicker loan experience. Using these models, good candidates for loans were accurately identified which could efficiently assist financial institutions in decreasing their loan default rates. Several machine learning models were built and evaluated to predict credit risk.

## Resources
- Dataset:
  - LoanStats_2019Q1.csv
  
- Software Used:
  - Jupyter Notebook
  - Python
  - NumPy, scikit-learn, imbalanced-learn libraries
  - Ensemble and resampling techniques
  
## Results

- Naive Random Oversampling:

![Naive_Random_Oversampling](https://user-images.githubusercontent.com/98711219/179661527-9ff18595-1a32-4810-89fd-e22e3151d58b.png)


- SMOTE Oversampling
![SMOTE_Oversampling](https://user-images.githubusercontent.com/98711219/179661584-9bdaeadf-6154-4e82-8667-67135e890103.png)


- Cluster Centroid Undersampling
![ClusterCentroids_Undersampling](https://user-images.githubusercontent.com/98711219/179661937-01eb24fc-7d69-4dd4-b17d-01f0d351c11f.png)


- SMOTEEN Combination Sampling
![SMOTEEN_Comb_Sampling](https://user-images.githubusercontent.com/98711219/179661691-c6062e2f-f744-4664-a04d-2da19eba0587.png)


- Balanced Random Forest Classifier
![Bal_RandomForest_Classifier](https://user-images.githubusercontent.com/98711219/179661765-097a0ac0-3566-4151-aa5b-e1102a67b565.png)


- Easy Ensemble AdaBoost Classifier
![EasyEnsemble_AdaBoost](https://user-images.githubusercontent.com/98711219/179661831-8084c698-d117-40dd-8efd-5bf4a1418c26.png)



## Summary

Sensitivity is more valuable than precision for analyzing risk and default loans in the financial industry on loan candidates. In order to prevent loan defaults it would be important for financial institutions to be able to identify those high risk individuals. Precision isn't as important since a good candidate mistakenly flagged as high-risk could receive further review. 

All six algorithms had a fairly low precision rate for high risk individuals. Since the Easy Ensemble AdaBoost Classifier had the highest precision rate at 7%, this is still pretty low and can be determined that out of all the customers flagged as high-risk, 7% actually were. With regards to the low-risk, all the models had a perfect precision with all the low-risk customers flagged correctly.

Precision is not giving us much information to compare the algorithms. Therefore, sensitivity should be looked at. The Easy Ensemble Adaboost Classifier had the highest sensitivity (91% for high-risk and 94% for low-risk). This means that 91% of the time, high-risk individuals are flagged correctly. 

Finally looking at the balanced accuracy score to determine how correct the model was, the Easy Ensemble AdaBoost Classifier had the highest accuracy score and should be the model of choice. 

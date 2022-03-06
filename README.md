# Credit_Risk_Analysis  
## Overview of the analysis
This project is brought out to use Python Machine Learning Models to assess the features of different applicants and to predict credit risk. 
A total of 6 models was used in this project, and the are listed as below.  
- Random Over Sampler
- SMOTE
- Cluster Centroids
- SMOTEEN
- Balanced Random Forest Classfier
- Easy Ensemble AdaBoost Classifier.  

## Results
Below are the results generated from this project.
![ROS](https://user-images.githubusercontent.com/93500353/156940885-e567861a-06fa-48b3-af66-c9918037a1c3.png)
![Random Oversampling](https://user-images.githubusercontent.com/93500353/156940893-2fa27729-cca5-4d3d-a028-31196979b59d.png)
### RandomOverSampler Results:  
The balanced accuracy score is at 64.13%. From the reports above, the precision of high_risk is at 1%, which is darastically lower than the precision of low_risk, at 100%.

![SMOTE](https://user-images.githubusercontent.com/93500353/156941091-c9c7f88b-d615-4c43-a1bf-0584f5331d83.png)
![SMOTE 2](https://user-images.githubusercontent.com/93500353/156941094-385123c2-525b-402b-9d5a-8e871387beaf.png)
### SMOTE Results:  
The balanced accuracy rate is at 63.74%. The reports above show a previson of 1% for high risk and 100% for low risk. Recall and F1 scores are both identical with the results from Random Over Sampling methods.  

![Under Sampling](https://user-images.githubusercontent.com/93500353/156941527-a0e4c283-077d-4da6-9190-c4685c36b554.png)
![Under Sampling 2](https://user-images.githubusercontent.com/93500353/156941532-a5058bc9-8078-488b-8020-ddf21f526295.png)
### Under Sampling with Cluster Centroids Results:  
The balanced accuracy score is 51.11% which is significantly lower than the results from over sampling models. The Precision remain the same as previous that in previous two models, while the recall and f1 scores are lower. This could be the result of lower sample sizes.   
  
![SMOTEENN](https://user-images.githubusercontent.com/93500353/156941743-863f1d89-307a-4cf7-9b9f-09f5990f517d.png)
![SMOTEENN 2](https://user-images.githubusercontent.com/93500353/156941754-92c8c3e1-92f7-4add-9b09-333b0e496374.png)
### Combination SMOTEENN Results:  
The balanced accuracy score is at 62.44% which is slightly lower than that in oversampling results. Precisions are the same with previous models, with 1% in high risk and 100% in low risk. Recall and f1 scores are higher than under sampling models but lower than over sampling results.  

![RFC 1](https://user-images.githubusercontent.com/93500353/156941975-688d5a71-5d99-48d0-980b-f91dd08cd4cf.png)
![RFC 2](https://user-images.githubusercontent.com/93500353/156941979-65943031-3cee-45cc-9df9-246261d0da99.png)
### Balanced Random Forest Classifier Results:  
This algorithm provides a balanced accuracy score of 78.77% which is relatively higher than that from all previous results. The Precision for high risk is increased to 4%, which higher recall and f1 scores of 67% and 0.07.  

![EAB 1](https://user-images.githubusercontent.com/93500353/156942229-db0dd4e1-d593-46b5-8683-a6e42454c374.png)
![EAB 2](https://user-images.githubusercontent.com/93500353/156942254-864367a8-8dc6-48f7-bf63-c80155008222.png)
### Easy Ensemble AdaBoost Classifier Results:  
The balanced accuracy score is at 92.54% which is signigicantly higher than all previous approaches. The precision of high risk is at 0.07. The recall for high risk is at 91% and f1 score is at 0.14.   

## Conclusion
The easy ensemble Adaboost Classifier methods did bring out more accurate response compared to all previsour algorithms. However, with the precision at 0.07, the bank will not have an clear indication on who to reject for high credit risk, and incurrs extra cost in the future. I would suggest to look into data source to get more samples in high risk categories to help build better machine learning results. 

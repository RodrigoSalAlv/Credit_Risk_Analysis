# Credit_Risk_Analysis
## Analysis Overview
Using different Supervised Machine Learning modes we need to predict a credit risk. With the results of each model we will evaluate the performance and make a recomendation on whether they should be used to predict the credit risk.

## Results
### Random Oversampling 
![image](https://user-images.githubusercontent.com/96214489/166395477-41b37a46-5be9-4c19-90be-c76c88a93af5.png)

- The balanced accuracy score is 63.6%
- The high risk precission is about 1% and a recall of 62%
- The low risk precission is about 100% and a recall of 65%
- Due to the low precission in high risk the f1 for high risk is about 2% and the f1 for low risk is about 79%

### SMOTE Oversampling
![image](https://user-images.githubusercontent.com/96214489/166395762-0e862c6d-83af-4e82-a8c1-612ebb241e02.png)

- Pretty similar results as the previous model
- The balanced accuracy score is 63.0%
- The high risk precission is about 1% and a recall of 62%
- The low risk precission is about 100% and a recall of 64%
- Again, due to the low precssion in high risk the f1 for them is about 2% and the f1 for low risk is about 78%

### Undersampling
![image](https://user-images.githubusercontent.com/96214489/166396088-a60985a0-ddb1-4fd5-a549-be800818d8f9.png)

- The balanced accuracy score is 51%
- Again, the high risk precsision is about 1% and a recall of 59%
- The low risk precission is 100% and a recall of 43%
- The f1 result for high risk is about 1% and the f1 for low risk is about 60%

### Combination Sampling
![image](https://user-images.githubusercontent.com/96214489/166396541-feb9a8fc-8870-4851-a9d1-6a8006256f2d.png)

- The balanced accuracy score is 63.7%
- The high risk precission is 1% and a recall of 70%
- The low risk precission is about 100% and a recall of 57%
- The f1 result for high risk is about 2% and the f1 for low risk is about 73%

### Balanced Random Forest Classifier
![image](https://user-images.githubusercontent.com/96214489/166398402-f6c59775-a9b1-461f-bf75-f7dad749edb9.png)

- The balanced accuracy score is 78.8%
- The high risk precission is 3% and a recall of 70%
- The low risk precission is about 100% and a recall of 87%
- The f1 result for high risk is about 6% and the f1 for low risk is about 93%

### Easy Ensemble AdaBoost Classifier
![image](https://user-images.githubusercontent.com/96214489/166399504-cfb36e96-bd6e-4bb2-bc49-68c76356d46f.png)

- The balanced accuracy score is 93.1%
- The high risk precission is 9% and a recall of 92%
- The low risk precission is about 100% and a recall of 94%
- The f1 result for high risk is about 16% and the f1 for low risk is about 97%

## Summary

We can notice an improvement in performance of each model, however, each of them do not neet the minimun of "requirements" that a model to predict a high credit risk should. We could say that with the Ensemble AdaBoos Classifier get the less quantity of False Negatives, however the quantity of False Positives stills very high, about a 6% of the total cases evaluated will get a prediction as a "high risk" when they're not. However, if a 6% margin of error is acceptable, we could say that the last one could be a very good model.



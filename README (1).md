
# **Digit Recognizer**

My main goal is to identify digits and get high accuracy in this project. Here I want to elaborate how I have planned to go about it.

Our usual tendency is to seperate the dataset into train set and dev set (in case test set is already seperated), and train the whole dataset and evaluate on dev set, but in this project I used K-Fold cross-validation extensively.
Cross-validation help us to get clean predictions, clean means the predictions that model has never seen before.
Second thing is to scale our dataset and to expirement if scalling of data helps to get better result.

I want to evaluate my dataset with different classification metrics such as balanced-accuracy, micro-average, confusion matrix, ROC-AUC, Precision-Recall Curve other than accuracy, reason being, evaluating binary classification data with these metrics is quiet straight-forward, lets see how can we evalute our Multi-class classification dataset using these metrics.

Another thing that I'm curious about is 'Data Augmentation', we'll se if data augmentation helps in getting better result.
I want to do hyperparameter tunning but not from GridSearchCV but from Validation Curve.

Then I'll plot Learing curve to get to know whether the training and cross-validation scores converge together.
Finally, save best model and evaluate on test set.


## 🔗 Data set link
https://www.kaggle.com/competitions/digit-recognizer

## Installation

To install libraries used in this project-

```bash
  pip install scikit-learn
  pip install numpy
  pip install pandas
```
    
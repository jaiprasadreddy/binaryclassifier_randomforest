# Binary Classification of Tumor using gene expression data

## Synopsis
The dataset contains 62 samples collected from colon-cancer patients. Among them, 40 tumor biopsies are from tumors (labelled as "negative") and 22 normal (labelled as "positive") biopsies are from healthy parts of the colons of the same patients. Two thousand out of around 6500 genes were selected based on the confidence in the measured expression levels.
The task is to predict the presence of tumor based on the gene expression data.


## Data Preprocessing 
The dataset contains 2000 features for each input and the size of the dataset is 62,In this classfication task,The Multi level perceptron model is used to predict the class of tumor present or not. The positive samples are assigned to the output 1 and the negative samples are assigned to value 0.
The polt shows the  variance curve on the datset and it indicates that the variance converges after in the range of 38 to 42 and further transform the dataset to the axis of 40 features.
The 80% of the dataset is assigned to the training set and 20% is assigned to the test dataset.

## Prerequisities
The following softwares/Libraries are the prerequities for testing the model .
python 2.7
Matplotlib
sklearn
pandas
numpy
please run the set.sh file to install the following dependencies

## Cost sensitive Random Forest classifier
In medical diagnosis or skewed datasets where one class has maximum number of samples, the default assumption of equal misclassification costs underlying machine learning techniques is most likely violated. A dataset having more samples of single class will make the model to learn more features about one class and neglect about the other one. To address this problem, cost-sensitive classification is developed, which considers the varying costs of different misclassification types. Usually a cost matrix is defined or learned to reflect the penalty of classifying samples from one class as another. A cost-sensitive classification method takes a cost matrix into consideration during the model building process. 

## Results
The observation over the task is noticed that the model stops after certain specific number of estimators if there is not much change in the training loss and the training loss converges over the time. The model is tested over the test data and observed to give the over all accuracy of 85% bust as the dataset is skewed towards one class(having much of samples belonging to single class) The followng precision,recall and F1 score values are as follows 
               
                       precision    recall  f1-score   support
    class negative       0.85      0.92      0.88        12
    class positive       0.88      0.78      0.82         9

    avg / total       0.86      0.86      0.86        21

    Accuracy is: 85.7%

# binaryclassifier_randomforest

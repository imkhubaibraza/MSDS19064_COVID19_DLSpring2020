## Focal Loss for Handling Class Imbalance in Detecting Coronavirus Infections through Chest X-Ray images

This repository contains code and results for COVID-19 classification assignment by Deep Learning Spring 2020 course offered at Information Technology University, Lahore, Pakistan. This assignment is only for learning purposes and is not intended to be used for clinical purposes. 

## Dataset

[DataSet Link](https://drive.google.com/file/d/1eytbwaLQBv12psV8I-aMkIli9N3bf8nO/view?usp=sharing)

## Metric Used

1. Accuracy Score 
2. F1 score
3. Hamming Loss
4. Confusion Matrix


# Training

As this is multi label image classification, the loss function was  binary crossentropy logit and activation function used was sigmoid at the  output layer. so after training there is one probabilistic threshold method which  find out the best threshold value for each label seperately and based on the threshold value(0.5)



## Final Result

Accuracy| F1-score| Loss| Hamming loss
----------|-----------| -----------| -----------
94.0%| 95.1%| 0.016| 0.0429


| Covid19 |Predicted Infected        | Predicted Normal  |
| ------------- |:-------------:| -----:|
| Actual Infected      | 534 | 81 |
| Actual Normal      | 23      |   862 |


[[[598   2]
  [  9  19]]

Normal:
 [[209  19]
  [ 16 384]]

Pneumonia:
 [[384  16]
  [ 19 209]]]



## Focal Loss for Handling Class Imbalance in Detecting Coronavirus Infections through Chest X-Ray images

This repository contains code and results for COVID-19 classification assignment by Deep Learning Spring 2020 course offered at Information Technology University, Lahore, Pakistan. This assignment is only for learning purposes and is not intended to be used for clinical purposes. 

## Dataset

[DataSet Link](https://drive.google.com/file/d/1eytbwaLQBv12psV8I-aMkIli9N3bf8nO/view?usp=sharing)


## Models
[Saved Model Link](https://drive.google.com/drive/folders/14P2GRHZ7n-Nj-rhHTQu4SvTFKV_KlIF_?usp=sharing)
## Metric Used

1. Accuracy Score 
2. F1 score
3. Hamming Loss
4. Confusion Matrix


# Training

As this is multi label image classification, the loss function was  binary crossentropy logit and activation function used was sigmoid at the  output layer. so after training there is one probabilistic threshold method which  find out the best threshold value for each label seperately and based on the threshold value(0.5)


## Best Model
### Final Result on Validation Sets

Accuracy| F1-score| Loss| Hamming loss
----------|-----------| -----------| -----------
94.0%| 95.1%| 0.016| 0.0429


| Covid19 |Predicted Infected        | Predicted Normal  |
| ------------- |:-------------:| -----:|
| Actual Infected      | 598 | 2 |
| Actual Normal      | 9      |   19 |

| Normal |Predicted Infected        | Predicted Normal  |
| ------------- |:-------------:| -----:|
| Actual Infected      | 209 | 19 |
| Actual Normal      | 16      |   384 |

| Pneumonia |Predicted Infected        | Predicted Normal  |
| ------------- |:-------------:| -----:|
| Actual Infected      | 384 | 16 |
| Actual Normal      | 19      |   209 |


### Final Result on Training Sets

Accuracy| F1-score| Loss| Hamming loss
----------|-----------| -----------| -----------
92.3%| 93.1%| 0.014| 0.047


| Covid19 |Predicted Infected        | Predicted Normal  |
| ------------- |:-------------:| -----:|
| Actual Infected      | 5989 | 78 |
| Actual Normal      | 21      |   112 |

| Normal |Predicted Infected        | Predicted Normal  |
| ------------- |:-------------:| -----:|
| Actual Infected      | 1958 | 143 |
| Actual Normal      | 242      |   3857 |

| Pneumonia |Predicted Infected        | Predicted Normal  |
| ------------- |:-------------:| -----:|
| Actual Infected      | 3859 | 242 |
| Actual Normal      | 141      |   1958 |





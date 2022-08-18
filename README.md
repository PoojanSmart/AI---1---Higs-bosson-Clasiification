# AI-1-Higs-bosson-Clasiification
This project has been done under course AI - 1 (Univ.ai).
It was a [kaggle challange](https://www.kaggle.com/competitions/higgs-boson
).

## Problem statement

In LHC (large hadron collider), when protons are collided with each other, the collision is known as events.
These event data contains features like type, direction, energy. These features are used to create set of variables on which the events can be classified as significant or insignificant, here **signal** or **background**.
when an event is unique and its feature space is disconnected from the ones previously observed in past experiments, a new particle deems to be discovered.
Therefore, classification of these events holds lot of scope for future studies and experiments of the events classified as signal.

![image](https://github.com/PoojanSmart/AI-1-Higs-bosson-Clasiification/blob/main/images/lhc.jpg)

## Pipeline
1. Data Loading
2. Data Exploration
3. Data Preprocessing and Viz.
4. Base models
5. Ensemble models
6. Final results and Inference

## Models

### Base models
1. Logistic Regression
2. Decision Tree Classifier

### Ensemble models
1. Random Forest
2. Gradient Boosting

## Results

| Strategy | Recall | F1 Score | AUC score | AMS|
| --- | --- | --- | --- | --- |
| Logistic Regression - No imbalance correction | 0.5333 |  0.5946  |   0.6983  | 0.8745 |
|        Logistic Regression - Upsampling       | 0.7642 |  0.6676  |   0.7444  | 0.8875 |
|       Logistic Regression - Downsampling      | 0.7702 |  0.6685  |   0.745   | 0.8901 |
| Decision Tree - No imbalance correction | 0.7033 |  0.7316  |   0.7941  | 1.1572 |
|        Decision Tree - Upsampling       | 0.8003 |  0.7426  |   0.807   | 1.0342 |
|       Decision Tree - Downsampling      | 0.8076 |  0.7405  |   0.8058  | 1.0181 |
| `Random Forest - No imbalance correction` | 0.7097 |  0.7513  |   0.8078  | **1.2927** |
|        `Random Forest - Upsampling`       | 0.8051 |  **0.7659**  |   **0.8246**  |  1.14  |
|       `Random Forest - Downsampling`      | 0.8051 |  **0.7659**  |   **0.8246**  |  1.14  |
| Bagging - No imbalance correction | 0.7098 |  0.7449  |   0.8035  | 1.2319 |
|     Bagging Tree - Upsampling     | 0.8155 |  0.7534  |   0.8161  | 1.0661 |
|    `Bagging Tree - Downsampling`    | **0.8214** |  0.756   |   0.8185  | 1.0733 |
| Gradient Boosting - No imbalance correction |  0.71  |  0.7471  |   0.805   | 1.2347 |
|        Gradient Boosting - Upsampling       | 0.8078 |  0.7579  |   0.819   | 1.0886 |
|       Gradient Boosting - Downsampling      | 0.8209 |  0.7585  |   0.8204  | 1.0768 |

![image](https://github.com/PoojanSmart/AI-1-Higs-bosson-Clasiification/blob/main/images/roc%20curve.png)

## Participants
- Poojan Smart
- Abjasree S
- Niranjan Solanki
- Vaishnav Panuganti

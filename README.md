# Pumpkin-Seeds-Binary-Classification

## Overview

The main purpose of this project is to explore the binary classification between features and the pumpkin seed varieties.

In this project, the baseline model is logistic regression, further improvement and tuning will be applied in later section in order to compare the performance. An alternative model will be selected to compare with the baseline model.


## Dataset

The dataset used for this project is the Pumpkin Seeds Dataset. The dataset contains 13 columns consisting of 12 types of features and 1 target classes.

The dataset used in this project is the **Pumpkin Seeds Dataset** from Kaggle.

DATASET: https://www.muratkoklu.com/datasets/

Citation Request :
KOKLU, M., SARIGIL, S., & OZBEK, O. (2021). The use of machine learning methods in classification of pumpkin seeds (Cucurbita pepo L.). Genetic Resources and Crop Evolution, 68(7), 2713-2726. Doi: https://doi.org/10.1007/s10722-021-01226-0

https://link.springer.com/article/10.1007/s10722-021-01226-0
https://link.springer.com/content/pdf/10.1007/s10722-021-01226-0.pdf

Abstract: Pumpkin seeds are frequently consumed as confection worldwide because of their adequate amount of protein, fat, carbohydrate, and mineral contents. This study was carried out on the two most important and quality types of pumpkin seeds, ‘‘Urgup_Sivrisi’’ and ‘‘Cercevelik’’, generally grown in Urgup and Karacaoren regions in Turkey. However, morphological measurements of 2500 pumpkin seeds of both varieties were made possible by using the gray and binary forms of threshold techniques. Considering morphological features, all the data were modeled with five different machine learning methods: Logistic Regression (LR), Multilayer Perceptrons (MLP), Support Vector Machine (SVM) and Random Forest (RF), and k-Nearest Neighbor (k-NN), which further determined the most successful method for classifying pumpkin seed varieties. However, the performances of the models were determined with the help of the 10 kfold cross-validation method. The accuracy rates of the classifiers were obtained as LR 87.92 percent, MLP 88.52 percent, SVM 88.64 percent, RF 87.56 percent, and k-NN 87.64 percent.


## Key Findings

Based on the result printed in the notebook file, the accuracy of the baseline model is 0.86, which means there are 86% correct predictions in the test data. The precision of Cercevelik is 0.82, which means there are 82% correct prediction in the pumpkin seed predicted by the baseline model actually belong to the Class Cercevelik. The recall of Cercevelik is 0.93, that means the baseline model successfully recognized 93% of Cercevelik. F1 Score of the Cervevelik is 0.87, which balances precision and recall.

Since logistic regression use linear relationship and there are overlapping features distribution in the two classes of the pumpkin seeds, so it might not be able to capture the nonlinear relationship between features and the class.

There are two possible improvments, firsts is the cross-validation, it allows the model to utilize the dataset and make the evaluation performance to be more stable. The second is to compare with other models to evaluate if they can capture the relationship between the features and the class.

The alternative SVC model has the accuracy 0.852, the performance of SVC is better than the baseline model with hyperparameter tuning but worse than the original baseline logistic regression model. This might be because of the characteristics of SVC, since the two pumpkin seeds look not too much different and have overlapping feature distributions, so that there is not a very clear division line between two class.

## Technologies

- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Project Structure

```text
.
├── binary_classification.ipynb
├── README.md
├── data/
    └── Pumpkin_Seeds_Dataset.xlsx

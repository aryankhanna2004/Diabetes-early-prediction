# Diabetes Risk Prediction Model

## Overview
This project aims to develop a classification model to predict early-stage diabetes using various medical predictor variables. The dataset contains 520 observations of 17 variables, where each entry represents a medical profile of individuals assessed for diabetes risk.

## Dataset
The `diabetes_risk_prediction_dataset.csv` contains medical predictor variables such as Age, Gender, Polyuria, Polydipsia, and others which are symptoms or characteristics indicating diabetes risk. The dataset is well-structured with no missing values and comprises binary as well as numerical variables.

## Prerequisites
Before running the prediction models, ensure you have the following R packages installed:
- `tidyr`
- `dplyr`
- `reshape2`
- `mlr`
- `VIM`
- `ggpubr`
- `corrplot`
- `ggplot2`
- `e1071`
- `caret`

## Models
Two machine learning models were employed in this project:
1. Support Vector Machine (SVM)
2. Neural Network (NN)

Both models underwent hyperparameter tuning to maximize accuracy. The training and test set accuracies were recorded, along with the ROC curves and misclassification errors.

## Results
The SVM model showed a test set accuracy of 95.35% with the default settings and improved to 95.95% after hyperparameter tuning. The NN model, after tuning, achieved a test set accuracy of 92.48%. While the NN model performed slightly better in training, the SVM model demonstrated better generalization on the test set.

## Usage
To run the prediction models and replicate the study, follow these steps:
1. Load the dataset using `read.csv("diabetes_risk_prediction_dataset.csv")`.
2. Preprocess the data by converting character variables to factors and performing dummy encoding as necessary.
3. Partition the data into training and test sets.
4. Build and train the SVM and NN models using the `e1071` and `nnet` packages, respectively.
5. Evaluate the models' performances using accuracy, ROC curves, and error rates.

## Conclusion
Both models performed well on the diabetes dataset. However, due to its higher accuracy and better generalization, the SVM model is recommended for predicting diabetes risk.

## Authors
- Aryan Khanna
- Baixi Jiao
- Jasmine Kellett

## Acknowledgements
This project was conducted as part of the Data Analysis curriculum under the guidance of Apostolos Gournaris. We extend our gratitude to him for his support and insights.

## License
This project is licensed under the MIT License - see the LICENSE.md file for details.


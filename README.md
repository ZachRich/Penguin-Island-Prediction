# Palmer Archipelago (Antarctica) Penguin Island Prediction Study
## Overview
This study focuses on predicting the island of origin for penguins based on a range of attributes including species, culmen length and depth, flipper length, body mass, and sex. Utilizing the penguins_size.csv dataset, we conducted an exploratory data analysis to understand the distribution of these attributes across different penguin species and islands.

https://www.kaggle.com/datasets/parulpandey/palmer-archipelago-antarctica-penguin-data?resource=download&select=penguins_size.csv

## Data Analysis
Our analysis began with a descriptive statistical overview of the dataset, followed by visualizations such as histograms and box plots to explore the distribution of physical characteristics among the penguins. These initial insights revealed notable differences in measurements across species, suggesting the potential for these attributes to predict a penguin's island of origin.

![distribution](https://github.com/ZachRich/Penguin-Island-Prediction/assets/32521939/73b74bd8-c4bb-4bbb-aaeb-9135a6b5a788)
![measurementBySpecies](https://github.com/ZachRich/Penguin-Island-Prediction/assets/32521939/0acbdd8f-b992-4022-8627-9e79934761e9)

# Model Development

## Data Preparation
We prepared the data by dropping rows with missing values and encoding categorical variables (species and sex) to numerical form, making the dataset suitable for machine learning models.

## Model Selection
A Random Forest classifier was chosen for this classification task due to its robustness and ability to handle both numerical and categorical data. This model is well-suited for classification tasks and is capable of capturing complex relationships in the data.

## Model Training and Tuning
The initial model was trained with default hyperparameters, achieving an accuracy of approximately 62.69% on the test set. To improve performance, we conducted hyperparameter tuning using Grid Search CV, which identified an optimal configuration that improved the cross-validation score to approximately 70.79%.

## Conclusion and Future Work
Unfortunatley the model currently has an accuracy of 62% when predicting the island of a penguin.
But the study demonstrates the feasibility of using machine learning to predict the island of origin for penguins based on physical and species attributes. While the model achieved reasonable accuracy, there's potential for further improvement through extended hyperparameter tuning, feature engineering, and exploring alternative modeling approaches.

Future work could also explore the impact of additional features, more advanced machine learning models, and techniques to handle imbalanced data, aiming to enhance the model's predictive accuracy and generalizability.

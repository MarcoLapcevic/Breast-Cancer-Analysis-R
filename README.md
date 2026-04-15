# Overview

This project uses three datasets:

- breast-cancer.data
- breast-cancer_1.name
- NOTE: I have yet to add the third dataset file here

These datasets are derived from the Breast Cancer dataset specifically from th UCI Machine Learning Repository, and are used for 
classification tasks specifically predicting whether a patient will experience a recurrence of breast cancer.

## 1. Data Preprocessing

a. Handle missing values appropriately

```
# Load libraries
library(tidyverse)
library(caret)

# Load the cleaned dataset
data <- read.csv("breast-cancer.csv")

# Inspect structure
str(data)
summary(data)

# Fix column names
colnames(data) <- c(
  "Class",          # recurrence-events / no-recurrence-events
  "Age",
  "Menopause",
  "TumorSize",
  "InvNodes",
  "NodeCaps",
  "DegMalig",
  "Breast",
  "BreastQuad",
  "Irradiat"
)
```

b. Encode categorical variables as needed

```

```

c. Normalize or standardize features if required

```

```

## 2. Data Visualization

a. Create at least 3 meaningful visualizations to explore data distributions and relationships 

## 3. Model Building

a. Split the dataset into 75% training and 25% testing sets

b. Train the following classification modes:

- Decision Tee

- Support Vector Machine

- K-Nearest Neighbors

## 4. Cross-Validation Model Evaluation

Compare model performance across all 3 models using the following metrics:

- Accuracy

- Sensitivity (Recall)

- Specificity

- ROC/AUC

## 5. Fairness and Bias Evaluation

a. Evaluate your models for potential bias or unfairness across 
subgroups (e.g., sex, age group, race if available) by choosing at least one demographic variable from your dataset (e.g., gender, age group).

b. If bias is found, perform data processing steps to mitigate bias in the data. If bias is not found, be prepared to justify why mitigation steps are not needed.

## 6. Test Set Model Evaluation

a. Compare model performance across all 3 models using the following metrics:

- Accuracy

- Sensitivity (Recall)

- Specificity

- ROC/AUC

b. Compare differences in performance between the cross-validation and test results.

c. Create at least one visualization comparing test set model performances across the 3 models

## Authors

- Marco A. Lapcevic (Liaison)
-
-
-
-

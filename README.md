# Kaggle Competitions

## Overview

This repository acts as a central point for all the Kaggle competitions I compete it. There is a template branch I easily clone that contains my preferred file structure for data science projects. They are broadly split into two groups: ones with monetary rewards and the playground series (no monetary reward).

## Table of Contents

## Tabular Playground Series

- ### [S2E6 - Imputation](playground/TPS-06-22/readme.md) (132/884)
  - Missing value prediction on a synthetic dataset of 1 million samples and 81 features
  - Leveraged EDA to reduce training time and apply feature engineering
  - Designed a multi-head Multilayer Perceptron with skip connections and _mish_ activator
  - Things I learned:
    - Many different techniques to impute missing data
    - How imperative a thorough EDA is
    - How different MLP architecture can reduce training time while maintaining the same accuracy
- ### [S2E7 - Clustering](playground/TPS-07-22/README.md) (42/1253)
  - Predict clusters on a 98000 sample 29 feature synthetic dataset
  - Due to the lack of ground truth data and evaluation metric (Adjusted Rand Score), a brute force method was used instead of the usual cross validation
  - 2 stage approach to predictions:
    - Use a clustering model to predict clusters
    - Train classifiers on the high confident predictions from the clustering model and ensemble
  - Things I learned:
    - Some functionality of the SK-Lego library, this was necessary for the score I achieved
    - How to implement the pseudo-labelling technique
    - How to make a custom soft voting ensemble
- ### [S2E8 - Regularization](playground/TPS-08-22/README.md) (519/1888)
  - Synthetic dataset 26500 samples 26 features mimicking a real-world product test
- ### [S2E10 - Rocket League](playground/TPS-10-22/README.md) (354/463)
- ### [S3E5 - Quadratic Weighted Kappa](playground/S3E5/README.md)
- ### [S3E10](playground/S3E10/README.md)
  
## Monetary Rewards:
- ### [American Express - Predict Loan Defaults](AE-Loan_Default/README.md)
- ### [Women in Data Science](WiDS/README.md)
- ### [RSNA - Breast Cancer](cancer/README.md)
- ### [BirdCLEF 2023](birds/README.md)
- ### [IceCube - Neutrinos in Deep Ice](ice-cube/README.md)
- ### [Google - Isolated Sign Language Recognition](sign-language/README.md)

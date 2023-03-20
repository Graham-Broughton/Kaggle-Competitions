# Kaggle Competitions

## Overview

This repository acts as a central point for all the Kaggle competitions I compete it. There is a template branch I easily clone that contains my preferred file structure for data science projects. They are broadly split into two groups: ones with monetary rewards and the playground series (no monetary reward).

## Table of Contents

__Playground:__

- [S2E6 - Imputation](#s2e6---imputation-132884) (132/884)
- [S2E7 - Clustering](#s2e7---clustering-421253) (42/1253)
- [S2E8 - Regularization](#s2e8---regularization-5191888) (519/1888)
- [S3E10](#s3e10)

__Monetary:__
- [RSNA - Breast Cancer](#rsna---breast-cancer) (962/1687)
  - 314 Gigabyte dataset of ~55000 images from ~12000 patients in the form of DICOM files, with an accompanying auxiliary csv
  - 
- [Women in Data Science](#women-in-data-science)
- [BirdCLEF 2023](#birdclef-2023)
- [IceCube - Neutrinos in Deep Ice](#icecube---neutrinos-in-deep-ice)
- [Google - Isolated Sign Language Recognition](#google---isolated-sign-language-recognition)

## Competition Summary & Links

### Tabular Playground Series

- #### [S2E6 - Imputation](playground/TPS-06-22/readme.md) (132/884)
  - Missing value prediction on a synthetic dataset of 1 million samples and 81 features
  - Leveraged EDA to reduce training time and apply feature engineering
  - Designed a multi-head Multilayer Perceptron with skip connections and _mish_ activator
  - Things I learned:
    - Many different techniques to impute missing data
    - How imperative a thorough EDA is
    - How different MLP architecture can reduce training time while maintaining the same accuracy
- #### [S2E7 - Clustering](playground/TPS-07-22/README.md) (42/1253)
  - Predict clusters on a 98000 sample 29 feature synthetic dataset
  - Due to the lack of ground truth data and evaluation metric (Adjusted Rand Score), a brute force method was used instead of the usual cross validation
  - 2 stage approach to predictions:
    - Use a clustering model to predict clusters
    - Train classifiers on the high confident predictions from the clustering model and ensemble
  - Things I learned:
    - Some functionality of the SK-Lego library, this was necessary for the score I achieved
    - How to implement the pseudo-labelling technique
    - How to make a custom soft voting ensemble
- #### [S2E8 - Regularization](playground/TPS-08-22/README.md) (519/1888)
  - Predict failure on a synthetic dataset of 26500 samples 26 features which mimicked a real-world product test
  - Tricky competition with a lot of missing values and some features were strongly correlated with the target but not produce great results
  - Final model was an untuned Logistic regressor with a few engineered features
  - Things I learned:
    - The importance of creating a robust cross validation method, tricky for this one because the test set had categorical data and groups that was not in the training data
    - Missing data can be engineered into features
- #### [S3E10](playground/S3E10/README.md)
  
### Monetary Rewards

- #### [RSNA - Breast Cancer](cancer/README.md) (962/1687)
- #### [Women in Data Science](WiDS/README.md)
- #### [BirdCLEF 2023](birds/README.md)
- #### [IceCube - Neutrinos in Deep Ice](ice-cube/README.md)
- #### [Google - Isolated Sign Language Recognition](sign-language/README.md)

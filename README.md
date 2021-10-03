# Türkiye İş Bankası Machine Learning Challenge #2

A submission for [Türkiye İş Bankası Machine Learning Challenge #2](https://www.kaggle.com/c/ml-challenge-turkiye-is-bankasi-2/overview)

**team:** -
**members:** [@mustafahakkoz](https://github.com/mustafahakkoz)
**rank:** 50/94
**score (RMSLE):** 0.17970
**dataset:** [Transaction Amounts](https://www.kaggle.com/c/ml-challenge-turkiye-is-bankasi-2/data) A realistic dataset to predict future total transaction amount per sector for regression tasks. Since there are very few attributes, mining external features are encouraged such as inflation data, salary payment days, exchange rates, seasonal temperature ...

- training dataset ( 200.16 MB, 3.53M rows, 8 cols)

- 2 testing datasets ( 11.53 MB, 220K rows, 8 cols)

Implementation details can be found in notebooks.

---

#### Online Notebooks:

1. a. [EDA and preprocessing](https://www.kaggle.com/areukolateamleader/isbankasi-eda-preprocessing)
   b. [EDA and preprocessing alternative (without scaling)](https://www.kaggle.com/areukolateamleader/isbankasi-eda-preprocess-noscaling)
   c. [EDA and preprocessing alternative (without scaling and feature elimination)](https://www.kaggle.com/areukolateamleader/isbankasi-eda-preprocess-noscaling-noelimination)

2. a. [Overfitting XGBoost model](https://www.kaggle.com/hakkoz/isbankasi-overfit-xgboost)
   b. [Overfitting CatBoost model](https://www.kaggle.com/hakkoz/isbankasi-overfit-catboost)

3. a. [RandomizedSearch with XGBoost](https://www.kaggle.com/areukolateamleader/isbankasi-randomizedsearch-xgboost)
   b. [RandomizedSearch with CatBoost](https://www.kaggle.com/areukolateamleader/isbankasi-randomizedsearch-catboost)
   c. [RandomizedSearchwith XGBoost (Expanded search space)](https://www.kaggle.com/hakkoz/isbankasi-randomizedsearch-xgboost-expanded)
   d. [RandomizedSearchwith CatBoost (Expanded search space)](https://www.kaggle.com/hakkoz/isbankasi-randomizedsearch-catboost-expanded)
   e. [RandomizedSearchwith LightGBM (Expanded search space)](https://www.kaggle.com/areukolateamleader/isbankasi-randomizedsearch-lightgbm-expanded)

4. a. [BayesianOptimization with XGBoost](https://www.kaggle.com/hakkoz/isbankasi-bayesianoptimization-xgboost/)
   b. [BayesianOptimization with XGBoost (Expanded search space)](https://www.kaggle.com/areukolateamleader/isbankasi-bayesianoptimization-xgboost-expanded)

---

#### Repo Content and Implementation Steps:

[**1.isbankasi-eda-preprocessing.ipynb**]()

- Binning ordinal columns by KBinsDiscretizer

- Creating new features by 1-level groups

- Creating new features by 2-level groups

- Filling NaN values by means of each group

- Handling date column and creating new features by seasonal, yearly and monthly groups

- Mining external data such as economic indicators (17 cols) and exchange rates (2 cols).

- TargetEncoding for categorical columns

- MinMaxScaler for normalization

- Feature elimination by pearson correlation (52 -> 44)

- Feature elimination by PCA on external data columns (17+2 -> 3)

- Analyzing data by [pps (predictive power score)](https://github.com/8080labs/ppscore)
  
  

# kaggle-housing-prices
## Project: Housing Prices Regression

### Overview
Predict housing prices using Ridge regression on the Ames, Iowa Housing Prices dataset available as [Kaggle competition](https://www.kaggle.com/c/house-prices-advanced-regression-techniques). 
Final model scored RMSE 0.12132 with 10-fold cross validation and RMSE 0.12498 on Kaggle test set.

### Language
Python

### Packages Used
numpy, pandas, sklearn, scipy, matplotlib, seaborn

### Data Cleaning and Preparation
- replaced mis-spelled entries in categorical features
- tested filling nan values using linear regression between 2 features to estimate fill values, ultimately decided to fill with median values of feature subset
- filled nan values with mean or mode of feature subset
- encoded categorical features with ordinal and one hot encoding

### Feature Selection and Engineering
- removed price outliers from training set
- removed features with mutual information score = 0
- created new features from combinations of existing features
- clustered two features with K-means to form new feature
- dropped selected feature columns

### Model
- Ridge regression

### Resources
[Kaggle](https://www.kaggle.com/)

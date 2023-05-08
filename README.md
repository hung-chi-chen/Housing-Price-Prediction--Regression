# Project Description
This repository contains my solution for the "House Prices - Advanced Regression Techniques" competition on Kaggle. The objective of the competition is to predict the sale prices of houses in Ames, Iowa based on various features such as the size of the house, the number of rooms, the quality of the materials used, etc.

## Data
The dataset contains 79 features and 1,460 observations for the training set and 79 features and 1,459 observations for the test set. The target variable is the sale price of the house. The data can be found on the Kaggle competition page.

## Approach
To solve this problem, I used a combination of exploratory data analysis(EDA), data visualization, feature engineering, and machine learning algorithms. I started by exploring the dataset and visualizing the relationships between the features and the target variable. Then, I performed various data preprocessing steps such as handling missing values, encoding categorical variables, and scaling the data.

To ensure interpretability of the model, I also analyzed the feature importance using the permutation feature importance method. This method measures the decrease in model performance when a feature's values are randomly permuted while keeping all other features unchanged. Features that lead to a large decrease in performance when permuted are considered to be important for the model.

Finally, I trained and tuned several regression models including linear regression, SVM, XGBoost, random forest regression, and light gradient boosting machine. I evaluated the performance of the models using the mean squared error (MSE),root mean squared error (RMSE) , absolute squared error, and R^2 metrics.

## Results
The best performing model was the XGBoost regression model with a R^2 score of 0.8548. The submission to Kaggle achieved a score of 0.13425, which placed me in the top 20% of the competition.

The permutation feature importance analysis revealed that the most important features for the prediction of house prices were:
    
    Weight          Feature
    0.3941 ± 0.0583	Total_SF
    0.1222 ± 0.0406	OverallQual
    0.0241 ± 0.0016	2ndFlrSF
    0.0213 ± 0.0122	BsmtQual-Ex
    0.0147 ± 0.0154	LotArea
    0.0109 ± 0.0046	YearRemodAdd
    0.0106 ± 0.0032	YearBuilt
    0.0103 ± 0.0045	BsmtUnfSF
    0.0071 ± 0.0042	Total_Bath
    0.0059 ± 0.0022	BsmtFinSF1
    0.0058 ± 0.0063	BsmtExposure-No
    0.0053 ± 0.0038	GrLivArea
    0.0050 ± 0.0038	GarageCars
    0.0049 ± 0.0042	TotalPorchSF
    0.0040 ± 0.0024	OverallCond
    0.0036 ± 0.0030	Fireplaces
    0.0033 ± 0.0008	TotalBsmtSF
    0.0027 ± 0.0015	OpenPorchSF
    0.0023 ± 0.0018	KitchenQual-Ex
    0.0020 ± 0.0007	Neighborhood-Crawfor

## External Library
The following packages were used in this project:

  pandas
  numpy
  matplotlib
  seaborn
  scikit-learn
  xgboost
  plotly
  lightgbm
  shap

# Dataset Description
## File descriptions
  train.csv - the training set
  test.csv - the test set
  README.md: this file.
  Housing Price Prediction.ipynb: a Jupyter notebook containing the code for data exploration, feature engineering, and model training.
  
  
## Data fields
Here's a brief version of what you'll find in the data description file.


  SalePrice - the property's sale price in dollars. This is the target variable that you're trying to predict.\
  MSSubClass: The building class\
  MSZoning: The general zoning classification\
  LotFrontage: Linear feet of street connected to property\
  LotArea: Lot size in square feet\
  Street: Type of road access\
  Alley: Type of alley access\
  LotShape: General shape of property\
  LandContour: Flatness of the property\
  Utilities: Type of utilities available\
  LotConfig: Lot configuration\
  LandSlope: Slope of property\
  Neighborhood: Physical locations within Ames city limits\
  Condition1: Proximity to main road or railroad\
  Condition2: Proximity to main road or railroad (if a second is present)\
  BldgType: Type of dwelling\
  HouseStyle: Style of dwelling\
  OverallQual: Overall material and finish quality\
  OverallCond: Overall condition rating\
  YearBuilt: Original construction date\
  YearRemodAdd: Remodel date\
  RoofStyle: Type of roof\
  RoofMatl: Roof material\
  Exterior1st: Exterior covering on house\
  Exterior2nd: Exterior covering on house (if more than one material)\
  MasVnrType: Masonry veneer type\
  MasVnrArea: Masonry veneer area in square feet\
  ExterQual: Exterior material quality\
  ExterCond: Present condition of the material on the exterior\
  Foundation: Type of foundation\
  BsmtQual: Height of the basement\
  BsmtCond: General condition of the basement\
  BsmtExposure: Walkout or garden level basement walls\
  BsmtFinType1: Quality of basement finished area\
  BsmtFinSF1: Type 1 finished square feet\
  BsmtFinType2: Quality of second finished area (if present)\
  BsmtFinSF2: Type 2 finished square feet\
  BsmtUnfSF: Unfinished square feet of basement area\
  TotalBsmtSF: Total square feet of basement area\
  Heating: Type of heating\
  HeatingQC: Heating quality and condition\
  CentralAir: Central air conditioning\
  Electrical: Electrical system\
  1stFlrSF: First Floor square feet\
  2ndFlrSF: Second floor square feet\
  LowQualFinSF: Low quality finished square feet (all floors)\
  GrLivArea: Above grade (ground) living area square feet\
  BsmtFullBath: Basement full bathrooms\
  BsmtHalfBath: Basement half bathrooms\
  FullBath: Full bathrooms above grade\
  HalfBath: Half baths above grade\
  Bedroom: Number of bedrooms above basement level\
  Kitchen: Number of kitchens\
  KitchenQual: Kitchen quality\
  TotRmsAbvGrd: Total rooms above grade (does not include bathrooms)\
  Functional: Home functionality rating\
  Fireplaces: Number of fireplaces\
  FireplaceQu: Fireplace quality\
  GarageType: Garage location\
  GarageYrBlt: Year garage was built\
  GarageFinish: Interior finish of the garage\
  GarageCars: Size of garage in car capacity\
  GarageArea: Size of garage in square feet\
  GarageQual: Garage quality\
  GarageCond: Garage condition\
  PavedDrive: Paved driveway\
  WoodDeckSF: Wood deck area in square feet\
  OpenPorchSF: Open porch area in square feet\
  EnclosedPorch: Enclosed porch area in square feet\
  3SsnPorch: Three season porch area in square feet\
  ScreenPorch: Screen porch area in square feet\
  PoolArea: Pool area in square feet\
  PoolQC: Pool quality\
  Fence: Fence quality\
  MiscFeature: Miscellaneous feature not covered in other categories\
  MiscVal: $Value of miscellaneous feature\
  MoSold: Month Sold\
  YrSold: Year Sold\
  SaleType: Type of sale\
  SaleCondition: Condition of sale

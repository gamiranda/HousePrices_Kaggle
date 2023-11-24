# HousePrices_Kaggle
My solution to the "House Prices - Advanced Regression Techniques" kaggle competition

In this code I used LGBMRegressor, feature engineering and pipeline to reach Score 0.13178. By now, 1104 in the leaderboard. Maybe later I will try to reach a better score, but by now is good enough I believe. In a real world Score 0.13178 would be a very good score.

I used all the feature available in the dataset and created two more:

- TotalArea = LotFrontage + LotArea
- totalFlrSF = 1stFlrSF + 2ndFlrSF

For imputation of the categorical features I imputed them all with "None".

For imputation of the numerical features I used SimpleImputer(strategy='most_frequent').

By last, I transformed the target to log, inspired in another solution. The target transformed to log become pretty normal.

Link to the competition: https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/overview

# HousePrice_prediction_using_LassoRegression
Objective:
1 To practice data cleaning with high dimension feature (81 columns with numerical and catagorical values)
2 To predict house price using regularize regression (Lasso)
Process of this project/competition:
1 Data understanding 
1.1) There are many catagorical values in this dataframe, we will use piority-label encoding with mapping dictionaries
1.2) dependent varible is SalePrice (House Price) --> Distribution of SalePrice is not like a good Normal distribution
[Normal with right skewed] --> we use np.log1p() to normalize SalePrice
Note that: Do not forget to take np.expm1() to predicted value
2 Data preparation 
2.1) Catorical values: Using piority-label encoding by looking bar chart that X is each catagorical column, Y is SalePrice 
--> Grouping [high correlation value to high value]
3 Modeling using Lasso regression
3.1) To tackle overfitting problems and choose significant features given by Lasso regression

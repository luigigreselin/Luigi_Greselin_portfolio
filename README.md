# Porfolio Luigi Greselin

# [Project 1: ING case study](https://github.com/luigigreselin/ING_case_study)

The case study is about predicting the future sales of a number of different liquor shops in un undefined area. Sales of the previous 5 years (from 2012 to 2017) are given weekly for 7 different drink categories. A second dataset reports which shops are present in a radius of 5 km for each single shop to take into account the competition between different shops.

I used the Prophet model released by Fb to predict the total sales. I extracted the yearly trend, for the predicted performance in 2018, and then I classified them with an ANOVA, to check for differences between three homogenehous groups, being no competitors, few competitors and more then 6 competitors. No significant difference was found.

# [Project 2: House price, advanced regression techniques](https://github.com/luigigreselin/HOUSE_PRICE_REGRESSION)

Ask a home buyer to describe their dream house, and they probably won't begin with the height of the basement ceiling or the proximity to an east-west railroad. But this playground competition's dataset proves that much more influences price negotiations than the number of bedrooms or a white-picket fence. With 79 explanatory variables describing (almost) every aspect of residential homes in Ames, Iowa, this competition challenges you to predict the final price of each home.

I compared the results of Random Forest Regressor with GridSearchCV to refine the parameters and a fully connected Neural Network built on Keras. The first one hadd a R squared of 86 % on the cross validation, while the second one was tasted also on a held out dataset (30% of the training dataset) and produced a R squared of 88%.

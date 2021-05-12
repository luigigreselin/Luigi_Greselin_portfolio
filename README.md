# Porfolio Luigi Greselin

# [Project 1: ING case study, TIME SERIES](https://github.com/luigigreselin/ING_case_study)

The case study is about predicting the future sales of a number of different liquor shops in un undefined area. Sales of the previous 5 years (from 2012 to 2017) are given weekly for 7 different drink categories. A second dataset reports which shops are present in a radius of 5 km for each single shop to take into account the competition between different shops.

I used the Prophet model released by Fb to predict the total sales. I extracted the yearly trend, for the predicted performance in 2018, and then I classified them with an ANOVA, to check for differences between three homogenehous groups, being no competitors, few competitors and more then 6 competitors. No significant difference was found.
![](https://github.com/luigigreselin/Luigi_Greselin_portfolio/blob/main/prophet_output.PNG)

# [Project 2: House price, REGRESSION](https://github.com/luigigreselin/HOUSE_PRICE_REGRESSION)

Ask a home buyer to describe their dream house, and they probably won't begin with the height of the basement ceiling or the proximity to an east-west railroad. But this playground competition's dataset proves that much more influences price negotiations than the number of bedrooms or a white-picket fence. With 79 explanatory variables describing (almost) every aspect of residential homes in Ames, Iowa, this competition challenges you to predict the final price of each home.

I compared the results of Random Forest Regressor with GridSearchCV to refine the parameters and a fully connected Neural Network built on Keras. The first one hadd a R squared of 86 % on the cross validation, while the second one was tasted also on a held out dataset (30% of the training dataset) and produced a R squared of 88%.

here below the predicted house prices from the NN on the test dataset

![](https://github.com/luigigreselin/Luigi_Greselin_portfolio/blob/main/predicted%20prices%20with%20NN.PNG)


# [Project 3: Digit Recognition, IMAGE ANALYSIS](https://github.com/luigigreselin/digit_recognition)

MNIST ("Modified National Institute of Standards and Technology") is the de facto “hello world” dataset of computer vision. Since its release in 1999, this classic dataset of handwritten images has served as the basis for benchmarking classification algorithms. In this competition, the goal was to correctly identify digits from a dataset of tens of thousands of handwritten images.

![](https://github.com/luigigreselin/Luigi_Greselin_portfolio/blob/main/digit%20example.jpg =100x20)

I compared random Naive Baesyan classifier, logistic regression, KNN, decision tree, SVC, random forest and XGboost. Logistic regession, SVC, KNN and XGboost required too much time to be trained (Logistic regression failed multiple times to converge), due to the large anount of features (28 by 28 pixels per image). Random forest proved to be the best on training dataset, with an accuracy of 96% on the cross validation score (I then reported the confusion matrix).

Finally I built a CNN with two CL (and 2 dropout layers) and 2 dense layers at the end. In this second case I obtained an accuracy of 98.8 in my test dataset. Below you can see the summary of the CNN

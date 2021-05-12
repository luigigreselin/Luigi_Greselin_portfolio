# Porfolio Luigi Greselin

# [Project 1: ING case study](https://github.com/luigigreselin/ING_case_study)

The case study is about predicting the future sales of a number of different liquor shops in un undefined area. Sales of the previous 5 years (from 2012 to 2017) are given weekly for 7 different drink categories. A second dataset reports which shops are present in a radius of 5 km for each single shop to take into account the competition between different shops.
I used the Prophet model released by Fb to predict the total sales. I extracted the yearly trend, for the predicted performance in 2018, and then I classified them with an ANOVA, to check for differences between three homogenehous groups, being no competitors, few competitors and more then 6 competitors. No significant difference was found.

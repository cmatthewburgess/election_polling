# Predicting the Error of Election Polling in US Federal Elections

## Introduction:
### Problem Statement:
In Presidential, Senatorial, and Congressional elections across the United States, all campaigns and media outlets rely on polling. Exit polls help determine decisions on election day. Polls of Iowa in presidential primaries help determine the front-runner for a given race. But how often do these polls reflect the actual outcome of elections? More importantly, how wrong are they? My goal is to create a regression model that predicts the error of a polls prediction from the actual election.

### Data Set:
I plan on using data from the data news site FiveThirtyEight on polls. It is roughly 10000 rows by 25 columns from polls since 1998. It not only includes data of polls of race by party, but also the year, partisan lean of both the pollster and the district, and real percentage of votes obtained by a candidate. FiveThirtyEight is famous for its election prediction modeling, and they make their data open to the public.

[The data can be found here via FiveThirtyEight's GitHub](https://github.com/fivethirtyeight/data/tree/master/pollster-ratings)

### Application:
Being able to reliably predict the percent error on a poll is arguably one of the single most important things for political campaigns. In knowing the error, polls can be determined as reliable or not, and percent error can be used to make key choices about the campaign moving forward.

# Conclusions

After exploring a variety of algorithms including standard Linear Regression, Lasso Regression, Ridge Regression, and XGBoost Regression, XGBoost ended up providing the best prediction of the error of US Federal election polling. XGBoost's gradient boosting method helps handle model complexity and has fast computation speed. It was able to correctly predict the error of the poll 82% of the time, and those correct predictions had an absolute error of 0.92%. For practical application, this model is a great first step in providing a roadmap for political decision making. Being able to predict the error of a poll can help candidates and the media know how to lead strategy and report on good polling, respectively.

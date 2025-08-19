salesforecastproject

The goal of this project is to accurately predict demand for Walmart stores. This may be useful for anticipating unforeseen demands where product may run out of stock or be in surplus and expire. Using economic features such as CPI, unemployment indexes, and other features like temperature and whether the day is a holiday, a machine learning algorithm may be able to predict demand. This dataset is challenging to work with because of the prevalence of holidays and its cyclical nature. 

The working plan of this project is to:
1. Perform exploratory data analysis (EDA) on the dataset using PowerBI, determining the defining properties of the data and identifying how the machine learning model and doing any possible cleaning. A preliminary report (Walmart Sales Forecast PDF) will also be generated to showcase why the planned design will be used.
2. Produce a final report on the efficacy of the model, the predictions for the next year for each store and overall, and any recommended actions for Walmart.

Walmart Sales Forecast PDF: Some exploratory data analysis done in the Summer of 2024. I discontinued displaying my findings on this PDF not only because I took a long hiatus from this project, but also because I found displaying my findings in the README to make for a much more efficient workflow then editing a latex file and reuploading it every time I made changes.

Findings:

# Walmart's Growth is Stagnating

Year over year sales across all stores is stagnating, increasing by only 1.45% from 2010-2011 and 2.74% from 2011-2012 over the February to September period common across all years.

<img src="media\overall_nominal_sales.jpg" alt="nominal sales" width="400"/>

While the increase in growth rate appears reassuring, it appears that Walmart is only riding greater inflationary trends. By normalizing over CPI, we can calculate the real sales across all Walmarts. The results are much more sobering; with negligible sales changes year over year.

<img src="media\overall_real_sales.jpg" alt="real sales" width="400"/>

Whether the causes include economic downturn, changes in consumer preferences, or other things, it is clear that Walmart's sales strategies must change. 

# Holiday Hangover: Walmart's Christmas Sales Decline

One possible culprit for sales stagnation is the decline in Christmas sales. Real sales on Christmas sunk from $51 million in 2010 too $47 million in 2011, a decrease of about 7.71%.

<img src="media\overall_real_christmas_sales.jpg" alt="real sales" width="400"/>

Given the importance of Christmas as a holiday in terms of sales, this decrease in sales may be partly to blame for stagnating growth. In 2011 (the only complete year in the data), sales on the week of Christmas comprised roughly 3.12% of all sales for the year. The effectiveness of any attempts to remedy this issue, however, remains to be seen.

Christmas sales among stores appear to be declining across the board as well, suggesting systemic issues. Despite overall declines, however, not all stores are affected equally, and some stores were even able to weather the trend and experience growth. Further investigation into store 38 is in line, with an 11.08% growth in real sales change on Christmas. On the other hand, some stores were hit especially hard, namely store 36, with a -25.72% real sales change.

<img src="media\christmas_percent_sales_change.jpg" alt="real sales" width="400"/>

If Christmas sales decreases are the result of changes in consumer preferences, it may be advisable to invest less resources in Christmas promotions. It's possible that the salience of Christmas in American culture is waning, in which case sales declines may be alleviated but are inevitable.

However, some optimism rests in the fact that Christmas week wasn't marked as a holiday in the official data. Only New Year's Eve (the week after) was marked as a holiday, suggesting that Walmart is not running any promotions specific to Christmas. Since Americans generally have their wallets far more open during the Holidays, it may make sense to invest more resources in Christmas or rethink Christmas sales strategies.

If we look at the average real weekly sales for each holiday, we'll find that on average, New Year's sales are often down even compared to regular weeks. Increased purchases during Christmas suggest consumer fatigue which rolls over into the following week. There is also a noticeable gap in sales between Christmas, Thanksgiving, and the rest of the holidays.

<img src="media\overall_real_sales_holiday.jpg" alt="real sales" width="400"/>

With this information, it appears that by diverting resources assigned to New Year's promotions to Christmas, we may find more success with sales.



links:

dataset: https://www.kaggle.com/datasets/yasserh/walmart-dataset/data
geeksforgeeks timeseries pytorch: https://www.geeksforgeeks.org/time-series-forecasting-using-pytorch/
medium recurrent neural networks: https://infolksgroup.medium.com/recurrent-neural-network-and-long-term-dependencies-e21773defd92
geeksforgeeks arima: https://www.geeksforgeeks.org/python-arima-model-for-time-series-forecasting/
dukearima: https://people.duke.edu/~rnau/411arim.htm
Forecasting: Principles and Practice ARIMA: https://otexts.com/fpp2/arima.html
medium stationarity tests: https://medium.com/@ritusantra/tests-for-stationarity-in-time-series-dickey-fuller-test-augmented-dickey-fuller-adf-test-d2e92e214360

salesforecastproject

The goal of this project is to accurately predict demand for Walmart stores. This may be useful for anticipating unforeseen demands where product may run out of stock or be in surplus and expire. Using economic features such as CPI, unemployment indexes, and other features like temperature and whether the day is a holiday, a machine learning algorithm may be able to predict demand. This dataset is challenging to work with because of the prevalence of holidays and its cyclical nature. 

The working plan of this project is to:
1. Perform exploratory data analysis (EDA) on the dataset using PowerBI, determining the defining properties of the data and identifying how the machine learning model and doing any possible cleaning. A preliminary report (Walmart Sales Forecast PDF) will also be generated to showcase why the planned design will be used.
2. Produce a final report on the efficacy of the model, the predictions for the next year for each store and overall, and any recommended actions for Walmart.

Walmart Sales Forecast PDF: Some exploratory data analysis done in the Summer of 2024. I discontinued displaying my findings on this PDF not only because I took a long hiatus from this project, but also because I found displaying my findings in the README to make for a much more efficient workflow then editing a latex file and reuploading it every time I made changes.

Findings:

# Walmart Growth is Stagnating

Year over year sales across all stores is stagnating, increasing by only 1.45% from 2010-2011 and 2.74% from 2011-2012 over the February to September period common across all years.

<img src="media\overall_nominal_sales.jpg" alt="nominal sales" width="400"/>

While the increase in growth rate appears reassuring, it appears that Walmart is only riding greater inflationary trends. By normalizing over CPI, we can calculate the real sales across all Walmarts. The results are much more sobering; with negligible sales changes year over year.

<img src="media\overall_real_sales.jpg" alt="real sales" width="400"/>

Whether the causes include economic downturn, changes in consumer preferences, or other things, it is clear that Walmart's sales strategies must change. 

links:

dataset: https://www.kaggle.com/datasets/yasserh/walmart-dataset/data
geeksforgeeks timeseries pytorch: https://www.geeksforgeeks.org/time-series-forecasting-using-pytorch/
medium recurrent neural networks: https://infolksgroup.medium.com/recurrent-neural-network-and-long-term-dependencies-e21773defd92
geeksforgeeks arima: https://www.geeksforgeeks.org/python-arima-model-for-time-series-forecasting/
dukearima: https://people.duke.edu/~rnau/411arim.htm
Forecasting: Principles and Practice ARIMA: https://otexts.com/fpp2/arima.html
medium stationarity tests: https://medium.com/@ritusantra/tests-for-stationarity-in-time-series-dickey-fuller-test-augmented-dickey-fuller-adf-test-d2e92e214360

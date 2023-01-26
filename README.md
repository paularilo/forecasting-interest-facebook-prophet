**Time series: Prediction of future interest in a topic using Facebook's Prophet Library**

**Overview**
In this small project, I forecasted the interest in the topic 'data science' in the USA from 2004 until 2021 (200 months) using Facebook's Phophet Library. 

**Procedure**
We retrieve the dataset with the interest over time of the keyword \"data science\" since 2004 in the US from [trends.google.com](https://trends.google.com/trends/?geo=US). Interest in a topic is measured as search interest relative to the highest point on the chart for a given region and time. A value of 100 is the peak popularity for the term. A value of 50 means that the term is half as popular. A score of 0 means there was not enough data for the term.

I fitted the time series model on the data of 176 months (training data, 88 %). The 24 last months of the series are used for evaluation (test data). Several performance metrics (mse, rmse, mape) are used for model evaluation. 

**Usefulness**
With very few modifications, this code can be used to calculate evolution of interest in any topic over time with datasets from Google Trends and other providers of topic interest data.

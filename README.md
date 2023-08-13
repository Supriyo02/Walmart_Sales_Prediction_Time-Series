# Weekly_Sales_Prediction_of_a_Store_Time-Series
In this project a Time series ML model have been created to predict the sales of a Walmart store, using the previous sales data of the store, consisting of some other exogenous variabled.

The model comes with 96% accuracy score and fits well with the actual data. It can forecast the future sells of a store almost accurately with the time. The accuracy of the model increases even more if we can provide it some data of the future. It is a beginner friendly simple model, but beats other complex models in it's accuracy score.

SARIMAX model have been used for fiiting the model, as our time series dataset has seasonal component and it also consist of exogenous variables. Some data preprocessing is done before training the model. seasonal_decompose is used for decomposing the dataset and get a insight for any trend, seasonality and residual pattern. I have used auro_arima to estimate the parameters (p,d,q), (P,D,Q,m) and from the time series graph and have visually estimated the probable seasonal duration(m). The exogenous variables are taken in consideration as they affects our target variable, and so the model accuracy has also been increased. The dataset is splitten in test and training dataset and the SARIMAX model is trained on the training dataset. After training the model, predictions are made and they are plotted against the actual test dataset, and they fits well. Lastly the accuracy of the model is calculated.   

[This project is solely made by me, after a lot of try, and nights' work. As clear explanations of sarimax model for beginners, implementing it with exogenous variables isn't much available in the web, it took much time to understand the concept and find a dataset according to my needs]

The actual dataset is taken from Kaggle and then compressed according to our need. Among the 45 store data provided in the kaggle dataset we have taken thr data of only one store, to predict the future sales of the particular store -
[Kaggle Dataset](https://www.kaggle.com/datasets/yasserh/walmart-dataset)

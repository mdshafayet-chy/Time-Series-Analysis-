# Time-Series-Analysis-

This project has been done with challenging time-series dataset consisting of daily sales data, kindly provided by one of the largest Russian software firms - 1C Company.The aim of this project is to predicts the total yearly sales of the 1C company.Dataset collected from Kaggle.

Data Set:
   - sales_train.csv - the training set. Daily historical data from January 2013 to October 2015.

Data fields
   - ID - an Id that represents a (Shop, Item) tuple within the test set
   - shop_id - unique identifier of a shop
   - item_id - unique identifier of a product
   - item_category_id - unique identifier of item category
   - item_cnt_day - number of products sold.
   - item_price - current price of an item
   - date - date in format dd/mm/yyyy
   - date_block_num - a consecutive month number, used for convenience.January 2013 is 0,February 2013 is 1,...,October 2015 is 33
   - item_name - name of item
   - shop_name - name of shop
    -item_category_name - name of item category
    
This dataset is permitted to be used for any purpose, including commercial use.

-----------Workflow----------------
1. Import Dataset
2. Remove out-lier 
3. Groupby dataset by df_train.groupby(['date_block_num']) and the aggregate dataset by df_train.['item_cnt_day']
4. Check Stationary using adfuller method
5. Finding AR term 
6. Splitting data set into train and test
7. Finding MA term
8. Applying Auto_ARIMA 
9. Evaluate Auto_ATIMA model
10. Applying Seasonal_ARIMA
11.Evaualte SeasonaL_ARIMA

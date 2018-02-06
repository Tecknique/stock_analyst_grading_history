## Stock Analyst Upgrade Downgrade History

### Install

* requires 'pip' 

```
pip install pandas
pip install pandas-datareader
-m pip install matplotlib
-m pip install requests
pip install tqdm
```

### Description stock_upgradedowngradeHistory.ipynb

* the database is already created within the folder databases, it isn't important to run this code. This is just a reference of methodology.

* stock_upgradedowngradeHistory: Code used to scrape, clean, and combine data into relevant dataframes.
* Webscraped Yahoo Finance stock analyst data using BeautifulSoup4 and JSON
* Python Pandas to combine JSON objects into DataFrames
* Joined Upgrade Downgrade data with stock ticker historical data
* Combined grading terms into 5 different terms: Strong Buy, Buy, Hold, Sell, and Underperform
* added 1 day before, 1 day after, 30 days after, 60 days after, and 90 days after dates, prices, and percent changed from Open

* returned final dataframe with following columns

[['stockTicker',
 'Date',
 'Open',
 'Close',
 'Volume',
 'firm',
 'action',
 'fromGrade',
 'fromGrade_combined',          
 'toGrade',
 'toGrade_combined',
 '1_day_before_grade_Date',
 '1_day_before_grade_Date_Price',
 'percent1Before',
 '1_day_from_grade_Date',
 '1_day_from_grade_Date_Price',
 'percent1After',
 '30_days_from_grade_Date',
 '30_days_from_grade_Date_Price',
 'percent30',
 '60_days_from_grade_Date',
 '60_days_from_grade_Date_Price',
 'percent60',
 '90_days_from_grade_Date',
 '90_days_from_grade_Date_Price',
 'percent90']]



### Description: Loaded_Databases.ipynb

* This is the code to run for analysis
* Open with Jupyter Notebook
* Opens from the database folder, snp500merged and securities.csv (securities.csv retrieved from https://www.kaggle.com/dgawlik/nyse )
* run each cell



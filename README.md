# Cryptocurrency-forcasting-Power-BI
This POWER BI project uses data to analyze data of certain cryptocurrencies and predict their future prices.
there are 4 phases in this project :
## Extraction, transformation, loading (ETL) :
- we use a KAGGLE cryptocurrency database, which includes:
Date: observation date
Open: opening price of the given day
High: highest price of the given day
Low: lowest price of the given day
Close: closing price of the given day
Volume: Volume of transactions on the given day
Market Cap: Market capitalization in USD
It is a set of csv files for each currency.
- An Excel file contains general information for each currency.
- A Calendar table created with Date Query : 
function (StartDate as date,EndDate as date, FYStartMonth as number) as table =>

:heavy_check_mark: at the end of this phase we obtain our Data Warehouse

## modelization :
build a relational model: the fact table depends on the dimension table.
- Each dimension table represents an axis of analysis.

![1](https://user-images.githubusercontent.com/94402429/213493158-32e2b288-04dd-43ab-9a65-b3ee6e8e2b53.PNG)

## Analyse :
Enrich the data model with Measures and calculated columns using the DAX language.
- calculated columns : is computed at the row level within the table it belongs to. Tt does not depend on what the user does in the report.
-  Measures : is evaluated in the context of a DAX visualization or query.
it changes all the time based on interaction with the report, allowing you to quickly and dynamically explore the data you want to see.
## Reporting :
visualize data in the form of graphs to build reports and dashboards.
Our project consists of 3 pages:
• HOME
• OVERVIEW
• FORECASTING

**HOME**
![1](https://user-images.githubusercontent.com/94402429/213483873-dfe3e1bc-e4eb-4437-809c-d98d804b7eca.PNG)

**OVERVIEW**
![2](https://user-images.githubusercontent.com/94402429/213483889-45940336-53bd-490f-ab14-c886ca83125f.PNG)
![3](https://user-images.githubusercontent.com/94402429/213483902-03ce6173-af83-4d81-aa9c-7a52aa994065.PNG)

**FORECASTING**
![4](https://user-images.githubusercontent.com/94402429/213483917-cf778972-cd70-47c9-ad8c-d74d2f0a62fb.PNG)

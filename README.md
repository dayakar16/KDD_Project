# E-commerce Sales Prediction

<p align="center">
  <img src="https://www.pixelpool.com/wp-content/uploads/2018/12/retail-solutions-770x516.png" />
</p>

## Group 9 Members
* Dayakar Ravuri 
* Manideep Sadineni 
* Priyanka Satish 
* Rama Sri Saladi 
* Snehal Roy 
* Subramani S Sathiyamoorthi 
* Bhargava Ram Bonala


## Introduction
Demand forecasting is a critical concern for every retail business today. Retailers can no longer rely on inaccurate & legacy approaches to forecast demand. With access to a huge customer data, it is all about how efficiently companies are using this information to derive actionable insights. This is where application of Machine Learning comes in. The models & algorithms enable predicting demand for any products. You also get tailored recommendations and can identify fraudulent practices.

While the pandemic had put a pause on the traditional approaches for brick-and-mortar stores, they are placing greater emphasis on incorporating new tech-led approaches of AI, ML and more to their eCommerce strategy. With changing market dynamics and consumer demand, machine learning algorithms help derive meaningful insights from larger datasets more accurately. These techniques help retailers predict the demand of a product or service, uncover hidden patterns, plan promotional campaigns, analyze & accelerate data processing. All this was not possible with the traditional forecasting methods.

  ### What are the actual benefits?
  * Improved Accuracy – Accurate prediction of actual demand helps in improving operational performance and sales at optimized cost.
  * Better Logistics – Improvement in supply chain management will mean that products would stock up.
  * Improved Customer Relationship – With demand forecasting, you can predict the specific requirements of customers and roll-out products at right time and quantity in the market. This positions you as a reliable brand and can improve customer satisfaction.

#### About the data set:
This is a transnational data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail. This has following columns InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID and Country.

#### Goals:
Inventory prediction:
  An inventory system can also provide you with unparalleled insights into customer behavior, product performance, and channel performance, made possible even for large retailers with huge datasets.

## Data Resource:

Data set is taken from the kaggle website given below: 
https://www.kaggle.com/carrie1/ecommerce-data


## Date Preprocessing : 

We have performed the data preprocessing using data cleaning where we will be detecting and correcting or removing corrupt or inaccurate records from a data set. We first read the data set into data frame and check using head whether it is correctly parsed or not and then we checked for null values in columns and rows removed the null values if any are present and created the new data frame. We also removed the negative values from the quantity and price columns.

## Data Understanding and Exploration: 

In this project we are going to predict the retail sales using various algorithms. For this we explored the data set finding the number of orders of the customer from each country, Customer with the highest number of orders,total amount spent in each country, Most common product descriptions, most common stock codes used in the dataset. We will be taking the amount spent for the future use ie., creating the train and test sets and also for prediction.

## Data Preparation for Modeling: 

We have created the train and test data using the amount spent column where we took 80 percent for the train data and 20 percent for the test data. 

## Modeling, Evaluation and Results

We took LinearRegression, Decision Tree Regressor and Random Forest Regressor models for predicting the sales. We predicted the sales using those three algorithms and calculated the mean absolute error and cross validation for each of them to evaluate their prediction. Based on the results obtained Random Forest Regressor is the best model to predict the sales.


## Future Scope

<p align="center">
  <img src="https://www.comtecinfo.com/rpa/wp-content/uploads/2017/10/How-Data-Analytics-in-Retail-Industry-Can-Help-You-Predict-the-Future.jpg" />
</p>

Predictive analytics is a huge boost to the retail industry to anticipate their customer’s needs with greater certainty. Expand one's understanding of their relationship with individual consumers, to ensure the best of predictive analytics is procured. 

These are the following ways that this can be improved
* Automated, Scalable and Reproducible Data Initiatives.
* Automation and Prediction for Faster, More Accurate Management.
* Complete, Real Time Customer behaviour collection.
* Expanding these insights to other parts of retail industry.

## Conclusion

We were able to get the awareness of sales in the market from the data, different country sales, customer wise sales and amount of money spent by each country. This data helps us to predict the number of sales in the upcoming years. Data cleaning was performed to remove the null values from the rows and columns. In addition we removed the negative values from Quantity and price columns. We have created amount_spent column based on the items price and quantity. We evaluated the Linear Regression, Decision Tree and Random Forest Models based on Mean Obsolute Error and Cross Validation. To properly forecast, it’s imperative that each of their sales managers and sales professionals refers to the same sales stages, uses the same terminology, and ultimately adjusts deals in the machine the same exact way. But we are encountered with some of the InvoiceId, description and stock code inconsistencies of the terminology usage. Which made the whole process of cleaning it. We used google colab before running the notebook. User should upload the dataset to the google colab if any error is observed.
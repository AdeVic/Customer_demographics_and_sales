# Customer demographics and sales data analysis
### By Adelami Niyi Victor

__Catalog Demand__
* This datset contains customer demographics of some stores in US, Italy, Spain, Australia, Germany, France and Canada. It has a total of 204 rows and 62 columns
* The aim of this visualization is to find the prdictor variables that inflences the freight_charges and number of purchase made in stores

### Required Software


Jupyter notebook is needed to run this analysis The following libraries should be installed on the jupyter notebook 
* Pandas 
* Numpy 
* Matplotlib 
* Seaborn

__List of files included in the project__
The following files are in this project: 
1. Customer_demographics_and_sales_Lab5.ipynb 
2. Customer_demographics_and_sales_Lab5.xlsx



### Data Cleaning


__The following cleaning operations were carried out on the dataset__


__`Cleanliness Issues`__
1. The AGE, CUST_ID and ORDER_ID variablee were changed to integer data type
2. The order_time was properly formatted
3. Duplicated rows in the dataset was removed
4. The number of Miss. and Master in the gender code variable is very low therefore they were changed to Mr. and Mrs.
5. Missing Age variables were changed to Null 
6. The columns that were not properlt named were renamed
7. American Express spelling was corrected in the creditcard type column
8. The folowing variables were changed to categorical type:
    - `Gender_code`
    - `Counrty_code`
    - `CREDITCARD_TYPE`
    - `NATIONALITY`
    - `T_TYPE`
    - `PURCHASE_TOUCHPOINT`
    - `PURCHASE_STATUS`
    - `ORDER_TYPE`
    - `GENERATION`

__`Tidieness issues`__


1. Columns __`ADDRESS2, LOCALITY and DRIVER_LICENSE`__ with no value were removed. 
2. The variables were removed and renamed as products:
                                            `'Beer','Wine','Club Soda','Sports Drink','Chips','Popcorn',
                                            'Oatmeal','Medicines','Canned Foods','Cigarettes','Cheese',
                                            'Cleaning Products','Condiments','Frozen Foods','Kitchen Items',
                                            'Meat','Office Supplies','Personal Care','Pet Supplies',
                                            'Sea Food','Spices'`                                      
3. Rows with empty values were deleted
4. The __`POSTAL_CODE_PLUS4, ORDER_POSTED_DATE and ORDER_DATE`__ has too many incomplete data and was deleted
5. __`NATIONAL_ID and CREDITCARD_NUMBER`__ has too much unusable entries and were deleted 


### __Summary of Findings__
* There are more male customers than females. The use of phone at payment touchpoint is more prevalent than desktop. 
* The Dinners Club is mostly used, followed by the VISA card and American Express is the least used.
* Customers pay more with American Express, followed by Master Card, Visa, Dinners Club, JCB, and Discover
* Most of the purchase made in the stores are ocassional, followed by frequent buyes and very few first time buyes.
* Most purchase are either low value or high value. There are few orders with medium value 
* Most transactions happens on the weekend while wednesday is known to have the least number of transactions
* Canada has the highest mean frieght charges, followed by Spain. With France having the least mean freight charges and Italy having the highest inter quartile range
* On average, more money is spent on Tuesday, Thursday and saturday
* There are more men that buys just once from the store, these men may return or may not return to the store


### __Key Insights__
* Encouraging the use of Dinners Club card on phone touchpoint will increase the number of purchase made in each stores. Promotions cand be done to increase this
* The stores should focus more buying low value and highr value products to draw more buyers interest while maintaining the number of medium level products sold
* The nuber of useres in diffrenet generations increases in the following order: Baby Boomers (around 45 to 50 years), Gen X, Gen Y and Gen Z
* Both male and female have similar mean and 25 percentile frieght charges but the female has slightly higher 75th percentile frieght charge


### Acknowledgements and credits


>I will like to acknowledge ALX for giving the opportunity to gain this skill through Udacity I will also like to thank Godswill Ayame the Session Lead and Obinna Iheanachor the Career Coach at Udacity for providing the neccesary assistance during this project. GitHub resources, stackoverflow, and Kaggle has also been of a good help during the implementation of this analysis


### Bugs


The dataset provided does not contain enough detail to enable a time series data analysis which would have been an interesting kind of analysis in this project
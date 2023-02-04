# Big-Mart Sales Predictions
## Discovering the item sales per Outlet type and Size

**James Belk**: 

<p align = "center"> 
  <img src = "https://github.com/jamesbelk0/sales_predictions/blob/39b13cb3d373d922ba6e04f66b74ed0edf828ede/grocery_store.png">
</p>

### Business problem:

Discover the sales per Outlet Size and Type

### Data:
Big Mart Data - https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/#About
For this dataset, there are 8,523 rows and 12 columns

### Data Dictionary:

* Item_Identifier - Unique product ID
* Item_Weight - Weight of product
* Item_Fat_Content - Whether the product is low fat or regular
* Item_Visibility - The percentage of total display area of all products in a store allocated to the particular product
* Item_Type - The category to which the product belongs
* Item_MRP - Maximum Retail Price (list price) of the product
* Outlet_Identifier - Unique store ID
* Outlet_Establishment_Year - The year in which store was established
* Outlet_Size - The size of the store in terms of ground area covered
* Outlet_Location_Type - The type of area in which the store is located
* Outlet_Type - Whether the outlet is a grocery store or some sort of supermarket
* Item_Outlet_Sales - Sales of the product in the particular store. This is the target variable to be predicted.

## To prepare this data, the data was cleaned of extra rows and unneeded columns.The following processes were performed:

### Exploratory Data Analysis

 - During the exploratory data analysis, a bar chart and histogram were used to visualize the quantities of Outlet Sizes and Average Sales
 - This provides a better understanding of the quantity of each for comparisons later.
 
 <p align = "center"> 
  <img src = "https://github.com/jamesbelk0/sales_predictions/blob/d8294734469af5fb95f3c375ab6f771c52e31d7c/Average_Sale_Size.png">
</p>

 - This shows the most sales are sold through the Medium Outlet Size compared to the High and Small. Ruling out an ordinal approach.

## Explanatory Visuals

<p align = "center"> 
  <img src = "https://github.com/jamesbelk0/sales_predictions/blob/d8294734469af5fb95f3c375ab6f771c52e31d7c/Outlet_Size_Count.png">
</p>

This shows the breakdown of the total of Outlet Sizes

- Small: 2388
- Medium: 2793
- High: 932
- Missing: 2410

### Machine Learning Using the Following Models:
  - Linear Regression Model
  - Decision Tree Regressor Model
  - Tuned Decision Tree Regressor Model
## Models Evaluated & Results
- Linear Regression Model (Testing Set):
  - MAE: 847.1571 
  - MSE: 1,297,218.6566 
  - RMSE: 1,138.9551 
  - R2: 0.5617

- Decision Tree Regressor Model (Testing Set):
  - MAE: 1,138.5329 
  - MSE: 2,255,705.5459 
  - RMSE: 1,501.9006 
  - R2: 0.2378

- Tuned Decision Tree Regressor Model (Testing Set):
  - MAE: 762.6076 
  - MSE: 1,172,166.0943 
  - RMSE: 1,082.6662 
  - R2: 0.6039
 
 - The final model chose was a `Tuned Decision Tree` with the max_depth tuned to 5.
 - The Mean Absolute Error was off by about `24.40`.
 - The Mean Squared Error was `54,007`.
 - The Root Meaqn Squared Error had a calculation of `25.2354`.
 

For any additional questions, please contact **jamesbelk0@gmail.com**

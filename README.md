# Mini-project-powerbi
# E-Commerse sales analysis by power bi
# Dashboard pages and visuals
## Data Modelling and DAX
• Created a new Date Table using DAX.
**Syntax Date table = ADDCOLUMNS(CALENDAR(MIN('Calculated data'[Purchase Date]),MAX('Calculated data'[Purchase Date])),"Year",YEAR([Date]),"month Number",MONTH([Date]),"month name",FORMAT([Date],"MMM"),"Day",DAY([DATE]))**
* Established relationship between the caculated data and date table
* Created calculated measures for sales, discount ,customers, and transaction
   # Overall Sales Dashboard
## Cards
* created card for the following items
*  Total Transactions
**TOTAL TRANSCATION = DISTINCTCOUNT('Calculated data'[TID])**
* Total Customers
**TOTAL CUSTOMERS = DISTINCTCOUNT('Calculated data'[CID])**
* Gross Sales
**GROSS SALES = sum('Calculated data'[Gross Amount])**
* Net Sales
**NET SALES = SUM('Calculated data'[Net Amount])**
* Total Discount
**TOTAL DISCOUNT = SUM('Calculated data'[Discount Amount (INR)])**
 ## Line chart:
* created Monthly Net Sales Trend by using line chart by adding date in x-axis and net sales in        y-axis.
## Bar chart
* created  Net Sales by Product Category by using bar chart by adding net sales in x-axis and product catagory in y-axis.
## Donut chart
* created a  Transactions by Purchase Method by using donut chart.
## Slicers
*created slicers for the given items Year, Location, Gender, Product Category

# Customer Analysis
## slicers
* added slicers for age group, product cateogry, location, date, gender
## Customer count by Age Group
* created a clustered column chart to show the total customer by age group.
## Net Sales by Gender
* created a clustered bar chart to net sales by gender category.
## Average Purchase Value by Age Category
* created a pie chart to show the average purchase value by different age category.
## Customer transactions by Location
* created a clustered bar chart to show the customer transaction in different location.
## Matrix comparing age groups and product categories
* created a matrix to show different age group and product cateogry

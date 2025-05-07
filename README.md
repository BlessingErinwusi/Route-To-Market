# Route-To-Market-Trade Depot USING EXCEL

## Step-wise Analysis
![image](https://github.com/user-attachments/assets/fa63249d-20f8-44a6-b996-d8e8c252e2a9)


### Introduction - Data summary
Trade Depot are the top consumer goods producer, importer, and local highest manufacturer in Nigeria. Below is a sample dataset of orders generated on the TradeDepot platform in December 2020.

Each row shows a line item as a component of an order.

The dataset contains 15 columns and 2046 rows. The details of the columns include:
Fields Definitions

OrderedAt Date The Order Date

Order No. The Unique Order Number for Each Order

Customer Name Name Of The Retail Outlet

Producer (The Line Item Producer)

Product The Line Item Product

Category Group (The Broad Category of the Line Item)

Category (The Line Item Product Category)

Variant The Line Item Stock Keeping Unit (SKU)

Quantity (The Quantity Of The Line Item (SKU))

Unit Price (The Unit Price Of The Line Item (SKU))

shippingStatus (The Fulfilment Status Of The Line Item (SKU))

Delivery Date (The Date Delivery Was Attempted)

Delivery Agent (The Delivery Agent The Order Was Assigned To)

Customer Type (The Classification of the customers)

Order Channel (The Channel The Order Was Raised Through)

From this dataset, we answer crucial questions associated with the sales and Orders at Trade Depot. 

## Question 1) Show the following topline numbers in a Dashboard format in Excel.

a) Number of Unique Customers

b) Number of Unique Orders

c) Total Order Value

d) Average Order Value

e) Fulfilment Rate (Order Count)

f) Average Fulfilment Time (In hours)

g) Loss Sale

h) Unique Number of SKUs

i) Average Unique SKUs per Customer

## Answers
### a) Number of Unique Customers
#### Use a PivotTable in Excel to calculate the number of unique customers and the number of unique orders. Details below:

Select the data range that contains the information provided.

Go to the "Insert" tab in Excel.

Click on "PivotTable", and a dialog box will appear.

In the dialog box, make sure that the range you selected is displayed in the "Table/Range" field.

Choose where you want the PivotTable to be placed, either in a new worksheet or an existing one, preferably on a new worksheet.

Click "OK" to create the PivotTable.

In the PivotTable Field List on the right, you will see the fields you mentioned (e.g., "Customer Name" and "Order No.").

Drag the "Customer Name" field to the "Rows" area, and drag the "Order No." field to the "Values" area.

By default, Excel will count the number of orders (since "Order No." is a unique identifier for orders) in the "Values" area. You can see the count of unique orders in the PivotTable.

To calculate the number of unique customers, right-click on the "Order No." field in the "Values" area and choose "Value Field Settings."

In the dialog that appears, choose "Distinct Count" as the summary function. This will give you the count of unique customers based on the "Customer Name."

Click "OK," and now PivotTable will display the count of unique customers.

### b) Number of Unique Orders = 621
=([Quantity]*[Unit Price])
to get the Value then =SUM($K$3:$K$2048) to get the Total Value sum

### c) Average Order Value = 15960.69257
  =AVERAGE([Value]) 

## Question 1 - Dashboard
![image](https://github.com/user-attachments/assets/5439ba41-47dc-42ea-8cd4-fb0daf2b2858)

#2) Answer the following questions using any charts of your choice for visualisation (Show working for all answers provided)





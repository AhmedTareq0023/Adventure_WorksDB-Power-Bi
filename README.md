AdventureWorks-Sales-Dashboard 
![Worksheet1](https://github.com/user-attachments/assets/850e59f9-9e99-49d0-bd31-d9c6c75b2143)

![Worksheet2](https://github.com/user-attachments/assets/1737b6a8-b583-43dc-b2f6-4957343e8500)

![Worksheet3](https://github.com/user-attachments/assets/4abc9e9d-57f6-4b54-8331-3b7700acc54d)

AdventureWorks

Data Source:     https://github.com/Microsoft/sql-server-samples/releases/download/adventureworks/AdventureWorks2022.bak

Conductivity Mode => DirectQuery

Tables: Sales.SalesOrderHeader Sales.SalesOrderDetail Sales.vSalesPerson (view) Sales.SalesTerritory Purchasing.ShipMethod Production.Product Production.ProductSubcategory Production.ProductCategory

Create Status (Add based on ufnGetSalesOrderStatusText function) Create Dates table

-Rename Tables, columns -Remove unused columns

-Denormalized into one table (Merge M Language) Production.Product Production.ProductSubcategory Production.ProductCategory

Contains: PorductID, Product, SubCategory, Category

Solve TotalDue, Tax and Fright by Power Query or DAX

Modelig:

Star Schema

Product Hierarchy

line chart vs. counts (USERELATIONSHIP) orderdate shipdate duedate

Model => Star Schema

Measures

Total no. of Orders Measure
Total SubTotal Measure
Total Tax Measure
Total Freight Measure
Total Due Measure
Total no. of Qty
create DAX table that contains all measures

Visuals: (Use Measures)

Drill Down

Drill Through

Tooltip page

Total no. of Orders Card

Total SubTotal Card

Total Tax Card

Total Freight Card

Total Due Card

Total no. of Orders by OrderDate vs. ShipDate vs. DueDate

Total no. of Orders by Shipmethod

Total no. of Orders by Category, SubCategory, Product

Total no. of Orders by FlagOnlineOffline

Total no. of Orders vs. TotalDue by Territory

Top 5 Sales Perosns (# Orders)
Top 5 Sales Perosns (SubTotal)

Bottom 5 Sales Perosns (# Orders)
Bottom 5 Sales Perosns (SubTotal)

Total Due by Month

Total due vs orders by territory

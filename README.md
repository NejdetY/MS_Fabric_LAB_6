# MS_Fabric_LAB_6
# Power BI - Data Modeling and Merge Operations

This project focuses on practicing data merging and expansion operations using Power Query in Power BI.

## Project Summary

In this exercise, I performed a join operation between two tables: **FactSalesOrder** and **DimProduct**.  
The goal was to enrich the sales data with product names by merging based on a common key.

## Steps Followed

1. Opened the Merge Queries window in Power Query.
2. Selected **FactSalesOrder** as the primary table and **DimProduct** as the secondary table.
3. Chose **ProductKey** as the matching column in both tables.
4. Kept the **Left Outer Join** as the default join type.
5. After merging, expanded the newly added **DimProduct** column.
6. Selected only the **ProductName** field to be added to the FactSalesOrder table.

## Challenge Faced

At first, I encountered the following error:

> **"This table has no rows."**

Upon investigation, I found out that this happened because:
- **FactSalesOrder** table had no data, or
- **ProductKey** values between FactSalesOrder and DimProduct did not match properly.

I resolved this issue by carefully checking the source data and ensuring that ProductKey columns contained valid, matching entries in both tables.

## Key Learnings

- How to perform table merges in Power Query.
- The role and behavior of **Left Outer Join** operations.
- How to expand related table fields after merging.
- Troubleshooting data preview issues in Power Query.

## Tools and Technologies

- Power BI Desktop
- Power Query Editor

---

> This project is a part of my journey to strengthen my data modeling and analytical skills in Power BI.

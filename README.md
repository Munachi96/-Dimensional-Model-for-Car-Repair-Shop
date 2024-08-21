## Dimensional Model for Car Repair Shop
Introduction :
This report presents a dimensional model for a car repair shop, designed to efficiently store and analyze data to provide valuable insights. The process includes identifying key data and designing fact and dimension tables using a star schema.

## Business Requirements
Key Invoice Data:
- Customer Information : Name, address, phone number.
- Vehicle Information : Make, model, year, VIN, etc.
- Job Information : Description, hours, rate, amount.
- Parts Information : Part number, name, quantity, price.
- Invoice Information : Invoice number, date, totals.
- Shop Information : Shop name, address, contact details.

## Facts and Dimensions
Facts:
- Service Charges : Total labor charges.
- Parts Charges : Total parts charges.
- Total Sales : Combined services and parts charges.
- Sales Tax : Amount of sales tax.
  
 Dimensions:<br>
- Customer : ID, name, address, phone number.<br>
- Vehicle : ID, make, model, year, VIN, etc.<br>
- Job : ID, description, hours, rate, amount.<br>
- Part : ID, number, name, quantity, price, amount.<br>
- Shop : ID, name, address, phone, email.<br>
- Date : ID, date, month, year. <br>

## Fact and Dimension Tables
Fact_Sales Table:
- Stores sales-related data and links to dimension tables via foreign keys.

Dimension Tables:

- Dim_Customer : Stores customer information.
- Dim_Vehicle : Stores vehicle details.
- Dim_Job : Stores job/service details.
- Dim_Part : Stores parts information.
- Dim_Shop : Stores shop location details.
- Dim_Date : Stores transaction dates.

## ER Diagram and Table Descriptions
The ER diagram illustrates the relationships between the fact and dimension tables, ensuring efficient data retrieval and analysis.

## Logical Design:
- Customer Dimension : Captures customer demographics.<br>
- Vehicle Dimension : Analyzes sales by vehicle specifications.<br>
- Service Dimension : Assesses service types and financial contributions.<br>
- Part Dimension : Tracks parts sales and inventory.<br>
- Location Dimension : Evaluates geographic sales performance.<br>
- Date Dimension : Identifies sales trends over time.<br> [FULL REPORT HERE ](https://ocs.google.com/document/d/1t2rxDYYZV364g7jhEfuiHsKRX-TLbA0coEEo8ZMtcKY/edit)

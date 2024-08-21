```SQL Code

create table dim_customer (
Customer_ID INT primary key,
Name VARCHAR(255),
Address VARCHAR(255),
Phone_Number INT
)
create table dim_vehicle (
Vehicle_ID INT primary key,
Make VARCHAR(255),
Model VARCHAR(255),
Year INT,
Color VARCHAR(255),
VIN VARCHAR(255),
Registration_Number VARCHAR(255),
Mileage INT
)
create table dim_job (
Job_ID INT primary key,
Job_Description VARCHAR(255),
Hours INT,
Rate DECIMAL,
Amount DECIMAL
)
create table dim_part (
Part_ID INT primary key,
Part_Number INT,
Part_Name VARCHAR(255),
Quantity INT,
Unit_Price DECIMAL,
Amount DECIMAL
)
create table dim_shop (
Shop_ID INT primary key,
Shop_Name VARCHAR(255),
Address VARCHAR(255),
Email  VARCHAR(255),
Phone INT
)
create table dim_date (
Date_ID INT primary key,
Date DATE,
Month INT,
Year INT

)

CREATE TABLE sales (
  sale_id INT PRIMARY KEY,
  date_id INT,
  customer_id INT,
  vehicle_id INT,
  shop_id INT,
  job_id INT,
  part_id INT,
	Service_Charges DECIMAL(10, 2),
	Parts_Charges DECIMAL(10, 2),
	Total_Sales DECIMAL(10, 2),
	Sales_Tax DECIMAL(10, 2),
  FOREIGN KEY (date_id) REFERENCES dim_date(date_id),
  FOREIGN KEY (customer_id) REFERENCES dim_customer(customer_id),
  FOREIGN KEY (vehicle_id) REFERENCES dim_vehicle(vehicle_id),
  FOREIGN KEY (shop_id) REFERENCES dim_shop(shop_id),
  FOREIGN KEY (job_id) REFERENCES dim_job(job_id),
  FOREIGN KEY (part_id) REFERENCES dim_part(part_id)

);

```
    

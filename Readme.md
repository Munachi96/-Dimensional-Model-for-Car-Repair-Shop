```
create table dim_customer (
Customer_ID INT primary key,
Name VARCHAR(255),
Address VARCHAR(255),
Phone_Number INT
)

create table dim_job (
Job_ID INT primary key,
Job_Description VARCHAR(255),
Hours INT,
Rate DECIMAL,
Amount DECIMAL
)

# AdventureWorks_DWi9
Final Project for the Indicium Academy Analytics Engineer course. Full Data Warehouse ELT for the Demo Adventure Works Database

## Data Stack:

* Extract and Load (EL):
    - Kondado

* Transform (T):
    - DBT

* Data Warehouse:
    - Google BigQuery

* Visualization:
    - Google Data Studio

* Orchestration:
    - Apache Airflow


## Business Questions:
These are the business questions to be answered using Dashboards in a DataViz Tool.

* Question:
    - Dimensions -> [AssociatedTable]

1 - Number of Orders, Purchase Amounts and Negotiated Value, by:

    - Product; -> [production.product, sales.salesorderdetail]
    - Card Type; -> [sales.creditcard]
    - Sale reason; -> [sales.salesreason]
    - Date of Sale; -> [sales.salesorderheader]   
    - Client; -> [person.person, sales.customer]
    - Status; -> [sales.salesorderheader]
    - City, State, Country. -> [person.address, person.stateprovince, person.countryregion]

2 - Which products have the the highest average ticket sale by:

    - Month; -> [sale.salesorderheader]
    - Year; -> [sale.salesorderheader]
    - City, State, Country. -> [person.address, person.stateprovince, person.countryregion]

3 - What are the 10 best clients in Total Negotiated Value, by:

    Clients -> [person.person, sales.customer]

    - Product; -> [production.product, sales.salesorderdetail]
    - Card Type; -> [sales.creditcard]
    - Sale reason; -> [sales.salesreason]
    - Date of Sale; -> [sales.salesorderheader]
    - Status; -> [sales.salesorderheader]
    - City, State, Country. -> [person.address, person.stateprovince, person.countryregion]

4 - What are the 5 best cities in Total Negotiated Value, by:

    - Product; -> [production.product, sales.salesorderdetail]
    - Card Type; -> [sales.creditcard]
    - Sale reason; -> [sales.salesreason]
    - Date of Sale; -> [sales.salesorderheader]
    - Client; -> [person.person, sales.customer]
    - Status; -> [sales.salesorderheader]
    - City, State, Country. -> [person.address, person.stateprovince, person.countryregion]

5 - What is the Number od Orders, Purchased Amount and Total Negotiated Value, by:

    - Month; -> [sales.salesorderheader]
    - Year. -> [sales.salesorderheader]

6 - What is the product with the highest Purchased Amount for the reason: "Promotion"

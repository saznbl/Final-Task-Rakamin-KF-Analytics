# Final-Task-Rakamin-KF-Analytics
This repository stores BigQuery syntax and analysis result for the final task in project-based internship program at Kimia Farma

The Task is as follow:
**Importing Dataset to BigQuery**
In this project, you are tasked with importing a dataset that has been provided:
- [kf_final_transaction.csv](https://drive.google.com/file/d/1iDOBdKZ4-kkLhpklQWWrsFvACtI7MCz3/view?usp=sharing), 
- [kf_inventory.csv](https://drive.google.com/file/d/1ihtG2t0V1AO0IAGkGwQaqtba6AxDEKDI/view?usp=sharing), 
- [kf_kantor_cabang.csv](https://drive.google.com/file/d/1vzaasqIeXqqe_jI99dNLaa8nxnoe9OWW/view?usp=sharing), 
- [kf_product.csv](https://drive.google.com/file/d/1739wO7BwtVStHCA4Dcj9xGhlc_blBNbT/view?usp=sharing).
You must import these four datasets to to be a table in BigQuery according to the table name from the dataset, but without the ".csv"

**Create Analysis Table**
In this project, you are also asked to create an analysis table based on the aggregation results of the four existing tables
previously imported. The following are the columns mandatory in the table:
* transaction_id : transaction ID code,
* date : the date the transaction was made,
* branch_id : Kimia Farma's branch ID code,
* branch_name : branch name,
* kota : branch city,
* provinsi : branch province,
* rating_cabang : consumers rating for branch
* customer_name : name of the customer making the transaction
* product_id : product ID code,
* product_name : product name,
* actual_price : product price,
* discount_percentage : discount percentage given on products,
* persentase_gross_laba : the profit percentage that should be accepted from products with the following conditions:
  + Harga <= Rp 50.000 -> laba 10%
  + Harga > Rp 50.000 - 100.000 -> laba 15%
  + Harga > Rp 100.000 - 300.000 -> laba 20%
  + Harga > Rp 300.000 - 500.000 -> laba 25%
  + Harga > Rp 500.000 -> laba 30%,
* nett_sales : price after discount,
* nett_profit : profit earned by Kimia Farma,
* rating_transaksi : customers rating for transaction

**Create Dashboard Performance Analytics Kimia Farma Business Year 2020-2023**
Create this dashboard based on the analysis table that previously created in BigQuery. The dashboard must include:
* Dashboard Title
* Summary Dashboard
* Filter Control
* Data Snapshots
* Comparison of Kimia Farma's profit from year to year
* Top 10 Total provincial branch transactions
* Top 10 provincial Nett sales
* Top 5 Branches with the Highest Ratings, Lowest Transactions
* Indonesia's Geo Map for Total Profit for Each Province
* And other analyzes that you can explore.

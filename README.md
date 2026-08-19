# SQL Business Report – DVD Rental Company (ETL)

**PLEASE VIEW THE "WALKTHROUGH SQL PROJECT" FILE ABOVE TO VIEW THE FULL PROJECT**

## Description
A fictional DVD rental company wants to know which film categories (genres) are 
rented most often by their customers, so they know which categories to invest 
in. This report answers that business question by implementing functions, 
triggers, and a stored procedure to prepare, automate, and refresh a summary 
dataset for analysis.

## What I Built
- **Detailed and summary report tables** designed from a multi-table relational 
  schema (customer, rental, inventory, film, category, and more)
- **A user-defined function** to concatenate category name and ID into a single 
  readable field
- **Multi-table joins** (5 tables) to extract and transform raw rental data into 
  the detailed table
- **A trigger** that automatically updates the summary table whenever new data 
  is added to the detailed table
- **A stored procedure** to refresh both tables on demand, designed to run on a 
  recurring schedule (e.g., via pgAgent) every 3 months

## Key Result
Sports was the most-rented category (1,179 rentals); Music was the least 
(830 rentals) — giving the business a clear, data-driven basis for stocking 
decisions.
<br>
<p align="center">
<b>Business Report Summary Table</b> <br>
<br>
<img src="https://i.ibb.co/1RJZdWZ/summary.png" alt="Summary Table"/>
<br />
<br />

## Languages and Utilities Used
- PL/pgSQL

## Environments Used
- PostgreSQL
- Lab On Demand (Lab Client and DVD Database)

## Other Resources/Credits
- PostgreSQL create trigger. PostgreSQL Tutorial. (n.d.). https://www.postgresqltutorial.com/postgresql-triggers/creating-first-trigger-postgresql/
- Koidan, K. (2020, August 6). Can you join two tables without a common column?. LearnSQL.com. https://learnsql.com/blog/join-tables-without-common-column/
- PostgreSQL CONCAT function. PostgreSQL Tutorial. (n.d.-a). https://www.postgresqltutorial.com/postgresql-string-functions/postgresql-concat-function/
- PostgreSQL create function statement. PostgreSQL Tutorial. (n.d.-b). https://www.postgresqltutorial.com/postgresql-plpgsql/postgresql-create-function/
- Johnson, B. (n.d.). Working with Triggers & Stored Procedures. Panopto. https://wgu.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=cdeef825-e36a-4e9a-a157-aeed0139b592
- Johnson, B. (n.d.-b). Writing & Using Functions in PostgreSQL. Panopto. https://wgu.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=0eabc1aa-1e70-43ac-bb1e-addb013a26e8

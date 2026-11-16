# Author : Peanut

# The Cost Of Redundancy

## 1. The Dangers of Data Redundancy
- When a company stores a customer's physical address in three different tables instead of using one central customers table, it creates data redundancy. This means the same information is stored multiple 
times, which can affect data integrity and cause inconsistencies. For example, when a customer changes their address, the company must update all three tables, whereas only one central customers tables could 
have just been updated. That also causes the database to contain different addresses for the same customer. This can lead to confusion, incorrect deliveries and outdated customer information. Using a single
normalised customers table helps prevent these problems and keeps the data accurate and consistent.

## 2. Primary vs. Foreign Key Enforcement
- A Foreign Key constraint acts as a guardrail by ensuring that a record in one table is linked to an exixting record in another table. It prevents orphan records, which are records that refer to information 
that does not exist in the related table. For example, a company may have a Customers table with a Customer_ID as the Primary Key and an Orders table with Customer_ID as a Foreign Key. If someone tries to 
add an order using a Customer_ID that does not exist in the Customers table, the database will reject the entry. This helps maintain referential integrity and ensures that related records remain connected.



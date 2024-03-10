# DB-Assignment
1. Explain the relationship between the "Product" and "Product_Category" entities from the above diagram.

The relationship between the "Product" and "Product_Category" entities is established through the "Category_id" attribute in the "Product" entity, which serves as a foreign key referencing the primary key "id" of the "Product_Category" entity.
A product can be associated with only one product category, while a product category can have multiple associated products.
This is an example of a one-to-many relationship, where one product category can have multiple products, but each product belongs to only one category. 

2. How could you ensure that each product in the "Product" table has a valid category assigned to it?

 Whenever we try to insert or update a record in the "Product" table, the database will check if the value in the "Category_id" column exists in the "id" column of the "Product_Category" table. If it doesn't find a matching value, it will throw an error, preventing the insertion or update of the record thus ensuring that each product has a valid category assigned to it.

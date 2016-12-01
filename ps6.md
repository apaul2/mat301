#### PS6: Due Dec. 2, 2016
---

1. True or False: MySQL automatically creates an _index_ for any key (foreign and primary).
  False 
2. True or False: You can create an index that can improve performance of the database.
  True
3. True or False: You should use indexes on columns that return a high percentage of data when that column is used as a filter condition in the `WHERE` clause.
  False
4. True or False:  You should use indexes on columns that have a high number of NULL values.
  False
5. True or False:  You should not use indexes on columns that are frequently manipulated.
  False
6. True or False:  You should never consider indexing a column used in a `GROUP BY` clause.
  False
7. What is a disadvantages of using indexes?
  It slows down the speed of queries. Also take up disk space.
8. Decide YES or NO whether an index should be used or not. 
  a. Several columns in a small table
    No
  b. Large table with a lot of data manipulation
    No
9.  Determine which is most restrictive, products in categories 200 or 201 and products manufactured by manufacturer number 72.
  SELECT 
    category_id, manufacturer_id
  FROM
    unemath_Paul.Products
  WHERE
    category_id = '200'
    AND manufacturer_id = '72'
    Six rows returned
    
    SELECT 
    category_id, manufacturer_id
  FROM
    unemath_Paul.Products
  WHERE
    category_id = '201'
    AND manufacturer_id = '72'
    Two rows returned
    
   Prodcuts that has a caterogies of 201 and a manufacturer of 72 is more restictive than the categories of 200 with a manufacturer of 72.
   
10.  Create a VIEW of all products from categories 200 or 201 manufactured by manufacturer 72 or 88. 
  CREATE VIEW Category_Manufacturer AS
  SELECT
    category_id, manufacturer_id
  FROM
    unemath_Paul.Products
  WHERE
    category_id in('200','201')
    AND manufacturer_id in('72', '88')
  

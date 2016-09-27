## Problem Set 3 

1. Define the terms: relation, tuple, attribute, record, and field.
  Relation- are two or more things that cna be related to each other through the sharing of a common entity characteristic. Relations can also mean a table, which also means when two or more concepts, objects, or people that are connected. 
  Tuple- is a row of attribrute values. This can also be called a record.  
  Attribrute- is a characteristic of an entity or object and it has a name and data type. Attribrute can also be called a Field or Column.          
  Record- is the collection of data about one item in the database. This can also be called Tuple or Row.
  Field- cell in a table that holds a single item of data. A field can also be called Attribute or Column.
  
2. What are keys in a relation?

3. What is a surrogate key and how is it used?

4. In the following equation, Area = Length x Width, identify the determinant(s).
  The detminant is this equation would be the Area. This would be the unique idendify because with length and width their could be another value that is the same as the other. 
5. If a relation has no duplicate data, how can you be sure there is always at least one primary key?

6. Give an example of a relation.  Determine a natural key for this relation.

  For question 7 - 8, Consider product *orders*.  In particular, associated with an order is: customer name (first and last), address (street, city, state, zip), phone, email, the products orders (including item, quantity, and price).  

7. Create a relational data model for *orders*.  Consider applying normalization rules (discuss Monday)

8. For customer, could email be used as a primary key?  If so, state why.  Also, if possible to use as a primary key, discuss any disadvantages of using email as a primary key.
  Yes an email can be used as a primary key because it is unique and everybody has their own unqie email address. However it would be the best choice becuase people have more than one, they delete email address, and change email address all the time. This would be a natural key.

9. Given two relations S and R below find the Cartsian Product S x R. 
  S x R
  | 1 | 2 | 3 | 1 | 1 |
  | 1 | 2 | 2 | 2 | 3 |
  | 1 | 2 | 2 | 1 | 5 |
  | 2 | 3 | 3 | 1 | 1 |
  | 2 | 3 | 2 | 2 | 3 |
  | 2 | 3 | 2 | 1 | 5 |
  
10. Find the natural join between the Faculty and Department relations below.

S
--------------
| A | B |
|---|---|
| 1 | 2 |
| 2 | 3 |
---------

R
------------
| C | D | E |
|---|---|---|
| 3 | 1 | 1 |
| 2 | 2 | 3 |
| 2 | 1 | 5 |



Faculty
--------------
| Name | ID | Dept |
|-------|----|----------------|
| Joe | 1 | Chemistry |
| Susan | 2 | Math |
| Tom | 3 | Marine Science |
| Mike | 4 | Math |


Department
------------
| Dept | Chair  |
|---|---|
| Chemistry | John |
| Math | Mike |
| Marine Science | Barry |

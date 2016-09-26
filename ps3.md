## Problem Set 3 

1. Define the terms: relation, tuple, attribute, record, and field.
  Relation is also mean a table and mean when two or more concepts, objects, or people that are connected.
  Tuple is row or record.
  Attribrute is also a Field or Column.
2. What are keys in a relation?

3. What is a surrogate key and how is it used?

4. In the following equation, Area = Length x Width, identify the determinant(s).

5. If a relation has no duplicate data, how can you be sure there is always at least one primary key?

6. Give an example of a relation.  Determine a natural key for this relation.

  For question 7 - 8, Consider product *orders*.  In particular, associated with an order is: customer name (first and last), address (street, city, state, zip), phone, email, the products orders (including item, quantity, and price).  

7. Create a relational data model for *orders*.  Consider applying normalization rules (discuss Monday)

8. For customer, could email be used as a primary key?  If so, state why.  Also, if possible to use as a primary key, discuss any disadvantages of using email as a primary key.
  Yes it can be a unique primary key, however would not be the best because people always change email address and deleted addresses. This is however a natural key.
9. Given two relations S and R below find the Cartsian Product S x R. 
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

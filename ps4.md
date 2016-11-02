## Problem Set 4 

1. Create three tables: Customers, Orders, and OrderItems.
CREATE TABLE `unemath_Paul`.`Customers` (
  `Customer_id` INT NOT NULL,
  `Customer_lastname` VARCHAR(10),
  `Customer_firstname` VARCHAR(15),
  `Customer_email` VARCHAR(45),
  `Zip_id` VARCHAR(9),
  `Customer_address1` VARCHAR(25),
  `Customer_address2` VARCHAR(20),
  `Cell Phone` CHAR(10) NULL AFTER `Customer_address2`,
  PRIMARY KEY (`Customer_id`));

CREATE TABLE `unemath_Paul`.`Orders` (
  `Orders_id` INT NOT NULL,
  `Customer_id` INT NULL,
  `Order_total` DECIMAL(2) NULL,
  `Order_date` DATETIME NULL,
  PRIMARY KEY (`Orders_id`));
  
  CREATE TABLE `unemath_Paul`.`Order Items` (
  `Orderitems_id` INT NOT NULL,
  `Product_id` INT NULL,
  `Customer_id` VARCHAR(45) NULL,
  `Item price` DECIMAL(2) NULL AFTER `Customer_id`,
  `Order_id` INT(11) NULL AFTER `Item Quantity`,
  `Item Quantity` VARCHAR(45) NULL AFTER `Item price`,
  PRIMARY KEY (`Orderitems_id`));
  
  
2. Why do we need an OrderItems table?
  We need a order items table because one customer can buy more than one item and want to 

3. Create linked tables in MS Access.

4. Create forms to enter customer data.

5. Create a form with a subform to enter orders and order item.

6. Use forms created in 4 and 5 to insert Customers and Orders.  Add customers that have not made any orders. Make the number of entries relatively small.  Why?  

7. Use SQL DML to INSERT records into Customers and Orders (and OrderItems).  

8. Find all customer orders.

9. Select all customers that orders a certain product (This will depend on what data you entered into the table).  Find all customers that ordered product 3452.  

10. List 5 questions that you can answer from this data.

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
  INSERT INTO `unemath_quinlan`.`Customers` (`id`,`fname`,`lname`,`phone`,`email`,`address1`,`address2`,`zip`) VALUES 
  (1031,'Imelda','Holcomb','937-484-2402','dolor@necenim.com','8350 Adipiscing Rd.','',99811),
  (1032,'Teagan','Crane','263-915-6116','risus@in.com','139-1596 Nisi Ave','Ap #126-2752 Varius. Ave','LR09 9JR'),
  (1033,'Destiny','Russell','361-305-1439','non@gravida.edu','9135 Magna. Street','963-6955 Lacinia Road','97891'),
  (1034,'Marsden','Dillard','821-151-2410','semper.et@nullaIntincidunt.com','4270 Aliquam Street','',26034),
  (1035,'Slade','Fowler','752-248-5096','tellus.imperdiet@quisturpisvitae.com','4368 Pede. Avenue','Apt 428',31775),
  (1036,'Sawyer','Mullen','201-029-2021','Maecenas.malesuada@Crassed.edu','298-1833 Mauris. Avenue','P.O. Box 905',73223),
  (1037,'Sydney','Guy','578-796-5277','ornare@velitdui.ca','Ap #249-3884 Elit St.','5786 Interdum. Road',26034),
  (1038,'Jessamine','Hall','330-338-1589','jahll@ovbc.edu','8738 Ohio Av.','',43920),
  (1039,'Maryam','Tyler','754-715-7082','malesuada.malesuada@idsapienCras.com','2376 Leo, Ave','',86550),
  (1040,'Cailin','Lamb','673-849-8970','clamb@tinder.com','9481 Road','',26034),
  (1041,'Aimee','Wilson','330-386-2464','amywilson@turpis.com','16160 Cannons Mills Rd.','',43920),
  (1042,'Colorado','Soto','996-590-7892','ut@Fuscemilorem.com','Ap #658-6927 Sociis Rd.','Ap #774-5804 Quis, Rd.',26034),
  (1043,'Eliana','Witt','439-978-0537','ultrices.mauris@purusgravida.com','Lucus St.','',43210),
  (1044,'Lee','Clemons','685-288-2021','Integer@lobortis.net','3085 Neil Ave.','',43201),
  (1045,'Ferris','Stevens','434-012-9560','ac@libero.org','Ap #248-3742 Nullam Av.','P.O. Box 827, 9442 Risus. Street',90210),
  (1046,'Margaret','Harding','787-095-7706','Proin.dolor.Nulla@enim.net','6978 Northest. Ave','',73585),
  (1047,'Suki','Holden','071-229-5461','justo.Proin@dolorvitae.edu','Ap #115-940 Neque. Av.','',02086),
  (1048,'Anastasia','Gillespie','067-183-8599','gillepie@Duis.com','6615 Leo. St.','',98591),
  (1049,'Yetta','Foley','692-366-9700','foley@diamloremauctor.net','2206 Montes, Rd.','Ap 537',56760),
  (1050,'Uriel','Richards','140-598-3289','massa@fringilla.edu','4231 Iaculis Road', 'Ap #305', 98591), 
  (1051,'Sage','Norris','677-467-0246','magna.Sed@Etiam.org','3747 Odio Rd.','P.O. Box 537, 8986 Ac Road',00613),
  (1052,'Neil','Alvarado','920-541-0563','feugiat.placerat@NullafacilisiSed.coom','5994 Sit Ave','',22009),
  (1053,'Tanisha','Finch','813-263-7292','magna@iaculis.edu','3816 Imperdiet Rd.','',22723),
  (1054,'Idola','Bradford','655-053-3758','Etiam.laoreet.libero@blandit.net','508 Enim, Rd.','P.O. Box 264',24522),
  (1055,'Ciara','Diaz','620-470-8510','ipsum.Curabitur@maurissagittis.edu','887-3371 At Street','492-3463 Fermentum Rd.',26034),
  (1056,'Rudyard','Chan','369-193-1499','adipiscing.lobortis@id.com','Ap #409 Varius Av.','Apt 209',24879),
  (1057,'Malachi','Chaney','054-717-3988','lorem@ornareInfaucibus.com','817 Tincidunt. St.','Ap #206',08217),
  (1058,'Baker','Foreman','047-985-7110','luctus.et@rutrum.com','P.O. Box 430, 5374 Arcu Av.','',60041),
  (1059,'Meredith','Browning','309-527-0273','lorem.auctor.quis@Maurisvestibulum.com','749-1071 Leo Rd.','',10757),
  (1060,'Ian','Mooney','946-576-3910','at@imperdiet.com','74501 Suspendisse St.','P.O. Box 895',26034);

8. Find all customer orders.

9. Select all customers that orders a certain product (This will depend on what data you entered into the table).  Find all customers that ordered product 3452.  

10. List 5 questions that you can answer from this data.

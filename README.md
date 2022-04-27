<!-- Note ALL comments will shown like this -->
<!-- I will put code commands inside '<>' -->
<!-- First I will begin by running <mysql-ctl cli> -->

mysql-ctl cli 

<!-- I will the check the databases I have on the system to see -->  
<!-- if I do not have an existing 'foondamate' database created -->
<!-- if have an existing 'foondamate' database created I will change the name -->
 <!-- Since I done I will create a database called 'foondamate' -->
 
CREATE DATABASE foondamate 

<!-- I will the check the to see if the database is craeted  --> 
<!-- Since it has been created, I will use the database to put my work -->

USE foondamate


<!-- I will verify that I'm working with the foondamate database --> 

SELECT DATABASE(); 

<!-- Now, I am working with foondamate database,s I will reveal existing tables  -->

SHOW TABLES;

<!-- There should be no existing table in this database as we just created it -->
<!-- I will create a new table called 'userdata' --> 

CREATE TABLE userdata
( 
    date_y  CHAR(15), 
    data_x  INT
);

<!--  I will reveal the table we just created  -->

SHOW TABLES;

<!--  We should see information about the newly created table -->
<!--  Now we will insert values given to us in the Task Question -->

INSERT INTO userdata(date_y, data_x)
VALUES ("01-01-2022", 300),
    ("02-01-2022", 500),
    ("03-01-2022", 700),
    ("04-01-2022", 1300),
    ("05-01-2022", 2000),
    ("06-01-2022", 3000),
    ("07-01-2022", 3500),
    ("08-01-2022", 4000),
    ("09-01-2022", 4500),
    ("10-01-2022", 5000),
    ("11-01-2022", 20000),
    ("12-01-2022", 35000),
    ("13-01-2022", 46000),
    ("14-01-2022", 70000),
    ("15-01-2022", 90000)
    ;
 
 <!--  I will reveal the table we just created  -->

SHOW TABLES;

<!--  You should see info about newly created table  -->
<!-- I will show column names and type within the new table  -->
 
 DESC userdata;
 
<!-- I will now display all the entries in the userdata table-->
 
 SELECT * FROM userdata;
 
<!-- I will now display all the entries in the userdata table but order it from the earliest date-->

SELECT * FROM userdata
ORDER BY date_y ASC ;

<!-- I will now display all the entries in the userdata table but order it from the latest date-->	

SELECT * FROM userdata
ORDER BY date_y DESC;

<!-- I hope this makes sense, thank you so much. You can find the visual representation on the excel spreadsheet-->	




  

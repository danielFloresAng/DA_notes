

* SELECT --> Selects the data that we want to interact with

* FROM --> Selects the table

* INSERT INTO --> Inserts new data on a table
  > Ej.:
      INSERT INTO `customer_data.customer_address` 
        (customer_id,address,city,state,zipcode,country) <!-- We specified the rows that we want to add data-->
      VALUES  <!--Type the keyword VALUES-->
        (2645,'333 SQL Road','Jackson',"MI",49202,"US") <!--Type the values to insert in the same order that we typed before-->

* UPDATE --> Updates values from a table
  > Ej.:
      UPDATE `customer_data.customer_address` <!-- Select the table with the keyword UPDAT -->
      SET address = '123 New Address' <!-- Use keyword SET and put the row and the new value -->
      WHERE customer_id = 2645 <!-- Specified the row and the value of the column to updat -->



      <!--  -->
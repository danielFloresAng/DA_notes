- SELECT --> Selects the data that we want to interact with
_____________________________________________________________________________
- FROM --> Selects the table
_____________________________________________________________________________
- INSERT INTO --> Inserts new data on a table

  > Ej.:

      INSERT INTO `customer_data.customer_address`
        (customer_id,address,city,state,zipcode,country) <!-- We specified the rows that we want to add data-->
      VALUES  <!--Type the keyword VALUES-->
        (2645,'333 SQL Road','Jackson',"MI",49202,"US") <!--Type the values to insert in the same order that we typed before-->
_____________________________________________________________________________
- UPDATE --> Updates values from a table

  > Ej.:

      UPDATE `customer_data.customer_address` <!-- Select the table with the keyword UPDAT -->
      SET address = '123 New Address' <!-- Use keyword SET and put the row and the new value -->
      WHERE customer_id = 2645 <!-- Specified the row and the value of the column to updat -->
_____________________________________________________________________________
- DISTINCT --> Helps to show just once each value of the table in case that there are duplicate data.

  > Ej.:

      SELECT
        DISTINCT customer_id
      FROM
        `customer_data.customer_address`
_____________________________________________________________________________
- LENGTH --> Checks the lenght of a text string

  > Ej.:

      SELECT
        LENGTH(country) AS letters_in_country <!-- between parenthesis, type the column that we want to make the query , and, opcional, we type AS and a temporal title to see the result of the query -->
      FROM
      `customer_data.customer_address`
_____________________________________________________________________________
- SUBSTR -> Filters the values of a column by the numbers of characters that we specified
  > Ej.:
      SELECT
        DISTINCT customer_id
      FROM
        `customer_data.customer_address`
      WHERE
        SUBSTR(country,1,2) = 'US' <!-- Between paranthesis indicate the column, the first characther and the second character. The we indicate the characters that we want to se after the equal sign(=) -->
_____________________________________________________________________________
- TRIM --> Selects and mantain only the characters that we want in a value, deleting the rest of the characters
  > Ej.:
  SELECT
      DISTINCT customer_id, state, country
  FROM
  `customer_data.customer_address`
  WHERE
  TRIM(state) = 'OH' <!-- Indicate between parenthesis the coulumn, and type the characters that we want to see -->
_____________________________________________________________________________
- CAST --> Can be used to convert anything from one data type to another

  > Ej.:
      SELECT
        CAST(purchase_price AS FLOAT64) <!-- Type CAST, and, between the parenthesis type the column name (purchase_price), and keyword 'AS', then we type the data type that we want to get -->
      FROM
        `projectsqlda.customer_data.customer_purchase`
      ORDER BY
        CAST(purchase_price AS FLOAT64) DESC
_____________________________________________________________________________
- CONCAT --> Adds strings together to create new text strings that can be used as unique keys

  > Ej.:
      SELECT 
        CONCAT(product_code, product_color) AS new_code <!--between parethesis put the columns that we want to concat -->
      FROM 
        `projectsqlda.customer_data.customer_purchase` 
      WHERE
        product = 'couch'
_____________________________________________________________________________
- COALESCE --> Return non-null values in a list

  > Ej.:
      SELECT 
        CONCAT(product_code, product_color) AS new_code <!--between parethesis put the columns that we want to concat -->
      FROM 
        `projectsqlda.customer_data.customer_purchase` 
      WHERE
        product = 'couch'

      <!--  -->

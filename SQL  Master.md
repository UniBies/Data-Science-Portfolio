# SQL Master 

## Basics

### Finding Data Queries

#### **SELECT**: used to select data from a database

* `SELECT` * `FROM` table_name;
  
* `SELECT DISTINCT` * `FROM` table_name;

### Filtering Data

#### **WHERE**: used for filtering data

* `SELECT` * `FROM` table_name <br>
  `WHERE` column_name = 'condition';
  
* `SELECT` * `FROM` table_name <br>
  `WHERE` column_name_1 = 'condition_1' `AND` column_name_2 = 'condition_2';
  
* `SELECT` * `FROM` table_name <br>
  `WHERE` column_name_1 = 'condition_1' `OR` column_name_2 = 'condition_2';

* `SELECT` * `FROM` table_name <br>
  `WHERE` column_name_1  `BETWEEN` 'condition_1' AND 'condition2';

* `SELECT` * `FROM` table_name <br>
  `WHERE` column_name_1 `IN` ('condition_1', 'condition_2', 'condition_3');

* `SELECT` * `FROM` table_name <br>
  `WHERE` column_name_1 `IN` (`SELECT STATEMENT` ...)

* `SELECT` * `FROM` table_name <br>
  `WHERE` column_name_1 `IS NULL`;

* `SELECT` * `FROM` table_name <br>
  `WHERE` column_name_1 `IS NOT NULL`;

* `SELECT` * `FROM` table_name <br>
  `WHERE` column_name_1 `<>` 'condition';

#### **LIKE**: filter data by searching for specific pattern in column

* `%` is a wildcard character that represents zero, one, or multiple characters
* `_` is a wildcard character that represents a single character
* `SELECT` column_name `FROM` table_name <br>
  `WHERE` column_name `LIKE` pattern;
* `LIKE` 'a%' - find any values that starts with 'a'
* `LIKE` '%a' - find any values that ends with 'a'
* `LIKE` '%or%' - find any values that have 'or' in any position
* `LIKE` '_r%' - find any values that have 'r' in the second position
* ` LIKE` 'a_%_%' - find any values that starts with 'a' and are at least 3 characters in length
* `LIKE` '[a-c]%' find any values starting with 'a', 'b' or 'c'

#### **ORDER BY**: used to order data in column in ascending or descending order

* `SELECT` * `FROM` table_name `ORDER BY` column;
* `SELECT` * `FROM` table_name `ORDER BY` column `DESC`;
* `SELECT` * `FROM` table_name `ORDER BY` column `ASC`, column_1 `DESC`;

#### **TOP**: used to specify the number of records to return from top of table

* `SELECT TOP` number * `FROM` table_name `WHERE` condition
* `SELECT TOP` NUMBER * `FROM` table_name `ORDER BY` column

* !! Not all databes systems supports `TOP`. In MySQL there is `LIMIT`
* `SELECT` * `FROM` table_name `LIMIT` offset, count

### FUNCTIONS

#### **CONCAT()**: used to combine columns into one

* `SELECT` `CONCAT`(column_1, ' ', column_2)

#### **LEFT()**: extract characters from a string starting from left

* `SELECT` `LEFT`(column_name, number_of_characters) `FROM` table_name

#### **RIGHT()**: extract characters from a string starting from right

* `SELECT` `RIGHT`(column_name, number_of_characters) `FROM` table_name

#### **SUBSTRING()**: extract characters from a string, starting in position

* `SELECT` `SUBSTRING`(column_name, position, number_of_characters) `FROM` table_name;

#### **LEN()**: return the length of a string

* `SELECT` `LEN`(column_name) `FROM` table_name;
* `SELECT` column `FROM` table_name <br>
  `WHERE` `LEN`(column_name) = 'condition';

#### **REPLACE()**: replace character

* `SELECT` `REPLACE`(column, 'a', 'b') `FROM` table_name;

#### **UPPER()**: change string into uppercase

* `SELECT` `UPPER`(column) `FROM` table_name;

#### **LOWER()**: change string into lowercase

* `SELECT` `LOWER`(column) `FROM` table_name;

#### **LTRIM()**: remove spaces from a left side of string

* `SELECT` `LTRIM`('   string')

#### **RTRIM()**: remove spaces from a right side of string

* `SELECT` `RTRIM`('string    ')

#### **ROUND()**: rounds up number 

* `SELECT` `ROUND`(number, number_of_decimal_places);

#### **FLOOR()**: rounds down to whole number 

* `SELECT` `FLOOR`(2,999) ---> 2

#### **CEILING()** rounds up to whole number

* `SELECT` `CEILING`(2,001) ----> 3

#### **POWER()**, **SQRT()**, **PI()**: mathematical operations

* `SELECT` `POWER`(number, power)
* `SELECT` `SQRT`(number)
* `SELECT` `PI`() 












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

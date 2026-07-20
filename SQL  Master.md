# SQL Master 

## Basics

### Finding Data Queries

#### **SELECT**: used to select data from a database
* `SELECT` * `FROM` table_name;
  
* `SELECT DISTINCT` * `FROM` table_name;

### Filtering Data

### **WHERE**: used for filtering data
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

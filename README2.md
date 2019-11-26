# Tables in SQL
- Remember data types CHAR, CARCHAR and DATA all use quotation marks for their values
- CREATE TABLE table_name (column1 datatype1, column2 datatype2, ...)

## Add Column
- Add a column in a table:
  - ALTER TABLE table_name
    ADD column_name datatype

## Drop Column
- Delete a column in a table:
  - ALTER TABLE table_name
    DROP COLUMN column_name

## Delete Records
- Delete existing records in the table:
  - DELETE FROM table_name WHERE <condition>

## Drop Table
- Delete table:
  - DROP TABLE table_name

## Alter/Modify Column
- To change the data type of the column in a table:
  - ALTER TABLE table_name
    ALTER COLUMN column_name datatype

## Insert Data into Table
  - INSERT INTO table_name (column1, column2, ...) VALUES (value1, value2, ...)

## Updating Table
  - UPDATE table_name
    SET column1 = value1, column2 = value2, ...
    WHERE <condition>

## Primary Key on Create Table
- Primary key constraint uniquely identifies each record in a table, must contain unique values and cannot contain null values
  - CREATE TABLE table_name (
    ID int NOT NULL PRIMARY KEY
    column1 datatype1 NOT NULL,
    column2 datatype2, )

## Primary Key on ALter Table
  - ALTER TABLE table_name
    ADD PRIMARY KEY (ID)

## Drop Primary Key
  - ALTER TABLE table_name
    DROP CONSTRAINT PK_table_name

## Foreign Key on Create Table

   Constraints in SQL
=>Are rules a table column should follow.
1.Not null-> should never be empty
2.Primary key-> unique identity of every record in the table
3.Foreign key-> Used on foreign columns that links to the primary key on the parent
4.Unique-> Used to ensure that every record in the column is unique
5.Default-> It gives a default value when a value is not provided
6.Check-> Allows you to specify a condition that every row in a table must satisfy

create table students(id datatype primary key not null, student_name varchar(255) not null, gender varchar(10) not null, age int not null, adm varchar(100) unique not null);

products(id(pk) buying_price selling_price)

create table products(id type primary_key, buying_price type not null, selling price type not null check(selling_price>buying_price));

     Datatypes
=>The kind of data a column should have
1.INT->All whole numbers
2.Decimal(p,s)->Used for fixed decimal numbers
3.Float->Used for all decimal numbers
4.Varchar(n)->Alphanumeric characters where n is the maximum number of characters
5.Char(n)->Fixed length text where n is the fixed number of characters
6.Text->Massively long texts
7.Date->Store year, mont and day
8.Time->Store times hours minutes seconds
9.Datetime->Both date and time 
10.Timestamp->>Both date and time and autogenerates time and date
Serial->mostly used on primary key and it autoincrement

    
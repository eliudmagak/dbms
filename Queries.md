    Queries
=>Used to interact with SQL databasase
=>We use queries to perform CRUD operations
-> C create (create database, tables, insert data)
-> R read (fetching data that has already been added to the database)
-> U update (updating data on the database)
-> D delete (deleting data on the database) 

    RDBMS(Relational database management system)
postgreSQL-

        psql shell
->Commandline tool used to manage databases
->It only allows commands and queries
->All commands must start with backslash(\)
->All queries must end with a semi-colon(;)

\l->List all the databases you have.

->Create the database using the query

create database database_name;
eg: create database school;

->Connect to the database
\c database name
\c school

->Display tables
     \dt

->Create tables(queries)
 ->create table table_name(column1 datatype constraints, column2 datatype constraints, column3 datatype constraints)

create table students (id in ptimary key, name varchar(10) not null)

\q->To quit psql shell

    Update and Delete Queries
  Update
->Used to edit records in a database table
     syntax
update table_name set column=new_value,column=new_value where condition;

update students set age=40 where id=100;

  Delete
->Removing records from the database table

    Syntax
delete from table name;
delete from students where condition;
delete from students where id=2;



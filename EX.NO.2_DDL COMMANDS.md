# EXP NO 2: DATA DEFINITION LANGUGE COMMANDS 

### DATE: 20/03/2024

## AIM: To create a student database and execute DDL queries using SQL.

## THEORY

### DDL (Data Definition Language)

* DDL or Data Definition Language actually consists of the SQL commands that can be used to define the database schema.
* It simply deals with descriptions of the database schema and is used to create and modify the structure of database objects in the database.
* DDL is a set of SQL commands used to create, modify, and delete database structures but not data.
* These commands are normally not used by a general user, who should be accessing the database via an application.

 
### List of DDL commands: 
1. CREATE: This command is used to create the database or its objects (like table, index, function, views, store procedure, and triggers).
2. DROP: This command is used to delete objects from the database.
3. ALTER: This is used to alter the structure of the database.
4. TRUNCATE: This is used to remove all records from a table, including all spaces allocated for the records are removed.
5. RENAME: This is used to rename an object existing in the database.

## Query:

### 1) Create a table student  and insert any two rows with the following fieds RegisterNumber,Name,Age,Address,Phone number

### SQL QUERY: 
```
 create table learner(RegisterNumber int,Name varchar(100),Age int,Address varchar(250),PhoneNumber int) ;
```

### OUTPUT:
![image](https://github.com/SivaramakrishnanBaskar/DBMS/assets/119476322/851aa02c-f946-445d-8155-9ebcb0e637eb)

### 2) Alter the above student table by adding another attribute department

### SQL QUERY: 
```
 alter table learner add Collage varchar(20);
```

### OUTPUT:
![image](https://github.com/SivaramakrishnanBaskar/DBMS/assets/119476322/66d02ad3-ff8e-441a-8b86-0ef9b658177d)

### 3) Rename the student table to mystudent

### SQL QUERY: 
```
 rename learner to students;
```

### OUTPUT:
![image](https://github.com/SivaramakrishnanBaskar/DBMS/assets/119476322/e75f4fa8-6fe1-40c9-bdfb-d21482a15a7d)

### 4) Delete the mystudent rows using truncate keyword

### SQL QUERY: 
```
 truncate table students ;
```

### OUTPUT:
![image](https://github.com/SivaramakrishnanBaskar/DBMS/assets/119476322/6f10dc12-5b27-4200-833e-a85882e9c3ba)

### 5) Drop the mystudent table
 
### SQL QUERY: 
```
 drop table students;
```
### OUTPUT:
![image](https://github.com/SivaramakrishnanBaskar/DBMS/assets/119476322/42d72dc3-db28-4644-b090-b2615e46960a)

## Result:
Thus the basic DDL commands in SQL are executed. 

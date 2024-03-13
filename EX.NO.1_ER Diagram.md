# EXP NO 1: ER DIAGRAM CREATION, RELATIONAL MODEL AND SCHEMA GENERATION  
### DATE
## AIM:
<div align="justify">
   To create a ER Diagram for Bank management system or College management system using ERD Plus tool and generate the relational model with schema. 
</div>

## Algorithm
1. Create a login with https://erdplus.com.
2. Create a new ER Diagram with name
3. Create a strong entity, relation and attributes.
4. Create a weak entity, relation and attributes.
5. Specify attributes unique, multivalued and composite attributes.

### ER Diagram 
![alt text](<WhatsApp Image 2024-03-13 at 11.34.26_7a416f4d.jpg>)

### Relational model
![alt text](<WhatsApp Image 2024-03-13 at 11.34.25_6bfb0bcb.jpg>)

### SQL DDL Schema 
```sql
CREATE TABLE Employee
(
  FName INT NOT NULL,
  LName INT NOT NULL,
  Minit INT NOT NULL,
  Address INT NOT NULL,
  Salary INT NOT NULL,
  Bdate INT NOT NULL,
  Ssn INT NOT NULL,
  Sex INT NOT NULL,
  PRIMARY KEY (Ssn)
);

CREATE TABLE Department
(
  Name INT NOT NULL,
  Number INT NOT NULL,
  PRIMARY KEY (Name),
  UNIQUE (Number)
);

CREATE TABLE Project
(
  Location INT NOT NULL,
  Name INT NOT NULL,
  Number INT NOT NULL,
  PRIMARY KEY (Name),
  UNIQUE (Number)
);

CREATE TABLE Dependent
(
  Sex INT NOT NULL,
  Relationship INT NOT NULL,
  Birth_date INT NOT NULL,
  Name INT NOT NULL,
  PRIMARY KEY (Name)
);

CREATE TABLE Department_Locations
(
  Locations INT NOT NULL,
  Name INT NOT NULL,
  PRIMARY KEY (Locations, Name),
  FOREIGN KEY (Name) REFERENCES Department(Name)
);
```

## RESULT 
<div align="justify">
Thus the ER diagram was drawn and relational diagram, SQL DDL staements are generated using ERD plus tool.
</div>

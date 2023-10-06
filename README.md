# Ex. No: 4 Creating Procedures using PL/SQL

### AIM: To create a procedure using PL/SQL.

### Steps:
1. Create employee table with following attributes (empid NUMBER, empname VARCHAR(10), dept VARCHAR(15),salary NUMBER);
2. Create a procedure named as insert_employee data.
3. Inside the procdure block, write the query for inserting the values into the employee table.
4. End the procedure.
5. Call the insert_employee data procedure to insert the values into the employee table.
6. Display the employee table

### Program:
```
Developed by:GURUMOORTHI R
Register no:212222230042
```
```
SQL> create table employeee(empid number,empname varchar (20), dept varchar (15) ,salary number);

Table created.

SQL>  create or replace procedure insert_employeee_data AS
    BEGIN
     insert into employeee(empid,empname,dept,salary)
    values(1,'GURU','CEO',10000000);
   insert into employeee(empid,empname,dept,salary)
    values(2,'KAVIN','MD',700000);
     insert into employeee(empid,empname,dept,salary)
    values(3,'DHINAKARAN','TEAM LEADER',20000);
    COMMIT;
    end;
    /
Procedure created.

SQL> begin
  2  insert_employeee_data;
  3  end;
  4  /

PL/SQL procedure successfully completed.

SQL> select * from employeee;
```
### Output:

![1](https://github.com/gururamu08/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/118707009/e5da5f6c-0abf-4f29-a441-d2f3dff6ac7f)


### Result:
Hence the procedure using pl/sql is created successfully.

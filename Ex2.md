# EX 2 Data Manipulation Language (DML) Commands and built in functions in SQL

##DATE


## AIM:
To create a manager database and execute DML queries using SQL.


## DML(Data Manipulation Language)
<div align="justify">
The SQL commands that deal with the manipulation of data present in the database belong to DML or Data Manipulation Language and this includes most of the SQL statements. It is the component of the SQL statement that controls access to data and to the database. Basically, DCL statements are grouped with DML statements.
</div>

## List of DML commands: 
<div align="justify">
INSERT: It is used to insert data into a table.<br>
UPDATE: It is used to update existing data within a table.<br>
DELETE: It is used to delete records from a database table.<br>
</div>

## Create the table as given below:
```sql
create table manager(enumber number(6),ename char(15),salary number(5),commission number(4),annualsalary number(7),Hiredate date,designation char(10),deptno number(2),reporting char(10));
```

## insert the following values into the table
```sql
insert into manager values(7369,'Dharsan',2500,500,30000,'30-June-81','clerk',10,'John');
insert into manager values(7839,'Subu',3000,400,36000,'1-Jul-82','manager',null,'James');
insert into manager values(7934,'Aadhi',3500,300,42000,'1-May-82','manager',30,NULL);
insert into manager values(7788,'Vikash',4000,0,48000,'12-Aug-82','clerk',50,'Bond');
```

### Q1) Update all the records of manager table by increasing 10% of their salary as bonus.

### QUERY:
UPDATE MANAGER SET SALARY=(SALARY*0.10)+SALARY;




### OUTPUT:
![image](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/58390e90-5303-4068-8d67-7d105145cc17)



### Q2) Delete the records from manager table where the salary less than 2750.


### QUERY:
DELETE WORKER FRPM MANAGER WHERE SALARY<2750;


### OUTPUT:

![image](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/dfc6e8cd-1e60-4bee-bd43-305ea0a49525)


### Q3) Display each name of the employee as “Name” and annual salary as “Annual Salary” (Note: Salary in emp table is the monthly salary)


### QUERY
SELECT ENAME AS 'NAME' ,SALARY * 12 AS 'ANNUAL SALARY' FROM MANAGER;


### OUTPUT:
![image](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/b2018c86-8e35-4b1d-b23b-59956cc37fd6)



### Q5)	List the names of Clerks from emp table.


### QUERY:
SELECT ENAME FROM MANAGER WHERE DESIGNATION='CLERK';




### OUTPUT:
![output1 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/637983f2-abdd-44a6-a18d-01de15311b73)




### Q6)	List the names of employee who are not Managers.


### QUERY:
SELECT ENAME FROM MANAGER WHERE DESIGNATION != 'MANAGERS';


### OUTPUT:
![output2 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/ccbc6edb-afad-4f95-869e-e9d99a400655)



### Q7)	List the names of employees not eligible for commission.


### QUERY:

SELECT ENAME FROM MANAGER WHERE COMMISSION=0;


### OUTPUT:
![image](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/93e0ec4a-234a-4a1d-b001-054ac1ac6447)



### Q8)	List employees whose name either start or end with ‘s’.


### QUERY:
SELECT ENAME FROM MANAGER WHERE ENAME LIKE 'S%' OR ENAME LIKE '%S';



### OUTPUT:
![image](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/e929646d-0ee1-40e5-8e0d-08ad4af19dae)



### Q9) Sort emp table in ascending order by hire-date and list ename, job, deptno and hire-date.


### QUERY:
SELECT ENAME,DESIGNATION,DEPTNO,HIREDATE FROM MANAGER ORDER BY HIREDATE ASC;


### OUTPUT:
![output6 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/43fd9aee-1674-4687-9670-1db1f11d6300)



### Q10) List the Details of Employees who have joined before 30 Sept 81.


### QUERY:
SELECT * FROM MANAGER WHERE HIREDATE < '30 SEP 81';



### OUTPUT:


![output7 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/5e86bb75-c04c-4be3-91d9-2c5a73c24ef4)

### Q11)	List ename, deptno and sal after sorting emp table in ascending order by deptno and then descending order by sal.


### QUERY:

SELECT ENAME,DEPTNO,SALARY FROM MANAGER ORDER BY DEPTNO ASC,SALARY DESC;


### OUTPUT:

![output8 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/a375ec32-6d21-4e4c-9799-f9c5e5528352)


### Q12) List the names of employees not belonging to dept no 30,40 & 10


### QUERY:

SELECT COUNT(*) AS NUM_ROWS FROM MANAGER;


### OUTPUT:
![output9 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/9331af63-23a1-470a-af94-8b7114f134ed)


### Q13) Find number of rows in the table EMP

### QUERY:
SELECT COUNT(*) AS NUM_ROWS FROM MANAGER;



### OUTPUT:
![output10 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/cbb26618-b363-4a58-8e9a-73d8e8f0f914)



### Q14) Find maximum, minimum and average salary in EMP table.

### QUERY:
SELECT MAX(SALARY) AS MAX_SALARY,MIN(SALARY) AS MIN_SALARY,AVG(SALRY) AS 
AVG_SALARY FROM MANAGER;



### OUTPUT:
![image](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/f57cc209-773f-402d-bf5b-f50e71a95c10)


### Q15) List the jobs and number of employees in each job. The result should be in the descending order of the number of employees.
### QUERY:
SELECT DESIGNATION,COUNT(*) AS NUM_EMPLOYEES FROM MANAGER GROUP BY 
DESIGNATION ORDER BY NUM_EMPLOYEES DESC;

### OUTPUT:
![output12 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/82ca2da1-f114-4421-83bf-a4f71594d533)

Result:The Data Manipulation Language (DML) Commands and built in functions in SQL is executed sucessfully.

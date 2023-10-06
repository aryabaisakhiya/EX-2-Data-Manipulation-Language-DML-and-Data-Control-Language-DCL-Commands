# EX 2 Data Manipulation Language (DML) Commands and built in functions in SQL
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
![image](https://github.com/DhanushPalani/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121594640/b32bceb5-9f0f-4c30-b27f-c4375e677f46)



### OUTPUT:
![image](https://github.com/DhanushPalani/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121594640/3fd9b83b-a6e7-4e47-b0cb-f2815bbbae95)


### Q2) Delete the records from manager table where the salary less than 2750.


### QUERY:
![image](https://github.com/DhanushPalani/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121594640/15e1ebf0-899f-4589-aee8-0ea4570cefba)


### OUTPUT:
![image](https://github.com/DhanushPalani/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121594640/ad0c2970-47bc-4591-8f4b-a295a38b092d)


### Q3) Display each name of the employee as “Name” and annual salary as “Annual Salary” (Note: Salary in emp table is the monthly salary)


### QUERY:

![image](https://github.com/DhanushPalani/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121594640/72faf04a-7d00-4070-8b1b-433f67d05a51)


### OUTPUT:
![image](https://github.com/DhanushPalani/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/121594640/b697b096-ba16-4329-ac6b-d015128fd061)


### Q5)	List the names of Clerks from emp table.


### QUERY:
![querry1 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/a3c7394a-5279-4cd7-a919-3153671ae417)



### OUTPUT:
![output1 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/637983f2-abdd-44a6-a18d-01de15311b73)




### Q6)	List the names of employee who are not Managers.


### QUERY:
![querry2 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/3caa4c6c-ded5-4589-8354-2945ab52077c)


### OUTPUT:
![output2 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/ccbc6edb-afad-4f95-869e-e9d99a400655)



### Q7)	List the names of employees not eligible for commission.


### QUERY:
![querry3 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/efebec9f-5e90-4071-9789-beedbc5be141)



### OUTPUT:
![image](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/93e0ec4a-234a-4a1d-b001-054ac1ac6447)



### Q8)	List employees whose name either start or end with ‘s’.


### QUERY:
![image](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/8ecb4793-98de-45fd-bc2f-49fae56c0178)



### OUTPUT:
![image](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/e929646d-0ee1-40e5-8e0d-08ad4af19dae)



### Q9) Sort emp table in ascending order by hire-date and list ename, job, deptno and hire-date.


### QUERY:

![querry6 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/093599b2-25ad-4051-bfe9-0dd92b3d8f8f)


### OUTPUT:
![output6 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/43fd9aee-1674-4687-9670-1db1f11d6300)



### Q10) List the Details of Employees who have joined before 30 Sept 81.


### QUERY:
![querry7 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/ec5240e3-085e-4d38-b4d0-f74f16aea4fe)



### OUTPUT:


![output7 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/5e86bb75-c04c-4be3-91d9-2c5a73c24ef4)

### Q11)	List ename, deptno and sal after sorting emp table in ascending order by deptno and then descending order by sal.


### QUERY:

![output7 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/5e86bb75-c04c-4be3-91d9-2c5a73c24ef4)



### OUTPUT:

![output8 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/a375ec32-6d21-4e4c-9799-f9c5e5528352)


### Q12) List the names of employees not belonging to dept no 30,40 & 10


### QUERY:
![querry9 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/cb7cbe70-0435-4a73-96aa-0ebb6ce3aa89)



### OUTPUT:
![output9 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/9331af63-23a1-470a-af94-8b7114f134ed)


### Q13) Find number of rows in the table EMP

### QUERY:
![querry10 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/82ab1a25-cae3-4360-88b2-7770efb2ac04)



### OUTPUT:
![output10 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/cbb26618-b363-4a58-8e9a-73d8e8f0f914)



### Q14) Find maximum, minimum and average salary in EMP table.

### QUERY:
![querry11 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/ffdbe1e7-ec33-4e84-9bfd-dbdcacf60039)



### OUTPUT:
![image](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/f57cc209-773f-402d-bf5b-f50e71a95c10)



### Q15) List the jobs and number of employees in each job. The result should be in the descending order of the number of employees.

### QUERY:
![querry12 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/e171beba-29b0-41ee-840c-86c42a88d9c2)



### OUTPUT:
![output12 ex2](https://github.com/aryabaisakhiya/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/119393645/82ca2da1-f114-4421-83bf-a4f71594d533)


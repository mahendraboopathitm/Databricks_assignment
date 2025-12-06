# Databricks_assignment

Databricks Assignment 

## Question 1:  

## Create 3 folders as source_to_bronze, bronze_to_silver, silver_to_gold. 

<img width="1912" height="828" alt="image" src="https://github.com/user-attachments/assets/a2eff85d-369c-48b4-823d-b22901943808" />

## Create 4 notebooks in this respective order.  
## 2 Notebooks named in source_to_bronze as utils (add all common functions in this notebook) and employee_source_to_bronze (driver notebook)  

<img width="1230" height="711" alt="image" src="https://github.com/user-attachments/assets/0c19208d-4ef6-42e5-bfd6-22af8b3a0520" />
 <img width="1912" height="798" alt="image" src="https://github.com/user-attachments/assets/12c94fae-8451-4db7-b694-bfa408a25d37" />

## 1 Notebook in bronze to silver as employee_bronze_to_silver   

<img width="1919" height="795" alt="image" src="https://github.com/user-attachments/assets/90667552-2e9c-491c-9cd2-a9122aa19db7" />



## 1 Notebook in silver to gold as employee_silver_to_gold  

<img width="1919" height="809" alt="image" src="https://github.com/user-attachments/assets/a9ad025f-4369-4d65-9193-d89f94db623f" />


## Read the 3 datasets as Dataframe in employee_source_to_bronze, call utils notebook in this notebook, and write to a location in DBFS, as /source_to_bronze/file_name.csv (employee, department_df, country_df) as CSV format 

<img width="1910" height="843" alt="image" src="https://github.com/user-attachments/assets/7e1486af-59e7-4756-8cac-217eb334a600" />
<img width="1860" height="855" alt="image" src="https://github.com/user-attachments/assets/c32d6502-2ca9-43aa-aa8b-02a96d737ff0" />

<img width="1908" height="790" alt="image" src="https://github.com/user-attachments/assets/22482987-db56-46ee-8740-790fb88b4963" />

## In employee_bronze_to_silver, call utils notebook in this notebook.   
## Read the file located in DBFS location source_to_bronze with as data frame different read methods using custom schema.  
<img width="1866" height="848" alt="image" src="https://github.com/user-attachments/assets/674f9865-d89f-4095-aca2-7be848761826" />
<img width="1855" height="845" alt="image" src="https://github.com/user-attachments/assets/89f7c7a9-1804-4c11-9e34-313c28865991" />
<img width="1841" height="843" alt="image" src="https://github.com/user-attachments/assets/256667ed-83e7-48c0-bfdf-20d497cd3f6f" />



## 5.convert the Camel case of the columns to the snake case using UDF.  

<img width="1841" height="834" alt="image" src="https://github.com/user-attachments/assets/1d5de29d-f539-40d8-85d7-7023a80e116a" />


## Add the load_date column with the current date.  
<img width="1841" height="834" alt="image" src="https://github.com/user-attachments/assets/1d5de29d-f539-40d8-85d7-7023a80e116a" />

## The primary key is EmployeeID, the Database name is Employee_info, Table name is dim_employee.  

<img width="1834" height="829" alt="image" src="https://github.com/user-attachments/assets/559f1085-18f2-43a5-80ff-2d4a59a270c6" />

## write the DF as a delta table to the location /silver/db_name/table_name.  

<img width="1844" height="788" alt="image" src="https://github.com/user-attachments/assets/6f126fc4-eee9-45db-9215-b905a3162885" />


## 7.In gold notebook employee_silver_to_gold, call utils notebook in this notebook  
<img width="1912" height="806" alt="image" src="https://github.com/user-attachments/assets/e6defbca-89b8-469f-83ed-c192f8abbe98" />

## Read the table stored in a silver layer as DataFrame and select the columns based on the following requirements A screenshot of a computer
<img width="1912" height="806" alt="image" src="https://github.com/user-attachments/assets/f6afea4e-3b47-43c8-a6ad-c5827390fcef" />
<img width="1862" height="798" alt="image" src="https://github.com/user-attachments/assets/9ab0802b-02d9-4352-b250-c1b26130b56a" />


## Find the salary of each department in descending order.  
<img width="1862" height="533" alt="image" src="https://github.com/user-attachments/assets/65106ead-c6d6-4ec3-9b40-d232de2f0553" />
<img width="1432" height="377" alt="image" src="https://github.com/user-attachments/assets/4f9911ba-2419-4084-9432-08a44c08db93" />

## Find the number of employees in each department located in each country.  
<img width="1873" height="541" alt="image" src="https://github.com/user-attachments/assets/50d3ddd6-8c99-4ca7-b259-cb0b3cf6ff25" />
<img width="1569" height="659" alt="image" src="https://github.com/user-attachments/assets/e237b7f9-41d1-4ef5-adbf-0955965f65c3" />

## List the department names along with their corresponding country names.  
<img width="1874" height="696" alt="image" src="https://github.com/user-attachments/assets/198f055e-3177-42bd-a00b-e2f30556a37c" />
<img width="1572" height="471" alt="image" src="https://github.com/user-attachments/assets/83d1a80c-7f3e-4fc4-86ff-fad953caa8b0" />

## What is the average age of employees in each department?  
<img width="1860" height="564" alt="image" src="https://github.com/user-attachments/assets/b10266c8-9f78-4774-a56f-fceed46f35c0" />
<img width="1839" height="738" alt="image" src="https://github.com/user-attachments/assets/22ebfcbb-3e1c-4a59-9fff-f9629acb05b0" />

## Add the at_load_date column to data frames.  
## OutPut: 
<img width="1844" height="815" alt="image" src="https://github.com/user-attachments/assets/2589b769-701e-46a5-9c48-c54c3710dbae" />


## Write the df to dbfs location /gold/employee/table_name(fact_employee) with overwrite and replace where condition on at_load_date.  

 <img width="1849" height="823" alt="image" src="https://github.com/user-attachments/assets/92f43b4f-539e-4dd8-920d-a39fb3e42611" />


 

Question 2:  

Api: https://reqres.in/api/users?page=2  
drop "page”, "per_page", "total", "total_pages" and complete block of support.  

Fetch the data from the given API by passing the parameter as a page and retrieving the data till the data is empty 

 

 

 

Read the data frame with a custom schema : 

 

 

Flatten the dataframe : 

 

Derive a new column from email as site_address with values(reqres.in) : 

 

Add load_date with the current date : 

 

Write the data frame to location in DBFS as /db_name /table_name with   

Db_name as site_info and table_name as person_info with delta format and overwrite mode.  

 


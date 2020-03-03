# Using Impala
- 44517-01
- 04-Using Impala

## Team Members
- Chitralekha Chikku -s534630@nwmissouri.edu
- Manasa Goriparthi - s534782@nwmissouri.edu
- Bhavani Pathuri - s534867@nwmissouri.edu
- Nithya Vudayamarri - s534641@nwmissouri.edu

## Link to our repository
- https://github.com/manasagoriparthi/workshop-impala

## Instructions
- Before getting started make sure you have all the setup ready i.e installed Oracle virtual box and downloaded Cloudera quickstart CDH   in your machines.

- Similar to Hadoop and its ecosystem software, we need to install Impala on Linux operating system. Since cloudera shipped Impala, it     is available with Cloudera Quick Start VM.

- To start Impala, open the terminal and execute this command - 'impala-shell' 
### Below are some general purpose commands:
- To check the current version of impala execute this command - [quickstart.cloudera:21000] > version;
- To check the list of commands available in impala execute this command - [quickstart.cloudera:21000] > help;
- To quit from the impala shell execute this command - [quickstart.cloudera:21000] > exit; 
- The command to connect to the given instance of impala - [quickstart.cloudera:21000] > connect; 

- Below link can be used as the refernce for the setup: 

   https://www.tutorialspoint.com/impala/impala_shell.htm
   
## Working with Impala
- Use the following commands within impala-shell to pass requests to the impalad daemon that the shell is connected to. You can enter a   command interactively at the prompt, or pass it as the argument to the -q option of impala-shell. Most of these commands are passed to   the Impala daemon as SQL statements.

- Command to Create a Database:
  CREATE DATABASE IF NOT EXISTS database_name;
  
- Command to verify
  SHOW DATABASES;
  
- Command to use a Database:
  USE database_name;
  
- Command to Drop a Database:
  DROP DATABASE IF EXISTS database_name;
  
- Command to Create a Table:
  create table IF NOT EXISTS database_name.table_name (
   column1 data_type,
   column2 data_type,
   column3 data_type,
   ………
   columnN data_type
);

- Command to insert values in Table:
  insert into table_name (column1, column2, column3,...columnN)
  values (value1, value2, value3,...valueN);
- Command to drop a Table:
  DROP table database_name.table_name;
  
- Command to describe a Table:
  Describe table_name;
  
- In order to create a database in HDFS file system, you need to specify the location where the database is to be created as shown         below.
  CREATE DATABASE IF NOT EXISTS database_name LOCATION hdfs_path;
  





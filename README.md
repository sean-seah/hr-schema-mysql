# hr-schema-mysql
DML and DDL scripts to generate the HR SQL Schema for MySQL

Check also https://github.com/nomemory/neat-sample-databases-generators for scripts to generate data for various schemas. Data is arbitrary generated.

After download the file, import it using the command, 
CREATE DATABASE hr; //create an empty database named hr
cd download // to enter the folder "download" where the hr-schema-mysql file located.
mysql -u root -p hr < hr-schema-mysql.sql //import the downloaded file"hr-schema.mysql.sql" into empty database "hr" which previously was create in MySQL using command, "CREATE Database hr;"

# Local Server Installation
MySQL DB Local Server
Guidelines

Note: Pre-requisite: To install vscode https://code.visualstudio.com/

1. download https://dev.mysql.com/downloads/mysql/ and  https://dev.mysql.com/downloads/workbench/
2. choose "Windows (x86, 64-bit), MSI Installer" or the first option in the list
3. suggestion for students: register oracle account using utm's email (university's email)
3. during setup, can choose "typical" 
4. during configuration, can choose default
5. During MySQL Configurator

Accounts and Roles
Root Account Password
---------------------
MySQL Root Password: admin123
(Note: operate as root, so no need to add user)

6. During Window Service, UNTICK start the MySQL server at system startup
7. During Sample Databases, tick both Sakila and World
8. During Configuration Complete, "Copy Log to Clipboard"
9. Manual: https://dev.mysql.com/doc/refman/9.1/en/entering-queries.html
10. Open Terminal or Command Prompt
11. type "mysql -u root -p"
12. type "path" to check exist path
13. look for where is MySQL bin //edit the system environment variables>advanced>environment variables>add the copied URL into path through'edit' and paste it with "
set path=%PATH%;C:\Program Files\MySQL\MySQL Server 9.1\bin" 

15. try again, type "mysql -u root -p"
16. then come out the message to enter password
17. start the first command: type "show databases;"
18. choose to use the sakila database: type “use sakila;” 
19. display tables: type “show tables;”
20. display table with attributes: type “describe store;”
21. note: MUL meant multiple keys (reference: https://stackoverflow.com/questions/5317889/sql-keys-mul-vs-pri-vs-uni)
22. For project SQL commands submission that is based on created script (*.sql): The mysqldump client utility performs logical backups, producing a set of SQL statements that can be executed to reproduce the original database object
Example using mysqldump for employees.sql, the content how it looks like as below: (https://github.com/datacharmer/test_db/blob/master/employees.sql)
mysqldump -u [username] -p [database_name] > [output_file].sql

23. Example To import the data into your MySQL instance, load the data through the mysql command-line tool: type “mysql -t < employees.sql”

24. exit from MySQL: type "exit"
Visual Studio Code - Code Editing. Redefined
Visual Studio Code redefines AI-powered coding with GitHub Copilot for building and debugging modern web and cloud applications. Visual Studio Code is free and available on your favorite platform -...
 

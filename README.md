# hr-schema-mysql
DML and DDL scripts to generate the HR SQL Schema for MySQL

Check also https://github.com/nomemory/neat-sample-databases-generators for scripts to generate data for various schemas. Data is arbitrary generated.

After download the file, import it using the command, 
CREATE DATABASE hr; //create an empty database named hr
cd download // to enter the folder "download" where the hr-schema-mysql file located.
mysql -u root -p hr < hr-schema-mysql.sql //import the downloaded file"hr-schema.mysql.sql" into empty database "hr" which previously was create in MySQL using command, "CREATE Database hr;"


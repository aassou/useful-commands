# Import a SQL file using the command line in MySQL

mysql -u username -p database_name < file.sql

# Disable ONLY_FULL_GROUP_BY

mysql > SET GLOBAL sql_mode=(SELECT REPLACE(@@sql_mode,'ONLY_FULL_GROUP_BY',''));

# 1. Import a SQL file using the command line in MySQL

mysql -u username -p database_name < file.sql

# 2. Export database using the command line

mysqldump -u username -p database_name > file.sql

# 3. Disable ONLY_FULL_GROUP_BY

mysql > SET GLOBAL sql_mode=(SELECT REPLACE(@@sql_mode,'ONLY_FULL_GROUP_BY',''));

# 4. Allow remote access to MySQL:
sudo nano /etc/mysql/mysql.conf.d/mysqld.cnf

-- Change this line from 127.0.0.1 to 0.0.0.0
bind-address = 127.0.0.1

# 5. Reset AutoIncrement
ALTER TABLE table_name AUTO_INCREMENT = 1;

# 6. Get size of MySQL database
SELECT 
    table_schema "table_name", 
    ROUND(SUM(data_length + index_length) / 1024 / 1024, 1) "DB Size in MB" 
FROM information_schema.tables 
GROUP BY table_schema; 


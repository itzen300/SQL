# SQL
Practical utilization for the concepts of Database Management System DBMS.
Learning practically the RDBMS (Relational DataBase Management System) via the application of MySQL both on the Workbench and 'cmd'. Since I do already have past experience in Linux Operating System so making caparitive and conceptual learning mutually.

--------------------------------------------------------------------------------------------------------------------------------------------
| **Function**               | **MySQL Command**                                 | **Linux Command (approximate)**                         |
| -------------------------- | ------------------------------------------------- | ------------------------------------------------------- |
| Check MySQL version        | `mysql --version` or `mysql -V`                   | `mysql --version` or `mysql -V`                         |
| Start MySQL shell          | `mysql -u root -p`                                | `mysql -u root -p` (same; just works in Linux terminal) |
| Exit MySQL shell           | `exit;` or `quit;`                                | `exit` (to leave shell)                                 |
| Show databases             | `SHOW DATABASES;`                                 | `ls /var/lib/mysql` (list database folders)             |
| Create a database          | `CREATE DATABASE dbname;`                         | `mkdir /var/lib/mysql/dbname` (roughly)                 |
| Use/select a database      | `USE dbname;`                                     | `cd /var/lib/mysql/dbname` (move into DB folder)        |
| Show tables in database    | `SHOW TABLES;`                                    | `ls` (list files in DB folder)                          |
| Show table structure       | `DESCRIBE tablename;`                             | `cat tablename.frm` (view raw, not human-readable)      |
| Create a table             | `CREATE TABLE tablename (...);`                   | (no direct Linux equivalent; DB action)                 |
| Insert data into table     | `INSERT INTO tablename (...) VALUES (...);`       | (no Linux equivalent)                                   |
| View table data            | `SELECT * FROM tablename;`                        | (no Linux equivalent)                                   |
| Delete a table             | `DROP TABLE tablename;`                           | `rm tablename.frm` (dangerous, not advised)             |
| Delete a database          | `DROP DATABASE dbname;`                           | `rm -r /var/lib/mysql/dbname` (dangerous, not advised)  |
| Create a new user          | `CREATE USER 'user'@'host' IDENTIFIED BY 'pass';` | `adduser username`                                      |
| Grant permissions to user  | `GRANT ALL PRIVILEGES ON db.* TO 'user'@'host';`  | `chmod` or `chown` (file permissions)                   |
| View current user          | `SELECT USER();`                                  | `whoami`                                                |
| View current database      | `SELECT DATABASE();`                              | `pwd` (show current folder)                             |
| Import SQL dump            | `mysql -u root -p dbname < dumpfile.sql`          | (file redirection)                                      |
| Export SQL dump            | `mysqldump -u root -p dbname > dumpfile.sql`      | (file redirection)                                      |
| Check MySQL service status | *(inside MySQL: no direct)*                       | `systemctl status mysql` or `service mysql status`      |
| Start/stop MySQL service   | *(inside MySQL: no direct)*                       | `sudo systemctl start mysql` / `stop mysql`    
| File Nature                |                                                   | file
--------------------------------------------------------------------------------------------------------------------------------------------

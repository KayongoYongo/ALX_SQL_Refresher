# ALX_SQL_Refresher
Just a refresher on SQL

## Getting Started with MySQL
# Install MySQL 8.0 on Ubuntu 20.04 LTS

``` shell
$ sudo apt update
$ sudo apt install mysql-server
...
$ mysql --version
mysql  Ver 8.0.25-0ubuntu0.20.04.1 for Linux on x86_64 ((Ubuntu))
$
```

# Start MySQL
``` shell
$ service mysql start 
```

## Tasks
# 0. List databases
**Write a script that lists all databases of your MySQL server.**
``` shell
vagrant@ubuntu-focal:~/ALX_SQL_Refresher$ cat 0-list_databases.sql | mysql -hlocalhost -uroot -p
Enter password:
Database
hbtn_0c_0
information_schema
mysql
performance_schema
sys
```

# 1. Create a database
**Write a script that creates the database hbtn_0c_0 in your MySQL server.**
* If the database hbtn_0c_0 already exists, your script should not fail
* You are not allowed to use the SELECT or SHOW statements
``` shell
vagrant@ubuntu-focal:~/ALX_SQL_Refresher$ cat 1-create_database_if_missing.sql | mysql -hlocalhost -uroot -p
Enter password: 
vagrant@ubuntu-focal:~/ALX_SQL_Refresher$ cat 0-list_databases.sql | mysql -hlocalhost -uroot -p
Ener password: 
Database
information_schema
hbtn_0c_0
mysql
performance_schema
```

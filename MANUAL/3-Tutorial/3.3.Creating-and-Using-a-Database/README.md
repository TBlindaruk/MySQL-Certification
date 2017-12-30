### 3.3 Creating and Using a Database

https://dev.mysql.com/doc/refman/5.6/en/database-use.html

<string>Use the SHOW statement to find out what databases currently exist on the server:</string>

```SQL
SHOW DATABASES;
```

| Database |
| -------- |
| information_schema |
| certification |
| homestead |
| mysql |
| mysql_manual |
| performance_schema |
| sys |
| your_internet |

--------------------------------

<strong>USE [database_name]</strong> - for change db. For example:

```SQL
USE test
```

`Database changed`

--------------------

<strong>Set permission to the database</strong>

```SQL
GRANT ALL ON menagerie.* TO 'your_mysql_name'@'your_client_host';
```
where your_mysql_name is the MySQL user name assigned to you and your_client_host is the host from which you connect to the server.
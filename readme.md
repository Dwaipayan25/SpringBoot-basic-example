1. # Some Docker Commands to connect Postgres here
2. ```docker compose up -d``` To run the docker-compose.yml file
2. ``` docker ps``` TO see details of the container
3. ``` docker exec -it postgres bash```
4.
```docker exec -it postgres bash```
```root@a9a8418a9208:/# psql -h localhost -U dwaipayan```
psql (16.3 (Debian 16.3-1.pgdg120+1))
Type "help" for help.

```dwaipayan=#  \c employeemanager```
You are now connected to database "employeemanager" as user "dwaipayan".
employeemanager=# SELECT * FROM employee;



```employeemanager=# SELECT * FROM employee;```

```dtd

dwaipayan=# \l
                                                        List of databases
   Name    |   Owner   | Encoding | Locale Provider |  Collate   |   Ctype    | ICU Locale | ICU Rules |    Access privileges    
-----------+-----------+----------+-----------------+------------+------------+------------+-----------+-------------------------
 dwaipayan | dwaipayan | UTF8     | libc            | en_US.utf8 | en_US.utf8 |            |           | 
 postgres  | dwaipayan | UTF8     | libc            | en_US.utf8 | en_US.utf8 |            |           | 
 template0 | dwaipayan | UTF8     | libc            | en_US.utf8 | en_US.utf8 |            |           | =c/dwaipayan           +
           |           |          |                 |            |            |            |           | dwaipayan=CTc/dwaipayan
 template1 | dwaipayan | UTF8     | libc            | en_US.utf8 | en_US.utf8 |            |           | =c/dwaipayan           +
           |           |          |                 |            |            |            |           | dwaipayan=CTc/dwaipayan
        (4 rows)

        dwaipayan=# CREATE DATABASE customer;
        CREATE DATABASE
        dwaipayan=# \l
        List of databases
        Name    |   Owner   | Encoding | Locale Provider |  Collate   |   Ctype    | ICU Locale | ICU Rules |    Access privileges
        -----------+-----------+----------+-----------------+------------+------------+------------+-----------+-------------------------
        customer  | dwaipayan | UTF8     | libc            | en_US.utf8 | en_US.utf8 |            |           |
        dwaipayan | dwaipayan | UTF8     | libc            | en_US.utf8 | en_US.utf8 |            |           |
        postgres  | dwaipayan | UTF8     | libc            | en_US.utf8 | en_US.utf8 |            |           |
        template0 | dwaipayan | UTF8     | libc            | en_US.utf8 | en_US.utf8 |            |           | =c/dwaipayan           +
        |           |          |                 |            |            |            |           | dwaipayan=CTc/dwaipayan
        template1 | dwaipayan | UTF8     | libc            | en_US.utf8 | en_US.utf8 |            |           | =c/dwaipayan           +
        |           |          |                 |            |            |            |           | dwaipayan=CTc/dwaipayan
        (5 rows)



```

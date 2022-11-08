# SQLite

Ejercicio Semanal - SQLite
update
update users set firstname="laura" where iduser=1;

![Image text](https://github.com/varrietasotelo/SQLite/blob/main/img/1.jpg) 

estructura de la base de datos .schema
.schema users

![Image text](https://github.com/varrietasotelo/SQLite/blob/main/img/2.jpg) 

date and time functions
now- select date('now');

![Image text](https://github.com/varrietasotelo/SQLite/blob/main/img/3.jpg) 

datetime - select datetime(‘no’);

![Image text](https://github.com/varrietasotelo/SQLite/blob/main/img/4.jpg) 

![Image text](https://github.com/varrietasotelo/SQLite/blob/main/img/5.jpg) 

primary key constraint
Al crear la tabla:

![Image text](https://github.com/varrietasotelo/SQLite/blob/main/img/6.jpg) 

Después de creada la tabla:

![Image text](https://github.com/varrietasotelo/SQLite/blob/main/img/7.jpg) 

![Image text](https://github.com/varrietasotelo/SQLite/blob/main/img/8.jpg) 

![Image text](https://github.com/varrietasotelo/SQLite/blob/main/img/9.jpg) 

not null constraint

![Image text](https://github.com/varrietasotelo/SQLite/blob/main/img/10.jpg) 

unique constraint
CREATE TABLE users(iduser int primary key unique, firstname text, lastname text, email text, age int check (age>=18));

![Image text](https://github.com/varrietasotelo/SQLite/blob/main/img/11.jpg) 

default constraint
create table employees (idemp int primary key, firstname text, lastname int, email text, city text default 'Bogota');

![Image text](https://github.com/varrietasotelo/SQLite/blob/main/img/12.jpg) 

check constraint
CREATE TABLE users(iduser int primary key unique, firstname text, lastname text, email text, age int check (age>=18));

![Image text](https://github.com/varrietasotelo/SQLite/blob/main/img/13.jpg) 

alter table
alter table employees rename to employees_old;

![Image text](https://github.com/varrietasotelo/SQLite/blob/main/img/14.jpg) 

delete, drop
drop table old_users;

![Image text](https://github.com/varrietasotelo/SQLite/blob/main/img/15.jpg) 


Drop Primary Key
pragma foreign_key=off;
alter table employees rename to employees_old;
create table employees (idemp int, firstname text, lastname int, email text, city text default 'Bogota');
insert into employees select * from employees_old;
commit;
pragma foreign_keys=on;

![Image text](https://github.com/varrietasotelo/SQLite/blob/main/img/16.jpg) 


backup, restore
sqlite3 chinook.db .dump > backup.sql

![Image text](https://github.com/varrietasotelo/SQLite/blob/main/img/17.jpg) 


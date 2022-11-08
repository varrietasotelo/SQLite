# SQLite

Atento saludo.
Ejercicio Semanal - SQLite
update
update users set firstname="laura" where iduser=1;
![Image text](https://github.com/varrietasotelo/patrones/blob/main/Imagenes/Instancia_Singleton.PNG) 

estructura de la base de datos .schema
.schema users
![Image text](https://github.com/varrietasotelo/patrones/blob/main/Imagenes/Instancia_Singleton.PNG) 

date and time functions
now- select date('now');
![Image text](https://github.com/varrietasotelo/patrones/blob/main/Imagenes/Instancia_Singleton.PNG) 

datetime - select datetime(‘no’);
![Image text](https://github.com/varrietasotelo/patrones/blob/main/Imagenes/Instancia_Singleton.PNG) 

![Image text](https://github.com/varrietasotelo/patrones/blob/main/Imagenes/Instancia_Singleton.PNG) 

primary key constraint
Al crear la tabla:
![Image text](https://github.com/varrietasotelo/patrones/blob/main/Imagenes/Instancia_Singleton.PNG) 

Después de creada la tabla:
![Image text](https://github.com/varrietasotelo/patrones/blob/main/Imagenes/Instancia_Singleton.PNG) 
![Image text](https://github.com/varrietasotelo/patrones/blob/main/Imagenes/Instancia_Singleton.PNG) 
![Image text](https://github.com/varrietasotelo/patrones/blob/main/Imagenes/Instancia_Singleton.PNG) 

not null constraint
![Image text](https://github.com/varrietasotelo/patrones/blob/main/Imagenes/Instancia_Singleton.PNG) 

unique constraint
CREATE TABLE users(iduser int primary key unique, firstname text, lastname text, email text, age int check (age>=18));
![Image text](https://github.com/varrietasotelo/patrones/blob/main/Imagenes/Instancia_Singleton.PNG) 

default constraint
create table employees (idemp int primary key, firstname text, lastname int, email text, city text default 'Bogota');
![Image text](https://github.com/varrietasotelo/patrones/blob/main/Imagenes/Instancia_Singleton.PNG) 

check constraint
CREATE TABLE users(iduser int primary key unique, firstname text, lastname text, email text, age int check (age>=18));
![Image text](https://github.com/varrietasotelo/patrones/blob/main/Imagenes/Instancia_Singleton.PNG) 

alter table
alter table employees rename to employees_old;
![Image text](https://github.com/varrietasotelo/patrones/blob/main/Imagenes/Instancia_Singleton.PNG) 

delete, drop
drop table old_users;
![Image text](https://github.com/varrietasotelo/patrones/blob/main/Imagenes/Instancia_Singleton.PNG) 


Drop Primary Key
pragma foreign_key=off;
alter table employees rename to employees_old;
create table employees (idemp int, firstname text, lastname int, email text, city text default 'Bogota');
insert into employees select * from employees_old;
commit;
pragma foreign_keys=on;
(https://github.com/varrietasotelo/patrones/blob/main/Imagenes/Instancia_Singleton.PNG) 






backup, restore
sqlite3 chinook.db .dump > backup.sql
(https://github.com/varrietasotelo/patrones/blob/main/Imagenes/Instancia_Singleton.PNG) 


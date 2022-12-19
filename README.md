# flasktut
this is first flask tutorial 
**python-flask-cmd-run-model and  check and create database use this code ,**


1>>> from market import db, app  // import model
2>>> app.app_context().push() // create object of app 
3>>> db.create_all() 

for item in Item.query.all(): // use for the data retrive 
...     item.id
...     item.name
...     item.price
...     item.barcode
...     item.descripation

(retrive from your database)

for item in Item.query.filter_by(price=500):
...     item.name
(retrive data from filtering)


keep one thing powershell use for your code is proper execute or not.
-----------------------------------------------------------------------------

So, these are the commands that you are going to be needing to work with Postgres:
1. Create a new user
create user 'username' with password 'password';
2. Assign roles and attributes to user
alter user 'username' with superuser;
alter user 'username' with createdb;
3. Switch user
\c 'database name' 'username'
4. Create database with new user
create database 'database name';
5. \du - display all users
6. \l - list all tables in a database
7. \q - quit psql shell.
8. \d  show to list of table in database
9. \d [table n
10. ame ] - show the filds of the table
11. query run  :select * from public."user_details"; 

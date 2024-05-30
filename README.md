## Library management using Python & MySQL
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

```
Dev/Editor: Kanika Vishwakarma , Abhinav, Kopal Vishwakarma
```
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

>Introduction:

Welcome to this intermediate project where we create a user-friendly library management system. This system allows you to:
- Add books with details
- Delete books
- View listed books
- Issue books to students or anyone
- Return books

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

>Dependencies:

- tkinter
- pillow
- pymysql
- cryptography
- MySQL should be installed

Commands to download dependencies:
```
pip install tk
pip install pillow
pip install pymysql
pip install cryptography
```
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

>_Note: You can directly install all the packages from the requirement.txt (included in the project). Make sure you are in the same directory as the requirements.txt. Just run -_ 

```
pip install -r requirements.txt
```

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

>❗ IMPORTANT STEP ❗

- We recommend to use the password as ```root``` or you can simply change the password in the scripts.
- Open MySQL Command Line Client (search using the Windows key if you're on Windows).
- Enter the password (root).
- Run the following commands to set up your database:

```
show databases;
```

```
create database db;
```

```
use db;
```

```
create table books(bid varchar(20) primary key, title varchar(30), author varchar(30), status varchar(30));
```

```
create table books_issued(bid varchar(20) primary key, issuedto varchar(30));
```

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 >How to start working with the project:

```  
To run the code, execute main.py : python main.py
```

- When you run main.py, the UI will pop up.

- Add a book by filling in the information (case sensitive). To verify, go to the MySQL CLI and run:

```
select * from books;. This will display the books added to the database.
```

- To verify deletion of a book, use the same code.

- When you issue a book, check who it is issued to by running: 
```
select * from books_issued;
```

- After issuing a book, check the status update by running: 

```
select * from books;
```

- The status should change from "Available" to "Issued".

_If you've followed all the steps correctly, congratulations on successfully setting up your library management system!_

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------       

Instagram : _elegant_kannu

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

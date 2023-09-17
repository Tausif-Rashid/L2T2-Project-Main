-L2T2-Project-Group13

# Grades Information System
![Model](https://github.com/Tausif-Rashid/L2T2-Project-Main/blob/main/Screenshot%202023-09-17%20082120.png)

## Overview

GRADES INFORMATION SYSTEM
A system similar to BIIS , for storing, viewing and updating student information and specially students' grades. View individual, level-wise, course-wise results. Also students can view and enrolled courses , advisors can manage course enrollment. Admin panel for viewing, adding or removing courses, students, notices, exam routines. 

## ERD
![Model](https://github.com/Tausif-Rashid/L2T2-Project-Main/blob/main/Screenshot%202023-09-17%20082945.png)

## Stack
Backend: Nodejs, ExpressJS <br/>
Frontend: HTML, CSS EJS

## Fetaures

---Student login:
1) View and Edit information like name, address, etc
2) View courses : taken, available, completed
-> Enroll new courses if prerequisites completed
3) View faculty info table, Advisor info
4) View Grades :
	-> Term-wise like BIIS
	-> Course-wise - TF, CT, Attendance

---Teacher Login:
1) View grades:
	->Section wise
	->Dept wise
 -> Course wise
2) View and change information
3) View courses taking currently 
4) View pending results

---Admin Login
1) View all students
2) View all teachers
3) View all courses
4) Add/Remove student , teachers , courses
5) View info update requests and approve(later)
6) Keep log of every changes to database and view logs<br/>

## Installation

### Prerequisites---
Oracle 19c, with SQL PLUS, DBeaver/Navicat, NodeJS, VSCode, Any browser. 

schema creation: 
Run these commands in SQL PLus:
1. SQL Plus login: ```sys as sysdba``` pass: ```1234```
2. ```show pdbs```
3. ```alter pluggable database orclpdb open;```
4. ```alter session set container=ORCLPDB;```
5. ```create user ProjectDBa identified by 12345;```
6. ```grant all privileges to ProjectDBa;```
7. ```alter user ProjectDBa quota unlimited on users;```

Connect schema with DBeaver/Navicat:
Navicat:
8. Connection type: Service name
a. Service name: orclpdb (if step 2 shows no error, and you run the command
from step 3)
b. Service name: orcl (if step 2 shows any errors and you skip step 3)
9. username: ```ProjectDBa```
10. password: ```12345```
DBeaver:
Database: ```ORCLPDB```
Username: ```ProjectDBa```
Password: ```12345```

Run SQL commands inside folder according to readme.txt.

---Running Project---

In VScode, open project folder, navigate to project folder in terminal.
run 
```npm start```
terminal should show
```server started at port 5000```
Go to 
```localhost:5000``` in your browser.
The login page should be visible.

---for checking---

Student Credentials:
id: ```S100001``` to ```S102000```
pw: ```password1001``` to ```password3000``` respectively

Teacher Credentials:
id: ```T1001``` to ```T1500```
pw: ```pwd100``` to ```pwd600```

Admin Credentials:
id: ```A10``` to ```A14```
pw: ```pwd12345_1``` to ```pwd12345_5```

Advisor-student pair
S100349
123

T1324
pwd423


## Project Team
Sajid: https://github.com/SajidNoor5051

Tausif: https://github.com/Tausif-Rashid



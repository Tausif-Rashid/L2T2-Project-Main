# L2T2-Project-Main
-L2T2-Project-Group13

---Overview---

GRADES INFORMATION SYSTEM
A system similar to BIIS , for storing, viewing and updating student information and specially students' grades. View individual, level-wise, course-wise results. Also students can view and enrolled courses , advisors can manage course enrollment. Admin panel for viewing, adding or removing courses, students, notices, exam routines. 


---Prerequisites---

Oracle 19c, with SQL PLUS, DBeaver/Navicat, NodeJS, VSCode, Any browser. 


---Installation---

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

Run SQLV3/Createtable.sql file inside dbeaver/navicat.
Run SQLV3/InsertData sql commands serially.
Run SQLV3/Functions file serially.

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


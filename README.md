Ryan Mastin - 101229946

Steven Wu - 101219383

3005 Final Project v2 - Group 169

https://youtu.be/7nverSZSl1Y

If you are looking for the SQL statements in our code, search through one of the GUI files with cntrl f searching for SQL.

All SQL functions will call SQL. in order to contact the database. 

**9 Files -> AdminGUI, InitalizeGUI, main.py, MemberBackend.py, MemberGUI, SQL.py, TrainerBackend.py, TrainerGUI.py, Utility.py**

**Installs:**

pip install psycopg2

Tkinter is installed alongside Python in the majority of releases. If it is not present, re-install python to the latest version. If that doesn't work (pip install tk) *may* work

**Operation:**

Ensure databased has been created and populated before operation (Check SQL folder in repo for DDL and DML files) and enter that in the pgAdmin query tool [after creating the db]

Install pyscopg2 using the pip command above (In the folder with the file, do pip install pyscopgy2). Tkinter SHOULD already be installed with modern python packages

If any info differs in your postgres database you must change it in the variables in the top of the SQL script

(Current Database Setup [Change to match your setup]): host = localhost, dbname (database name) = FinalProject, user = postgres, password = postgres

Navigate to the folder where you placed my file, and run using Python. e.g (In folder with the file [in cmd]) -> python main.py.

Click the user type you'd like to login as. Steven Wu is an already populated member, Alice Smith is an already populated Trainer, ADMIN gets you to the admin console, or create your own using member registration :D


**File Directory**
1. main.py - how u run the program. Calls Initialize GUI and Member/Trainer/Admin GUI
2. Initialize.py - Creates the Login screen and passes the input back to main
3. AdminGUI.py - Hosts all of the admin database functions and GUI
4. MemberGUI.py - Hosts all of the member database functions and GUI
    4a. MemberBackend - contains function to find available trainers on given date and time interval
5. SQL.py - Hosts the SQL psycopg2 statements for selecting, inserting, updating...etc
6. \SQL\ Final Project DDL.sql - Hosts the DDL File for database Creation
7. \SQL\ Final Project DML.sql - Hosts the DML File for database Inserts
8. TrainerGUI.py - Hosts the trainer GUI
9. TrainerBackend.py - Hosts the logic that runs when buttons on the trainer GUI are clicked
10. Utility.py - contains functions to: convert tuple to dictionary, and check if a value is within a given range

**Development Data**

Created on Windows 11 (stable release as of 2024-04-09)
    functional on Windows 10

Python 3.12.2

git version 2.44.0.windows.1

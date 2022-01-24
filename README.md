Amdocs Coding Task
------------------------------------------
Created By: Connor Weimer
Date: 01/23/2022
Program: connorweimer_program.py 
------------------------------------------
Dependencies:
Python 3.9.10
pywebio version 1.5.2
sqlite3 version 2.6.0
datetime version 4.3
------------------------------------------
INSTRUCTIONS TO RUN PROGRAM
1. Verify that Python is installed.
2. Download and unzip the connorweimer_program.zip.
3. Open the command prompt and type “pip install pywebio”.
4. In the connorweimer_program folder double click the connorweimer_program.bat.
5. Copy the http address that appears in the command prompt and paste into any browser or multiple browsers. (Do not close the command prompt)
6. Enter the data into the fields and hit “Submit”.
7. Refresh to enter more rows into the database until satisfied.
8. Close the command prompt to end the program and the instance of the local server.
------------------------------------------
Process:
1. The program searches for a connection to the database product.db. If the database is not found it is created in the working directory of the running program.
2. Creates a table called product if the table does not exist. Table fields are ENTRY_ID (Auto incrementing primary key), ID integer, NUMBER integer,COMMENT text,START_DATE integer,END_DATE integer.
3. A local server instance is created, and the port is set to 8080.
4. The webpage is created when a get request is received. HTML items are rendered onto the screen. Entry fields are ready for data.
5. When “Submit” is clicked, validations are performed on the fields. If failed, error messages are displayed. 
6. After validations are passed, a local database connection is created.
7. Data from the input fields are inserted into the product table via prepared statements. 
8. The current time is taken and message displaying "Record was inserted into the database at <time>”
9. Server is live until the command prompt is closed.

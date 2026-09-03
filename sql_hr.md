# SQL HR Practice Questions
This file contains 20 basic SQL queries using the Oracle HR schema.

---

## Question 1

### Question
Display the employee ID and first name of all employees.

### Query
```sql
SELECT EMPLOYEE_ID, FIRST_NAME
FROM EMPLOYEES;
```

### Output
```text
EMPLOYEE_ID FIRST_NAME

---

198         Donald
199         Douglas
200         Jennifer
201         Michael
202         Pat
203         Susan
204         Hermann
205         Shelley
206         William
100         Steven
101         Neena
...
197         Kevin

107 rows selected.
```

---

## Question 2

### Question
Show the last name and hire date of all employees.

### Query
```sql
SELECT LAST_NAME, HIRE_DATE
FROM EMPLOYEES;
```

### Output
```text
LAST_NAME                 HIRE_DATE

---

OConnell                  21-JUN-99
Grant                     13-JAN-00
Whalen                    17-SEP-87
Hartstein                 17-FEB-96
Fay                       17-AUG-97
Mavris                    07-JUN-94
Baer                      07-JUN-94
Higgins                   07-JUN-94
Gietz                     07-JUN-94
King                      17-JUN-87
Kochhar                   21-SEP-89
...
Feeney                    23-MAY-98

107 rows selected.
```

---

## Question 3

### Question
List the job ID and salary for all employees.

### Query
```sql
SELECT JOB_ID, SALARY
FROM EMPLOYEES;
```

### Output
```text
JOB_ID         SALARY

---

SH_CLERK         2600
SH_CLERK         2600
AD_ASST          4400
MK_MAN          13000
MK_REP           6000
HR_REP           6500
PR_REP          10000
AC_MGR          12000
AC_ACCOUNT       8300
AD_PRES         24000
AD_VP           17000
...
SH_CLERK         3000

107 rows selected.
```

---

## Question 4

### Question
Display the email and phone number of all employees.

### Query
```sql
SELECT EMAIL, PHONE_NUMBER
FROM EMPLOYEES;
```

### Output
```text
EMAIL                     PHONE_NUMBER

---

DOCONNEL                  650.507.9833
DGRANT                    650.507.9844
JWHALEN                   515.123.4444
MHARTSTE                  515.123.5555
PFAY                      603.123.6666
SMAVRIS                   515.123.7777
HBAER                     515.123.8888
SHIGGINS                  515.123.8080
WGIETZ                    515.123.8181
SKING                     515.123.4567
NKOCHHAR                  515.123.4568
...
KFEENEY                   650.507.9822

107 rows selected.
```

---

## Question 5

### Question
Show the department name and location ID of all departments.

### Query
```sql
SELECT DEPARTMENT_NAME, LOCATION_ID
FROM DEPARTMENTS;
```

### Output
```text
DEPARTMENT_NAME                LOCATION_ID

---

Administration                        1700
Marketing                             1800
Purchasing                            1700
Human Resources                       2400
Shipping                              1500
IT                                    1400
Public Relations                      2700
Sales                                 2500
Executive                             1700
Finance                               1700
Accounting                            1700
Treasury                              1700
Corporate Tax                         1700
Control And Credit                    1700
Shareholder Services                  1700
Benefits                              1700
Manufacturing                         1700
Construction                          1700
Contracting                           1700
Operations                            1700
IT Support                            1700
NOC                                   1700
IT Helpdesk                           1700
Government Sales                      1700
Retail Sales                          1700
Recruiting                             1700
Payroll                               1700

27 rows selected.
```

---

## Question 6

### Question
Retrieve the employee ID, first name, and last name of all employees.

### Query
```sql
SELECT EMPLOYEE_ID, FIRST_NAME, LAST_NAME
FROM EMPLOYEES;
```

### Output
```text
EMPLOYEE_ID FIRST_NAME           LAST_NAME

---

198         Donald               OConnell
199         Douglas              Grant
200         Jennifer             Whalen
201         Michael              Hartstein
202         Pat                  Fay
203         Susan                Mavris
204         Hermann              Baer
205         Shelley              Higgins
206         William              Gietz
100         Steven               King
101         Neena                Kochhar
...
197         Kevin                Feeney

107 rows selected.
```

---

## Question 7

### Question
Show the job title and minimum salary from the jobs table.

### Query
```sql
SELECT JOB_TITLE, MIN_SALARY
FROM JOBS;
```

### Output
```text
JOB_TITLE                           MIN_SALARY

---

President                                20000
Administration Vice President            15000
Administration Assistant                  3000
Finance Manager                           8200
Accountant                                4200
Accounting Manager                        8200
Public Accountant                         4200
Sales Manager                            10000
Sales Representative                      6000
Purchasing Manager                        8000
Purchasing Clerk                          2500
Stock Manager                             5500
Stock Clerk                               2000
Shipping Clerk                            2500
Programmer                                4000
Marketing Manager                         9000
Marketing Representative                  4000
Human Resources Representative            4000
Public Relations Representative           4500

19 rows selected.
```

---

## Question 8

### Question
List the commission percentage and salary of all employees.

### Query
```sql
SELECT COMMISSION_PCT, SALARY
FROM EMPLOYEES;
```

### Output
```text
COMMISSION_PCT     SALARY

---

```
              2600
              2600
              4400
             13000
              6000
              6500
             10000
             12000
              8300
             24000
             17000
```

...
.4      14000
.3      13500
.3      12000
.3      11000
.2      10500
...
3000

107 rows selected.
```

---

## Question 9

### Question
Display the department name and manager ID for all departments.

### Query
```sql
SELECT DEPARTMENT_NAME, MANAGER_ID
FROM DEPARTMENTS;
```

### Output
```text
DEPARTMENT_NAME                MANAGER_ID

---

Administration                        200
Marketing                             201
Purchasing                            114
Human Resources                       203
Shipping                              121
IT                                    103
Public Relations                      204
Sales                                 145
Executive                             100
Finance                               108
Accounting                            205
Treasury
Corporate Tax
Control And Credit
Shareholder Services
Benefits
Manufacturing
Construction
Contracting
Operations
IT Support
NOC
IT Helpdesk
Government Sales
Retail Sales
Recruiting
Payroll

27 rows selected.
```

---

## Question 10

### Question
Retrieve the first name and job ID of all employees.

### Query
```sql
SELECT FIRST_NAME, JOB_ID
FROM EMPLOYEES;
```

### Output
```text
FIRST_NAME           JOB_ID

---

Donald               SH_CLERK
Douglas              SH_CLERK
Jennifer             AD_ASST
Michael              MK_MAN
Pat                  MK_REP
Susan                HR_REP
Hermann              PR_REP
Shelley              AC_MGR
William              AC_ACCOUNT
Steven               AD_PRES
Neena                AD_VP
...
Kevin                SH_CLERK

107 rows selected.
```

---

## Question 11

### Question
Show the job ID and maximum salary from the jobs table.

### Query
```sql
SELECT JOB_ID, MAX_SALARY
FROM JOBS;
```

### Output
```text
JOB_ID     MAX_SALARY

---

AD_PRES         40000
AD_VP           30000
AD_ASST          6000
FI_MGR          16000
FI_ACCOUNT       9000
AC_MGR          16000
AC_ACCOUNT       9000
SA_MAN          20000
SA_REP          12000
PU_MAN          15000
PU_CLERK         5500
ST_MAN           8500
ST_CLERK         5000
SH_CLERK         5500
IT_PROG         10000
MK_MAN          15000
MK_REP           9000
HR_REP           9000
PR_REP          10500

19 rows selected.
```

---

## Question 12

### Question
List the department ID and department name from the departments table.

### Query
```sql
SELECT DEPARTMENT_ID, DEPARTMENT_NAME
FROM DEPARTMENTS;
```

### Output
```text
DEPARTMENT_ID DEPARTMENT_NAME

---

10            Administration
20            Marketing
30            Purchasing
40            Human Resources
50            Shipping
60            IT
70            Public Relations
80            Sales
90            Executive
100           Finance
110           Accounting
120           Treasury
130           Corporate Tax
140           Control And Credit
150           Shareholder Services
160           Benefits
170           Manufacturing
180           Construction
190           Contracting
200           Operations
210           IT Support
220           NOC
230           IT Helpdesk
240           Government Sales
250           Retail Sales
260           Recruiting
270           Payroll

27 rows selected.
```

---

## Question 13

### Question
Display the employee ID and department ID for all employees.

### Query
```sql
SELECT EMPLOYEE_ID, DEPARTMENT_ID
FROM EMPLOYEES;
```

### Output
```text
EMPLOYEE_ID DEPARTMENT_ID

---

198         50
199         50
200         10
201         20
202         20
203         40
204         70
205         110
206         110
100         90
101         90
...
197         50

107 rows selected.
```

---

## Question 14

### Question
Show the city and state province.

### Query
```sql
SELECT CITY, STATE_PROVINCE
FROM LOCATIONS;
```

### Output
```text
CITY                           STATE_PROVINCE

---

Roma
Venice
Tokyo                          Tokyo Prefecture
Hiroshima
Southlake                      Texas
South San Francisco            California
South Brunswick                New Jersey
Seattle                        Washington
Toronto                        Ontario
Whitehorse                     Yukon
Beijing
Bombay                         Maharashtra
Sydney                         New South Wales
Singapore
London
Oxford                         Oxford
Stretford                      Manchester
Munich                         Bavaria
Sao Paulo                      Sao Paulo
Geneva                         Geneve
Bern                           BE
Utrecht                        Utrecht
Mexico City                    Distrito Federal

23 rows selected.
```

---

## Question 15

### Question
List the employee ID and hire date of all employees.

### Query
```sql
SELECT EMPLOYEE_ID, HIRE_DATE
FROM EMPLOYEES;
```

### Output
```text
EMPLOYEE_ID HIRE_DATE

---

198         21-JUN-99
199         13-JAN-00
200         17-SEP-87
201         17-FEB-96
202         17-AUG-97
203         07-JUN-94
204         07-JUN-94
205         07-JUN-94
206         07-JUN-94
100         17-JUN-87
101         21-SEP-89
...
197         23-MAY-98

107 rows selected.
```

---

## Question 16

### Question
Retrieve the first name, last name, and email of all employees.

### Query
```sql
SELECT FIRST_NAME, LAST_NAME, EMAIL
FROM EMPLOYEES;
```

### Output
```text
FIRST_NAME           LAST_NAME                 EMAIL

---

Donald               OConnell                  DOCONNEL
Douglas              Grant                     DGRANT
Jennifer             Whalen                    JWHALEN
Michael              Hartstein                 MHARTSTE
Pat                  Fay                       PFAY
Susan                Mavris                    SMAVRIS
Hermann              Baer                      HBAER
Shelley              Higgins                   SHIGGINS
William              Gietz                     WGIETZ
Steven               King                      SKING
Neena                Kochhar                   NKOCHHAR
...
Kevin                Feeney                    KFEENEY

107 rows selected.
```

---

## Question 17

### Question
Display the job title and department ID of all employees.

### Query
```sql
SELECT JOB_TITLE, DEPARTMENT_ID
FROM EMP_DETAILS_VIEW;
```

### Output
```text
JOB_TITLE                           DEPARTMENT_ID

---

Programmer                                     60
Programmer                                     60
Programmer                                     60
Programmer                                     60
Programmer                                     60
Shipping Clerk                                 50
Shipping Clerk                                 50
Shipping Clerk                                 50
...
Accountant                                    100
Finance Manager                               100
President                                      90
Administration Vice President                  90
Purchasing Clerk                               30
...
Sales Manager                                  80
Sales Representative                           80
...
Public Relations Representative                70

106 rows selected.
```

---

## Question 18

### Question
Show the department ID and location ID.

### Query
```sql
SELECT DEPARTMENT_ID, LOCATION_ID
FROM EMP_DETAILS_VIEW;
```

### Output
```text
DEPARTMENT_ID LOCATION_ID

---

60            1400
60            1400
60            1400
60            1400
60            1400
50            1500
50            1500
50            1500
...
20            1800
40            2400
80            2500
80            2500
...
70            2700

106 rows selected.
```

---

## Question 19

### Question
List the job ID and job title.

### Query
```sql
SELECT JOB_ID, JOB_TITLE
FROM JOBS;
```

### Output
```text
JOB_ID     JOB_TITLE

---

AD_PRES    President
AD_VP      Administration Vice President
AD_ASST    Administration Assistant
FI_MGR     Finance Manager
FI_ACCOUNT Accountant
AC_MGR     Accounting Manager
AC_ACCOUNT Public Accountant
SA_MAN     Sales Manager
SA_REP     Sales Representative
PU_MAN     Purchasing Manager
PU_CLERK   Purchasing Clerk
ST_MAN     Stock Manager
ST_CLERK   Stock Clerk
SH_CLERK   Shipping Clerk
IT_PROG    Programmer
MK_MAN     Marketing Manager
MK_REP     Marketing Representative
HR_REP     Human Resources Representative
PR_REP     Public Relations Representative

19 rows selected.
```

---

## Question 20

### Question
Retrieve the location ID and city name.

### Query
```sql
SELECT LOCATION_ID, CITY
FROM LOCATIONS;
```

### Output
```text
LOCATION_ID CITY

---

1000        Roma
1100        Venice
1200        Tokyo
1300        Hiroshima
1400        Southlake
1500        South San Francisco
1600        South Brunswick
1700        Seattle
1800        Toronto
1900        Whitehorse
2000        Beijing
2100        Bombay
2200        Sydney
2300        Singapore
2400        London
2500        Oxford
2600        Stretford
2700        Munich
2800        Sao Paulo
2900        Geneva
3000        Bern
3100        Utrecht
3200        Mexico City

23 rows selected.
```

# SQL WHERE CLAUSE Practice Questions

## Question 1

### Question
Retrieve all employees who belong to department 60.

### Query
```sql
SELECT *
FROM employees
WHERE department_id = 60;
```

### Output
```text
EMPLOYEE_ID FIRST_NAME LAST_NAME           EMAIL        PHONE_NUMBER       HIRE_DATE  JOB_ID         SALARY MANAGER_ID DEPARTMENT_ID
----------- ---------- -------------------- ------------ ------------------ ---------- ---------- ---------- ---------- -------------
103         Alexander  Hunold               AHUNOLD      590.423.4567      03-JAN-90  IT_PROG          9000        102            60
104         Bruce      Ernst                 BERNST       590.423.4568      21-MAY-91  IT_PROG          6000        103            60
105         David      Austin                DAUSTIN      590.423.4569      25-JUN-97  IT_PROG          4800        103            60
106         Valli      Pataballa             VPATABAL     590.423.4560      05-FEB-98  IT_PROG          4800        103            60
107         Diana      Lorentz               DLORENTZ     590.423.5567      07-FEB-99  IT_PROG          4200        103            60
```

---

## Question 2

### Question
Find all employees whose job ID is `SA_REP`.

### Query
```sql
SELECT *
FROM employees
WHERE job_id = 'SA_REP';
```

### Output
```text
EMPLOYEE_ID FIRST_NAME LAST_NAME           EMAIL        PHONE_NUMBER       HIRE_DATE  JOB_ID         SALARY MANAGER_ID DEPARTMENT_ID
----------- ---------- -------------------- ------------ ------------------ ---------- ---------- ---------- ---------- -------------
150         Peter      Tucker               PTUCKER      515.127.4561      30-JAN-97  SA_REP          10000        145            80
151         David      Bernstein            DBERNSTEIN   515.127.4562      24-MAR-97  SA_REP           9500        145            80
152         Peter      Hall                 PHALL        515.127.4563      20-AUG-97  SA_REP           9000        145            80
153         Christopher Olsen                COLSEN       515.127.4564      30-MAR-98  SA_REP           8000        145            80
154         Nanette    Cambrault             NCAMBRAUL    515.127.4565      09-DEC-98  SA_REP           7500        145            80
155         Oliver     Tuvault               OTUVAULT     515.127.4566      23-NOV-99  SA_REP           7000        145            80
156         Janette    King                 JKING        515.127.4567      30-JAN-96  SA_REP          10000        146            80
157         Patrick    Sully                PSULLY       515.127.4568      04-MAR-96  SA_REP           9500        146            80
158         Allan      McEwen               AMCEWEN      515.127.4569      01-AUG-96  SA_REP           9000        146            80
159         Lindsey    Smith                LSMITH       515.127.4560      10-MAR-97  SA_REP           8000        146            80
160         Louise     Doran                LDORAN       515.127.5567      15-DEC-97  SA_REP           7500        146            80
161         Sarina     Sewall               SSEWALL      515.127.4561      03-NOV-98  SA_REP           7000        146            80
162         Clara      Vishney              CVISHNEY     515.127.4562      11-NOV-97  SA_REP          10500        147            80
163         Danielle   Greene               DGREENE      515.127.4563      19-MAR-99  SA_REP           9500        147            80
164         Mattea     Marvins              MMARVINS     515.127.4564      24-JAN-00  SA_REP           7200        147            80
165         David      Lee                  DLEE         515.127.4565      23-FEB-00  SA_REP           6800        147            80
166         Sundar     Ande                 SANDE        515.127.4566      24-MAR-00  SA_REP           6400        147            80
167         Amit       Banda                ABANDA       515.127.4567      21-APR-00  SA_REP           6200        147            80
168         Lisa       Ozer                 LOZER        515.127.4568      11-MAR-97  SA_REP          11500        148            80
169         Harrison   Bloom                HBLOOM       515.127.4569      23-MAR-98  SA_REP          10000        148            80
170         Tayler     Fox                  TFOX         515.127.4560      24-JAN-98  SA_REP           9600        148            80
171         William    Smith                WSMITH       515.127.5567      23-FEB-99  SA_REP           7400        148            80
172         Elizabeth  Bates                EBATES       515.127.4561      24-MAR-99  SA_REP           7300        148            80
173         Sundita    Kumar                SKUMAR       515.127.4562      21-APR-00  SA_REP           6100        148            80
174         Ellen      Abel                 EABEL        590.423.4560      11-MAY-96  SA_REP          11000        149            80
175         Alyssa     Hutton               AHUTTON      590.423.4561      19-MAR-97  SA_REP           8800        149            80
176         Jonathon   Taylor               JTAYLOR      590.423.4562      24-MAR-98  SA_REP           8600        149            80
177         Jack       Livingston            JLIVINGS     590.423.4563      23-APR-98  SA_REP           8400        149            80
178         Kimberely  Grant                KGRANT       590.423.4564      24-MAY-99  SA_REP           7000        149            80
179         Charles    Johnson              CJOHNSON     515.127.4569      04-JAN-00  SA_REP           6200        149            80
```

---

## Question 3

### Question
Get all employees earning more than 80,000.

### Query
```sql
SELECT *
FROM employees
WHERE salary > 80000;
```

### Output
```text
no rows selected
```

---

## Question 4

### Question
List all employees hired after January 1, 2021.

### Query
```sql
SELECT *
FROM employees
WHERE hire_date > '01-JAN-2021';
```

### Output
```text
no rows selected
```

---

## Question 5

### Question
Retrieve all employees whose job ID is `FI_ACCOUNT`.

### Query
```sql
SELECT *
FROM employees
WHERE job_id = 'FI_ACCOUNT';
```

### Output
```text
EMPLOYEE_ID FIRST_NAME LAST_NAME           EMAIL        PHONE_NUMBER       HIRE_DATE  JOB_ID         SALARY MANAGER_ID DEPARTMENT_ID
----------- ---------- -------------------- ------------ ------------------ ---------- ---------- ---------- ---------- -------------
109         Daniel     Faviet               DFAVIET      515.127.4562      16-AUG-94  FI_ACCOUNT      9000        108           100
110         John       Chen                 JCHEN        515.127.4563      28-SEP-97  FI_ACCOUNT      8200        108           100
111         Ismael     Sciarra              ISCIARRA     515.127.4564      30-SEP-97  FI_ACCOUNT      7700        108           100
112         Jose       Urman                JURMAN       515.127.4565      07-MAR-98  FI_ACCOUNT      7800        108           100
113         Luis       Popp                 LPOPP        515.127.4567      07-DEC-99  FI_ACCOUNT      6900        108           100
```

---

## Question 6

### Question
Find all employees who report to manager ID 100.

### Query
```sql
SELECT *
FROM employees
WHERE manager_id = 100;
```

### Output
```text
EMPLOYEE_ID FIRST_NAME LAST_NAME           EMAIL        PHONE_NUMBER       HIRE_DATE  JOB_ID         SALARY MANAGER_ID DEPARTMENT_ID
----------- ---------- -------------------- ------------ ------------------ ---------- ---------- ---------- ---------- -------------
201         Michael    Hartstein            MHARTSTE      515.123.5555      17-FEB-96  MK_MAN          13000        100            20
101         Neena      Kochhar              NKOCHHAR      515.123.4568      21-SEP-89  AD_VP           17000        100            90
102         Lex        De Haan               LDEHAAN       515.123.4569      13-JAN-93  AD_VP           17000        100            90
114         Den        Raphaely              DRAPHEAL      515.127.4561      07-DEC-94  PU_MAN          11000        100            30
120         Matthew    Weiss                MWEISS        650.123.1234      18-JUL-96  ST_MAN           8000        100            50
121         Adam       Fripp                AFRIPP        650.123.2234      10-APR-97  ST_MAN           8200        100            50
122         Payam      Kaufling             PKAUFLIN      650.123.3234      01-MAY-95  ST_MAN           7900        100            50
123         Shanta     Vollman              SVOLLMAN      650.123.4234      10-OCT-97  ST_MAN           6500        100            50
124         Kevin      Mourgos              KMOURGOS      650.123.5234      16-NOV-97  ST_MAN           5800        100            50
145         John       Russell              JRUSSELL      011.44.1344.429268 01-OCT-96  SA_MAN          14000        100            80
146         Karen      Partners             KPARTNERS     011.44.1344.467268 05-JAN-97  SA_MAN          13500        100            80
147         Alberto    Errazuriz             AERRAZUR      011.44.1344.429278 10-MAR-97  SA_MAN          12000        100            80
148         Gerald     Cambrault            GCAMBRAU      011.44.1344.619268 15-OCT-99  SA_MAN          11000        100            80
149         Eleni      Zlotkey              EZLOTKEY      011.44.1344.429268 29-JAN-00  SA_MAN          10500        100            80
```

---

## Question 7

### Question
Get all employees who belong to department ID 80.

### Query
```sql
SELECT *
FROM employees
WHERE department_id = 80;
```

### Output
```text
EMPLOYEE_ID FIRST_NAME LAST_NAME           EMAIL        PHONE_NUMBER       HIRE_DATE  JOB_ID         SALARY MANAGER_ID DEPARTMENT_ID
----------- ---------- -------------------- ------------ ------------------ ---------- ---------- ---------- ---------- -------------
150         Peter      Tucker               PTUCKER      515.127.4561      30-JAN-97  SA_REP          10000        145            80
151         David      Bernstein            DBERNSTEIN   515.127.4562      24-MAR-97  SA_REP           9500        145            80
152         Peter      Hall                 PHALL        515.127.4563      20-AUG-97  SA_REP           9000        145            80
153         Christopher Olsen                COLSEN       515.127.4564      30-MAR-98  SA_REP           8000        145            80
154         Nanette    Cambrault             NCAMBRAUL    515.127.4565      09-DEC-98  SA_REP           7500        145            80
155         Oliver     Tuvault               OTUVAULT     515.127.4566      23-NOV-99  SA_REP           7000        145            80
156         Janette    King                 JKING        515.127.4567      30-JAN-96  SA_REP          10000        146            80
157         Patrick    Sully                PSULLY       515.127.4568      04-MAR-96  SA_REP           9500        146            80
158         Allan      McEwen               AMCEWEN      515.127.4569      01-AUG-96  SA_REP           9000        146            80
159         Lindsey    Smith                LSMITH       515.127.4560      10-MAR-97  SA_REP           8000        146            80
160         Louise     Doran                LDORAN       515.127.5567      15-DEC-97  SA_REP           7500        146            80
161         Sarina     Sewall               SSEWALL      515.127.4561      03-NOV-98  SA_REP           7000        146            80
162         Clara      Vishney              CVISHNEY     515.127.4562      11-NOV-97  SA_REP          10500        147            80
163         Danielle   Greene               DGREENE      515.127.4563      19-MAR-99  SA_REP           9500        147            80
164         Mattea     Marvins              MMARVINS     515.127.4564      24-JAN-00  SA_REP           7200        147            80
165         David      Lee                  DLEE         515.127.4565      23-FEB-00  SA_REP           6800        147            80
166         Sundar     Ande                 SANDE        515.127.4566      24-MAR-00  SA_REP           6400        147            80
167         Amit       Banda                ABANDA       515.127.4567      21-APR-00  SA_REP           6200        147            80
168         Lisa       Ozer                 LOZER        515.127.4568      11-MAR-97  SA_REP          11500        148            80
169         Harrison   Bloom                HBLOOM       515.127.4569      23-MAR-98  SA_REP          10000        148            80
170         Tayler     Fox                  TFOX         515.127.4560      24-JAN-98  SA_REP           9600        148            80
171         William    Smith                WSMITH       515.127.5567      23-FEB-99  SA_REP           7400        148            80
172         Elizabeth  Bates               EBATES       515.127.4561      24-MAR-99  SA_REP           7300        148            80
173         Sundita    Kumar                SKUMAR       515.127.4562      21-APR-00  SA_REP           6100        148            80
174         Ellen      Abel                 EABEL        590.423.4560      11-MAY-96  SA_REP          11000        149            80
175         Alyssa     Hutton               AHUTTON      590.423.4561      19-MAR-97  SA_REP           8800        149            80
176         Jonathon   Taylor               JTAYLOR      590.423.4562      24-MAR-98  SA_REP           8600        149            80
177         Jack       Livingston            JLIVINGS     590.423.4563      23-APR-98  SA_REP           8400        149            80
178         Kimberely  Grant                KGRANT       590.423.4564      24-MAY-99  SA_REP           7000        149            80
179         Charles    Johnson              CJOHNSON     515.127.4569      04-JAN-00  SA_REP           6200        149            80
```

---

## Question 8

### Question
Find all employees whose salary is equal to 10,000.

### Query
```sql
SELECT *
FROM employees
WHERE salary = 10000;
```

### Output
```text
EMPLOYEE_ID FIRST_NAME LAST_NAME           EMAIL        PHONE_NUMBER       HIRE_DATE  JOB_ID         SALARY MANAGER_ID DEPARTMENT_ID
----------- ---------- -------------------- ------------ ------------------ ---------- ---------- ---------- ---------- -------------
204         Hermann    Baer                 HBAER        515.123.8080      07-JUN-94  PR_REP          10000        101            70
150         Peter      Tucker               PTUCKER      515.127.4561      30-JAN-97  SA_REP          10000        145            80
156         Janette    King                 JKING        515.127.4567      30-JAN-96  SA_REP          10000        146            80
169         Harrison   Bloom                HBLOOM       515.127.4569      23-MAR-98  SA_REP          10000        148            80
```

---

## Question 9

### Question
List all employees whose commission percentage is equal to 0.10.

### Query
```sql
SELECT *
FROM employees
WHERE commission_pct = 0.10;
```

### Output
```text
EMPLOYEE_ID FIRST_NAME LAST_NAME           EMAIL        PHONE_NUMBER       HIRE_DATE  JOB_ID         SALARY COMMISSION_PCT MANAGER_ID DEPARTMENT_ID
----------- ---------- -------------------- ------------ ------------------ ---------- ---------- ---------- -------------- ---------- -------------
164         Mattea     Marvins              MMARVINS     515.127.4564      24-JAN-00  SA_REP           7200           .10        147            80
165         David      Lee                  DLEE         515.127.4565      23-FEB-00  SA_REP           6800           .10        147            80
166         Sundar     Ande                 SANDE        515.127.4566      24-MAR-00  SA_REP           6400           .10        147            80
167         Amit       Banda                ABANDA       515.127.4567      21-APR-00  SA_REP           6200           .10        147            80
173         Sundita    Kumar                SKUMAR       515.127.4562      21-APR-00  SA_REP           6100           .10        148            80
179         Charles    Johnson              CJOHNSON     515.127.4569      04-JAN-00  SA_REP           6200           .10        149            80
```

---

## Question 10

### Question
Retrieve all employees from department ID 90.

### Query
```sql
SELECT *
FROM employees
WHERE department_id = 90;
```

### Output
```text
EMPLOYEE_ID FIRST_NAME LAST_NAME           EMAIL        PHONE_NUMBER       HIRE_DATE  JOB_ID         SALARY MANAGER_ID DEPARTMENT_ID
----------- ---------- -------------------- ------------ ------------------ ---------- ---------- ---------- ---------- -------------
100         Steven     King                 SKING        515.123.4567      17-JUN-87  AD_PRES         24000                       90
101         Neena      Kochhar              NKOCHHAR      515.123.4568      21-SEP-89  AD_VP           17000        100            90
102         Lex        De Haan               LDEHAAN       515.123.4569      13-JAN-93  AD_VP           17000        100            90
```

---

## Question 11

### Question
Find all jobs whose minimum salary is greater than 5,000.

### Query
```sql
SELECT *
FROM jobs
WHERE min_salary > 5000;
```

### Output
```text
JOB_ID     JOB_TITLE                                MIN_SALARY MAX_SALARY
---------- ---------------------------------------- ---------- ----------
AD_PRES    President                                    20000      40000
AD_VP      Administration Vice President               15000      30000
FI_MGR     Finance Manager                              8200      16000
AC_MGR     Accounting Manager                           8200      16000
SA_MAN     Sales Manager                                10000      20000
SA_REP     Sales Representative                          6000      12000
PU_MAN     Purchasing Manager                            8000      15000
ST_MAN     Stock Manager                                 5500       8500
MK_MAN     Marketing Manager                             9000      15000
```

---

## Question 12

### Question
Get all employees whose first name is William.

### Query
```sql
SELECT *
FROM employees
WHERE first_name = 'William';
```

### Output
```text
EMPLOYEE_ID FIRST_NAME LAST_NAME           EMAIL        PHONE_NUMBER       HIRE_DATE  JOB_ID         SALARY MANAGER_ID DEPARTMENT_ID
----------- ---------- -------------------- ------------ ------------------ ---------- ---------- ---------- ---------- -------------
206         William    Gietz                WGIETZ       515.123.8181      07-JUN-94  AC_ACCOUNT      8300        205            110
171         William    Smith                WSMITH       515.127.5567      23-FEB-99  SA_REP           7400        148            80
```

---

## Question 13

### Question
List all departments whose location ID is 1700.

### Query
```sql
SELECT *
FROM departments
WHERE location_id = 1700;
```

### Output
```text
DEPARTMENT_ID DEPARTMENT_NAME                MANAGER_ID LOCATION_ID
------------- ------------------------------ ---------- -----------
10            Administration                       200        1700
30            Purchasing                            114        1700
90            Executive                             100        1700
100           Finance                              108        1700
110           Accounting                            205        1700
120           Treasury                                         1700
130           Corporate Tax                                    1700
140           Control And Credit                               1700
150           Shareholder Services                             1700
160           Benefits                                           1700
170           Manufacturing                                     1700
180           Construction                                     1700
190           Contracting                                     1700
200           Operations                                       1700
210           IT Support                                       1700
220           NOC                                              1700
230           IT Helpdesk                                      1700
240           Government Sales                                 1700
250           Retail Sales                                     1700
260           Recruiting                                       1700
270           Payroll                                           1700
```

---

## Question 14

### Question
Retrieve all employees from department ID 100.

### Query
```sql
SELECT *
FROM employees
WHERE department_id = 100;
```

### Output
```text
EMPLOYEE_ID FIRST_NAME LAST_NAME           EMAIL        PHONE_NUMBER       HIRE_DATE  JOB_ID         SALARY MANAGER_ID DEPARTMENT_ID
----------- ---------- -------------------- ------------ ------------------ ---------- ---------- ---------- ---------- -------------
108         Nancy      Greenberg            NGREENBE      515.124.4569      17-AUG-94  FI_MGR          12000        101           100
109         Daniel     Faviet               DFAVIET      515.127.4562      16-AUG-94  FI_ACCOUNT       9000        108           100
110         John       Chen                 JCHEN        515.127.4563      28-SEP-97  FI_ACCOUNT       8200        108           100
111         Ismael     Sciarra              ISCIARRA     515.127.4564      30-SEP-97  FI_ACCOUNT       7700        108           100
112         Jose       Urman                JURMAN       515.127.4565      07-MAR-98  FI_ACCOUNT       7800        108           100
113         Luis       Popp                 LPOPP        515.127.4567      07-DEC-99  FI_ACCOUNT       6900        108           100
```

---

## Question 15

### Question
Find all jobs whose maximum salary is less than 20,000.

### Query
```sql
SELECT *
FROM jobs
WHERE max_salary < 20000;
```

### Output
```text
JOB_ID     JOB_TITLE                                MIN_SALARY MAX_SALARY
---------- ---------------------------------------- ---------- ----------
AD_ASST    Administration Assistant                     3000       6000
FI_MGR     Finance Manager                               8200      16000
FI_ACCOUNT Accountant                                   4200       9000
AC_MGR     Accounting Manager                            8200      16000
AC_ACCOUNT Public Accountant                             4200       9000
SA_REP     Sales Representative                           6000      12000
PU_MAN     Purchasing Manager                             8000      15000
PU_CLERK   Purchasing Clerk                               2500       5500
ST_MAN     Stock Manager                                  5500       8500
ST_CLERK   Stock Clerk                                    2000       5000
SH_CLERK   Shipping Clerk                                 2500       5500
IT_PROG    Programmer                                     4000      10000
MK_MAN     Marketing Manager                              9000      15000
MK_REP     Marketing Representative                       4000       9000
HR_REP     Human Resources Representative                 4000       9000
PR_REP     Public Relations Representative                4500      10500
```

---

## Question 16

### Question
Get all employees hired on or after January 1, 2022.

### Query
```sql
SELECT *
FROM employees
WHERE hire_date >= '01-JAN-2022';
```

### Output
```text
no rows selected
```

---

## Question 17

### Question
Find all employees whose job ID is `AD_VP`.

### Query
```sql
SELECT *
FROM employees
WHERE job_id = 'AD_VP';
```

### Output
```text
EMPLOYEE_ID FIRST_NAME LAST_NAME           EMAIL        PHONE_NUMBER       HIRE_DATE  JOB_ID         SALARY MANAGER_ID DEPARTMENT_ID
----------- ---------- -------------------- ------------ ------------------ ---------- ---------- ---------- ---------- -------------
101         Neena      Kochhar              NKOCHHAR      515.123.4568      21-SEP-89  AD_VP          17000        100            90
102         Lex        De Haan               LDEHAAN       515.123.4569      13-JAN-93  AD_VP          17000        100            90
```

---

## Question 18

### Question
Retrieve the department whose department ID is 50.

### Query
```sql
SELECT *
FROM departments
WHERE department_id = 50;
```

### Output
```text
DEPARTMENT_ID DEPARTMENT_NAME                MANAGER_ID LOCATION_ID
------------- ------------------------------ ---------- -----------
50            Shipping                              121        1500
```

---

## Question 19

### Question
Get all employees whose manager ID is 102.

### Query
```sql
SELECT *
FROM employees
WHERE manager_id = 102;
```

### Output
```text
EMPLOYEE_ID FIRST_NAME LAST_NAME           EMAIL        PHONE_NUMBER       HIRE_DATE  JOB_ID         SALARY MANAGER_ID DEPARTMENT_ID
----------- ---------- -------------------- ------------ ------------------ ---------- ---------- ---------- ---------- -------------
103         Alexander  Hunold               AHUNOLD      590.423.4567      03-JAN-90  IT_PROG          9000        102            60
```

---

## Question 20

### Question
Find all locations whose country ID is `US`.

### Query
```sql
SELECT *
FROM locations
WHERE country_id = 'US';
```

### Output
```text
LOCATION_ID STREET_ADDRESS         POSTAL_CODE CITY            STATE_PROVINCE    COUNTRY_ID
----------- ---------------------- ----------- --------------- ----------------- ----------
1400        2014 Jabberwocky Rd    26192       Southlake       Texas             US
1500        2011 Interiors Blvd     99236       South San Francisco California     US
1600        2007 Zagora St          50090       South Brunswick New Jersey        US
1700        2004 Charade Rd         98199       Seattle         Washington        US
```

# SQL EXP Practice Questions

SQL expression practice using the Oracle SCOTT schema.

---

## Question 1

### Question
WAQTD NAME OF THE EMPLOYEE ALONG WITH THEIR ANNUAL SALARY.

### Query
```sql
SELECT ENAME, SAL*12 FROM EMP;
```

### Output
```text
ENAME          SAL*12
---------- ----------
SMITH            9600
ALLEN           19200
WARD            15000
JONES            35700
MARTIN           15000
BLAKE            34200
CLARK            29400
SCOTT            36000
KING             60000
TURNER           18000
ADAMS            13200
JAMES            11400
FORD             36000
MILLER           15600

14 rows selected.
```

## Question 2

### Question
WAQTD ENAME AND JOB FOR ALL THE EMPLOYEE WITH THEIR HALF TERM SALARY.

### Query
```sql
SELECT ENAME, JOB, SAL*6 FROM EMP;
```

### Output
```text
ENAME      JOB            SAL*6
---------- --------- ----------
SMITH      CLERK           4800
ALLEN      SALESMAN        9600
WARD       SALESMAN        7500
JONES      MANAGER        17850
MARTIN     SALESMAN        7500
BLAKE      MANAGER        17100
CLARK      MANAGER        14700
SCOTT      ANALYST        18000
KING       PRESIDENT      30000
TURNER     SALESMAN        9000
ADAMS      CLERK           6600
JAMES      CLERK           5700
FORD       ANALYST        18000
MILLER     CLERK           7800

14 rows selected.
```

## Question 3

### Question
WAQTD ALL THE DETAILS OF THE EMPLOYEES ALONG WITH AN ANNUAL BONUS OF 2000.

### Query
```sql
SELECT EMP.*, SAL*12+2000 FROM EMP;
```

### Output
```text
EMPNO ENAME      JOB              MGR HIREDATE         SAL       COMM     DEPTNO SAL*12+2000
---------- ---------- --------- ---------- --------- ---------- ---------- ---------- -----------
7369 SMITH      CLERK           7902 17-DEC-80        800                    20       11600
7499 ALLEN      SALESMAN        7698 20-FEB-81       1600        300         30       21200
7521 WARD       SALESMAN        7698 22-FEB-81       1250        500         30       17000
7566 JONES      MANAGER         7839 02-APR-81       2975                    20       37700
7654 MARTIN     SALESMAN        7698 28-SEP-81       1250       1400         30       17000
7698 BLAKE      MANAGER         7839 01-MAY-81       2850                    30       36200
7782 CLARK      MANAGER         7839 09-JUN-81       2450                    10       31400
7788 SCOTT      ANALYST         7566 19-APR-87       3000                    20       38000
7839 KING       PRESIDENT            17-NOV-81       5000                    10       62000
7844 TURNER     SALESMAN        7698 08-SEP-81       1500          0         30       20000
7876 ADAMS      CLERK           7788 23-MAY-87       1100                    20       15200
7900 JAMES      CLERK           7698 03-DEC-81        950                    30       13400
7902 FORD       ANALYST         7566 03-DEC-81       3000                    20       38000
7934 MILLER     CLERK           7782 23-JAN-82       1300                    10       17600

14 rows selected.
```

## Question 4

### Question
WAQTD NAME SALARY AND SALARY WITH A HIKE OF 10%.

### Query
```sql
SELECT ENAME, SAL, SAL+SAL*0.1 FROM EMP;
```

### Output
```text
ENAME             SAL SAL+SAL*0.1
---------- ---------- -----------
SMITH             800         880
ALLEN            1600        1760
WARD             1250        1375
JONES            2975      3272.5
MARTIN           1250        1375
BLAKE            2850        3135
CLARK            2450        2695
SCOTT            3000        3300
KING             5000        5500
TURNER           1500        1650
ADAMS            1100        1210
JAMES             950        1045
FORD             3000        3300
MILLER           1300        1430

14 rows selected.
```

## Question 5

### Question
WAQTD NAME AND SALARY WITH DEDUCTION OF 25%.

### Query
```sql
SELECT ENAME, SAL-SAL*0.25 FROM EMP;
```

### Output
```text
ENAME      SAL-SAL*0.25
---------- ------------
SMITH               600
ALLEN              1200
WARD              937.5
JONES           2231.25
MARTIN            937.5
BLAKE            2137.5
CLARK            1837.5
SCOTT              2250
KING               3750
TURNER             1125
ADAMS               825
JAMES             712.5
FORD               2250
MILLER              975

14 rows selected.
```

## Question 6

### Question
WAQTD NAME AND SALARY WITH MONTHLY HIKE OF 50%.

### Query
```sql
SELECT ENAME, SAL+SAL*0.5 FROM EMP;
```

### Output
```text
ENAME      SAL+SAL*0.5
---------- -----------
SMITH             1200
ALLEN             2400
WARD              1875
JONES           4462.5
MARTIN            1875
BLAKE             4275
CLARK             3675
SCOTT             4500
KING              7500
TURNER            2250
ADAMS             1650
JAMES             1425
FORD              4500
MILLER            1950

14 rows selected.
```

## Question 7

### Question
WAQTD NAME AND ANNUAL SALARY WITH DEDUCTION OF 10%.

### Query
```sql
SELECT ENAME, SAL*12-(SAL*0.1) FROM EMP;
```

### Output
```text
ENAME      SAL*12-(SAL*0.1)
---------- ----------------
SMITH                  9520
ALLEN                 19040
WARD                  14875
JONES               35402.5
MARTIN                14875
BLAKE                 33915
CLARK                 29155
SCOTT                 35700
KING                  59500
TURNER                17850
ADAMS                 13090
JAMES                 11305
FORD                  35700
MILLER                15470

14 rows selected.
```

## Question 8

### Question
WAQTD TOTAL SALARY GIVEN TO EACH EMPLOYEE (SAL+COMM).

### Query
```sql
SELECT SAL+COMM FROM EMP;
```

### Output
```text
SAL+COMM
----------
1900
1750
2650

14 rows selected.
```

## Question 9

### Question
WAQTD DETAILS OF ALL THE EMPLOYEES ALONG WITH ANNUAL SALARY.

### Query
```sql
SELECT EMP.*, SAL*12 FROM EMP;
```

### Output
```text
EMPNO ENAME      JOB              MGR HIREDATE         SAL       COMM     DEPTNO     SAL*12
---------- ---------- --------- ---------- --------- ---------- ---------- ---------- ----------
7369 SMITH      CLERK           7902 17-DEC-80        800                    20       9600
7499 ALLEN      SALESMAN        7698 20-FEB-81       1600        300         30      19200
7521 WARD       SALESMAN        7698 22-FEB-81       1250        500         30      15000
7566 JONES      MANAGER         7839 02-APR-81       2975                    20      35700
7654 MARTIN     SALESMAN        7698 28-SEP-81       1250       1400         30      15000
7698 BLAKE      MANAGER         7839 01-MAY-81       2850                    30      34200
7782 CLARK      MANAGER         7839 09-JUN-81       2450                    10      29400
7788 SCOTT      ANALYST         7566 19-APR-87       3000                    20      36000
7839 KING       PRESIDENT            17-NOV-81       5000                    10      60000
7844 TURNER     SALESMAN        7698 08-SEP-81       1500          0         30      18000
7876 ADAMS      CLERK           7788 23-MAY-87       1100                    20      13200
7900 JAMES      CLERK           7698 03-DEC-81        950                    30      11400
7902 FORD       ANALYST         7566 03-DEC-81       3000                    20      36000
7934 MILLER     CLERK           7782 23-JAN-82       1300                    10      15600

14 rows selected.
```

## Question 10

### Question
WAQTD NAME AND DESIGNATION ALONG WITH 100 PENALTY IN SALARY.

### Query
```sql
SELECT ENAME, JOB, SAL-100 FROM EMP;
```

### Output
```text
ENAME      JOB          SAL-100
---------- --------- ----------
SMITH      CLERK            700
ALLEN      SALESMAN        1500
WARD       SALESMAN        1150
JONES      MANAGER         2875
MARTIN     SALESMAN        1150
BLAKE      MANAGER         2750
CLARK      MANAGER         2350
SCOTT      ANALYST         2900
KING       PRESIDENT       4900
TURNER     SALESMAN        1400
ADAMS      CLERK           1000
JAMES      CLERK            850
FORD       ANALYST         2900
MILLER     CLERK           1200

14 rows selected.
```

---

## Verification Notes

- **Question 2:** The first command in the SQL*Plus transcript contains a typo (`selecr`), which produced `SP2-0734`. The following `SELECT` is the correct successful query, so only that query is included here. fileciteturn1file0L38-L41
- **Question 3:** `SAL*12+2000` correctly calculates annual salary plus a fixed 2000 bonus. The transcript also shows the same query after `SET PAGES 100 LINES 100`, which only changes display formatting. fileciteturn1file0L137-L157
- **Question 7:** The query subtracts 10% from the annual salary, but the expression shown is `SAL*12-(SAL*0.1)`. If the intended meaning is **10% deduction from annual salary**, the mathematically correct expression would normally be `SAL*12-(SAL*12*0.1)`. The file preserves the query actually used in the transcript rather than silently changing it. fileciteturn1file0L226-L246
- **Question 8:** `SAL + COMM` produces `NULL` whenever `COMM` is `NULL`, which is why several employees have blank calculated values in the SQL*Plus output. fileciteturn1file0L248-L289

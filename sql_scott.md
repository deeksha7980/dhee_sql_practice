# SQL SCOTT Practice Questions

This file contains 10 basic SQL queries using the Oracle SCOTT schema.

---

## Question 1

### Question
Write a query to display all the details from the employee table.

### Query
```sql
SELECT * FROM EMP;
```

### Output
```text
     EMPNO ENAME      JOB              MGR HIREDATE         SAL       COMM
---------- ---------- --------- ---------- --------- ---------- ----------
    DEPTNO
----------
      7369 SMITH      CLERK           7902 17-DEC-80        800
        20

      7499 ALLEN      SALESMAN        7698 20-FEB-81       1600        300
        30

      7521 WARD       SALESMAN        7698 22-FEB-81       1250        500
        30

      7566 JONES      MANAGER         7839 02-APR-81       2975
        20

      7654 MARTIN     SALESMAN        7698 28-SEP-81       1250       1400
        30

      7698 BLAKE      MANAGER         7839 01-MAY-81       2850
        30

      7782 CLARK      MANAGER         7839 09-JUN-81       2450
        10

      7788 SCOTT      ANALYST         7566 19-APR-87       3000
        20

      7839 KING       PRESIDENT            17-NOV-81       5000
        10

      7844 TURNER     SALESMAN        7698 08-SEP-81       1500          0
        30

      7876 ADAMS      CLERK           7788 23-MAY-87       1100
        20

      7900 JAMES      CLERK           7698 03-DEC-81        950
        30

      7902 FORD       ANALYST         7566 03-DEC-81       3000
        20

      7934 MILLER     CLERK           7782 23-JAN-82       1300
        10

14 rows selected.
```

---

## Question 2

### Question
WAQTD names of all the employees.

### Query
```sql
SELECT ENAME FROM EMP;
```

### Output
```text
ENAME
----------
SMITH
ALLEN
WARD
JONES
MARTIN
BLAKE
CLARK
SCOTT
KING
TURNER
ADAMS

ENAME
----------
JAMES
FORD
MILLER

14 rows selected.
```

---

## Question 3

### Question
WAQTD name and salary given to all the employees.

### Query
```sql
SELECT ENAME, SAL FROM EMP;
```

### Output
```text
ENAME             SAL
---------- ----------
SMITH             800
ALLEN            1600
WARD             1250
JONES            2975
MARTIN           1250
BLAKE            2850
CLARK            2450
SCOTT            3000
KING             5000
TURNER           1500
ADAMS            1100

ENAME             SAL
---------- ----------
JAMES             950
FORD             3000
MILLER           1300

14 rows selected.
```

---

## Question 4

### Question
WAQTD name and commission given to all the employees.

### Query
```sql
SELECT ENAME, COMM FROM EMP;
```

### Output
```text
ENAME            COMM
---------- ----------
SMITH
ALLEN             300
WARD              500
JONES
MARTIN           1400
BLAKE
CLARK
SCOTT
KING
TURNER              0
ADAMS

ENAME            COMM
---------- ----------
JAMES
FORD
MILLER

14 rows selected.
```

---

## Question 5

### Question
WAQTD employee ID and department number of all the employees in EMP table.

### Query
```sql
SELECT EMPNO, DEPTNO FROM EMP;
```

### Output
```text
     EMPNO     DEPTNO
---------- ----------
      7369         20
      7499         30
      7521         30
      7566         20
      7654         30
      7698         30
      7782         10
      7788         20
      7839         10
      7844         30
      7876         20

     EMPNO     DEPTNO
---------- ----------
      7900         30
      7902         20
      7934         10

14 rows selected.
```

---

## Question 6

### Question
WAQTD ENAME and HIREDATE of all the employees.

### Query
```sql
SELECT ENAME, HIREDATE FROM EMP;
```

### Output
```text
ENAME      HIREDATE
---------- ---------
SMITH      17-DEC-80
ALLEN      20-FEB-81
WARD       22-FEB-81
JONES      02-APR-81
MARTIN     28-SEP-81
BLAKE      01-MAY-81
CLARK      09-JUN-81
SCOTT      19-APR-87
KING       17-NOV-81
TURNER     08-SEP-81
ADAMS      23-MAY-87

ENAME      HIREDATE
---------- ---------
JAMES      03-DEC-81
FORD       03-DEC-81
MILLER     23-JAN-82

14 rows selected.
```

---

## Question 7

### Question
WAQTD name and designation of all the employees.

### Query
```sql
SELECT ENAME, JOB FROM EMP;
```

### Output
```text
ENAME      JOB
---------- ---------
SMITH      CLERK
ALLEN      SALESMAN
WARD       SALESMAN
JONES      MANAGER
MARTIN     SALESMAN
BLAKE      MANAGER
CLARK      MANAGER
SCOTT      ANALYST
KING       PRESIDENT
TURNER     SALESMAN
ADAMS      CLERK

ENAME      JOB
---------- ---------
JAMES      CLERK
FORD       ANALYST
MILLER     CLERK

14 rows selected.
```

---

## Question 8

### Question
WAQTD name, job and salary given to all the employees.

### Query
```sql
SELECT ENAME, JOB, SAL FROM EMP;
```

### Output
```text
ENAME      JOB              SAL
---------- --------- ----------
SMITH      CLERK            800
ALLEN      SALESMAN        1600
WARD       SALESMAN        1250
JONES      MANAGER         2975
MARTIN     SALESMAN        1250
BLAKE      MANAGER         2850
CLARK      MANAGER         2450
SCOTT      ANALYST         3000
KING       PRESIDENT       5000
TURNER     SALESMAN        1500
ADAMS      CLERK           1100

ENAME      JOB              SAL
---------- --------- ----------
JAMES      CLERK            950
FORD       ANALYST         3000
MILLER     CLERK           1300

14 rows selected.
```

---

## Question 9

### Question
WAQTD DNAMES present in department table.

### Query
```sql
SELECT DNAME FROM DEPT;
```

### Output
```text
DNAME
--------------
ACCOUNTING
RESEARCH
SALES
OPERATIONS
```

---

## Question 10

### Question
WAQTD DNAME and location present in DEPT table.

### Query
```sql
SELECT DNAME, LOC FROM DEPT;
```

### Output
```text
DNAME          LOC
-------------- -------------
ACCOUNTING     NEW YORK
RESEARCH       DALLAS
SALES          CHICAGO
OPERATIONS     BOSTON
```

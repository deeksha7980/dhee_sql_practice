WHERE Clause

Question 1

Question

WAQTD the annual salary of the employee whose name is SMITH.

Query

SELECT sal*12 FROM emp WHERE ename='SMITH';

Output

    SAL*12
----------
      9600

Question 2

Question

WAQTD name of the employees working as CLERK.

Query

SELECT ename FROM emp WHERE job='CLERK';

Output

ENAME
----------
SMITH
ADAMS
JAMES
MILLER

Question 3

Question

WAQTD salary of the employees who are working as SALESMAN.

Query

SELECT sal FROM emp WHERE job='SALESMAN';

Output

       SAL
----------
      1600
      1250
      1250
      1500

Question 4

Question

WAQTD details of the employees who earn more than 2000.

Query

SELECT * FROM emp WHERE sal>2000;

Output

     EMPNO ENAME      JOB              MGR HIREDATE         SAL       COMM     DEPTNO
---------- ---------- --------- ---------- --------- ---------- ---------- ----------
      7566 JONES      MANAGER         7839 02-APR-81       2975                    20
      7698 BLAKE      MANAGER         7839 01-MAY-81       2850                    30
      7782 CLARK      MANAGER         7839 09-JUN-81       2450                    10
      7788 SCOTT      ANALYST         7566 19-APR-87       3000                    20
      7839 KING       PRESIDENT            17-NOV-81       5000                    10
      7902 FORD       ANALYST         7566 03-DEC-81       3000                    20

6 rows selected.

Question 5

Question

WAQTD details of the employee whose name is JONES.

Query

SELECT * FROM emp WHERE ename='JONES';

Output

     EMPNO ENAME      JOB              MGR HIREDATE         SAL       COMM     DEPTNO
---------- ---------- --------- ---------- --------- ---------- ---------- ----------
      7566 JONES      MANAGER         7839 02-APR-81       2975                    20

Question 6

Question

WAQTD details of the employee who was hired after 01-JAN-81.

Query

SELECT * FROM emp WHERE hiredate>'01-JAN-81';

Output

     EMPNO ENAME      JOB              MGR HIREDATE         SAL       COMM     DEPTNO
---------- ---------- --------- ---------- --------- ---------- ---------- ----------
      7499 ALLEN      SALESMAN        7698 20-FEB-81       1600        300         30
      7521 WARD       SALESMAN        7698 22-FEB-81       1250        500         30
      7566 JONES      MANAGER         7839 02-APR-81       2975                    20
      7654 MARTIN     SALESMAN        7698 28-SEP-81       1250       1400         30
      7698 BLAKE      MANAGER         7839 01-MAY-81       2850                    30
      7782 CLARK      MANAGER         7839 09-JUN-81       2450                    10
      7788 SCOTT      ANALYST         7566 19-APR-87       3000                    20
      7839 KING       PRESIDENT            17-NOV-81       5000                    10
      7844 TURNER     SALESMAN        7698 08-SEP-81       1500          0         30
      7876 ADAMS      CLERK           7788 23-MAY-87       1100                    20
      7900 JAMES      CLERK           7698 03-DEC-81        950                    30
      7902 FORD       ANALYST         7566 03-DEC-81       3000                    20
      7934 MILLER     CLERK           7782 23-JAN-82       1300                    10

13 rows selected.

Question 7

Question

WAQTD name and salary along with annual salary if the annual salary is more than 12000.

Query

SELECT ename,sal,sal*12 FROM emp WHERE sal*12>12000;

Output

ENAME             SAL     SAL*12
---------- ---------- ----------
ALLEN            1600      19200
WARD             1250      15000
JONES            2975      35700
MARTIN           1250      15000
BLAKE            2850      34200
CLARK            2450      29400
SCOTT            3000      36000
KING             5000      60000
TURNER           1500      18000
ADAMS            1100      13200
FORD             3000      36000
MILLER           1300      15600

12 rows selected.

Question 8

Question

WAQTD EMPNO of the employees who are working in DEPT 30.

Query

SELECT empno FROM emp WHERE deptno=30;

Output

     EMPNO
----------
      7499
      7521
      7654
      7698
      7844
      7900

6 rows selected.

Question 9

Question

WAQTD ENAME and HIREDATE if they are hired before 1981.

Query

SELECT ename,hiredate FROM emp WHERE hiredate<'01-JAN-1981';

Output

ENAME      HIREDATE
---------- ---------
SMITH      17-DEC-80

Question 10

Question

WAQTD details of the employees working as MANAGER.

Query

SELECT * FROM emp WHERE job='MANAGER';

Output

     EMPNO ENAME      JOB              MGR HIREDATE         SAL       COMM     DEPTNO
---------- ---------- --------- ---------- --------- ---------- ---------- ----------
      7566 JONES      MANAGER         7839 02-APR-81       2975                    20
      7698 BLAKE      MANAGER         7839 01-MAY-81       2850                    30
      7782 CLARK      MANAGER         7839 09-JUN-81       2450                    10

Question 11

Question

WAQTD name and salary given to an employee if employee earns a commission of rupees 1400.

Query

SELECT ename,sal FROM emp WHERE comm=1400;

Output

ENAME             SAL
---------- ----------
MARTIN           1250

Question 12

Question

WAQTD details of employees having commission more than salary.

Query

SELECT * FROM emp WHERE comm>sal;

Output

     EMPNO ENAME      JOB              MGR HIREDATE         SAL       COMM     DEPTNO
---------- ---------- --------- ---------- --------- ---------- ---------- ----------
      7654 MARTIN     SALESMAN        7698 28-SEP-81       1250       1400         30

Question 13

Question

WAQTD EMPNO of employees hired before the year 87.

Query

SELECT empno FROM emp WHERE hiredate < '01-JAN-1987';

Output

     EMPNO
----------
      7369
      7499
      7521
      7566
      7654
      7698
      7782
      7839
      7844
      7900
      7902
      7934

12 rows selected.

Question 14

Question

WAQTD details of employees working as ANALYST.

Query

SELECT * FROM emp WHERE job='ANALYST';

Output

     EMPNO ENAME      JOB              MGR HIREDATE         SAL       COMM     DEPTNO
---------- ---------- --------- ---------- --------- ---------- ---------- ----------
      7788 SCOTT      ANALYST         7566 19-APR-87       3000                    20
      7902 FORD       ANALYST         7566 03-DEC-81       3000                    20

Question 15

Question

WAQTD details of the employees earning more than 2000 rupees per month.

Query

SELECT * FROM emp WHERE sal>2000;

Output

     EMPNO ENAME      JOB              MGR HIREDATE         SAL       COMM     DEPTNO
---------- ---------- --------- ---------- --------- ---------- ---------- ----------
      7566 JONES      MANAGER         7839 02-APR-81       2975                    20
      7698 BLAKE      MANAGER         7839 01-MAY-81       2850                    30
      7782 CLARK      MANAGER         7839 09-JUN-81       2450                    10
      7788 SCOTT      ANALYST         7566 19-APR-87       3000                    20
      7839 KING       PRESIDENT            17-NOV-81       5000                    10
      7902 FORD       ANALYST         7566 03-DEC-81       3000                    20

6 rows selected.

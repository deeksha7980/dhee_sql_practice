WHERE CLAUSE:
1.WAQTD THE ANNUAL SALARY OF THE EMPLOYEE WHOS NAME IS SMITH
2.WAQTD NAME OF THE EMPLOYEES WORKING AS CLERK
3.WAQTD SALARY OF THE EMPLOYEES WHO ARE WORKING AS SALESMAN
4.WAQTD DETAILS OF THE EMP WHO EARNS MORE THAN 2000
5.WAQTD DETAILS OF THE EMP WHOS NAME IS JONES
6.WAQTD DETAILS OF THE EMP WHO WAS HIRED AFTER 01-JAN-81
7.WAQTD NAME AND SAL ALONG WITH HIS ANNUAL 
SALARY IF THE ANNUAL SALARY IS MORE THAN 12000
8.WAQTD EMPNO OF THE EMPLOYEES WHO ARE WORKING 
IN DEPT 30 
9.WAQTD ENAME AND HIREDATE IF THEY ARE HIRED BEFORE 1981
10.WAQTD DETAILS OF THE EMPLOYEES WORKING AS MANAGER
11.WAQTD NAME AND SALARY GIVEN TO AN EMPLOYEE IF EMPLOYEE 
EARNS A COMMISSION OF RUPEES 1400 
12.WAQTD DETAILS OF EMPLOYEES HAVING COMMISSION MORE THAN 
SALARY 
13.WAQTD EMPNO OF EMPLOYEES HIRED BEFORE THE YEAR 87
14.WAQTD DETAILS OF EMPLOYEES WORKING AS AN N ANALYST
15.WAQTD DETAILS OF EMPS EARNING MORE THAN 2000 RUPEES PER MONTH



SQL> desc emp
 Name                                      Null?    Type
 ----------------------------------------- -------- ----------------------------
 EMPNO                                     NOT NULL NUMBER(4)
 ENAME                                              VARCHAR2(10)
 JOB                                                VARCHAR2(9)
 MGR                                                NUMBER(4)
 HIREDATE                                           DATE
 SAL                                                NUMBER(7,2)
 COMM                                               NUMBER(7,2)
 DEPTNO                                             NUMBER(2)

SQL> select sal*12 from emp where ename='SMITH';

    SAL*12
----------
      9600

SQL> select ename from emp where job='CLERK';

ENAME
----------
SMITH
ADAMS
JAMES
MILLER

SQL> select sal from emp where job='SALESMAN';

       SAL
----------
      1600
      1250
      1250
      1500

SQL> select * from emp where sal>2000;

     EMPNO ENAME      JOB              MGR HIREDATE         SAL       COMM
---------- ---------- --------- ---------- --------- ---------- ----------
    DEPTNO
----------
      7566 JONES      MANAGER         7839 02-APR-81       2975
        20

      7698 BLAKE      MANAGER         7839 01-MAY-81       2850
        30

      7782 CLARK      MANAGER         7839 09-JUN-81       2450
        10


     EMPNO ENAME      JOB              MGR HIREDATE         SAL       COMM
---------- ---------- --------- ---------- --------- ---------- ----------
    DEPTNO
----------
      7788 SCOTT      ANALYST         7566 19-APR-87       3000
        20

      7839 KING       PRESIDENT            17-NOV-81       5000
        10

      7902 FORD       ANALYST         7566 03-DEC-81       3000
        20


6 rows selected.

SQL> set pages 100 lines 100;
SQL> select * from emp where sal>2000;

     EMPNO ENAME      JOB              MGR HIREDATE         SAL       COMM     DEPTNO
---------- ---------- --------- ---------- --------- ---------- ---------- ----------
      7566 JONES      MANAGER         7839 02-APR-81       2975                    20
      7698 BLAKE      MANAGER         7839 01-MAY-81       2850                    30
      7782 CLARK      MANAGER         7839 09-JUN-81       2450                    10
      7788 SCOTT      ANALYST         7566 19-APR-87       3000                    20
      7839 KING       PRESIDENT            17-NOV-81       5000                    10
      7902 FORD       ANALYST         7566 03-DEC-81       3000                    20

6 rows selected.

SQL> seelct * from emp where ename='JONES';
SP2-0734: unknown command beginning "seelct * f..." - rest of line ignored.
SQL> select * from emp where ename='JONES';

     EMPNO ENAME      JOB              MGR HIREDATE         SAL       COMM     DEPTNO
---------- ---------- --------- ---------- --------- ---------- ---------- ----------
      7566 JONES      MANAGER         7839 02-APR-81       2975                    20

SQL> select * from emp where hiredate>'01-JAN-81';

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

SQL> select ename,sal,sal*12 from emp where sal*12>12000;

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

SQL> select empno from emp where deptno=30;

     EMPNO
----------
      7499
      7521
      7654
      7698
      7844
      7900

6 rows selected.

SQL> select ename,hiredate from emp where hiredate<'01-JAN-1981';

ENAME      HIREDATE
---------- ---------
SMITH      17-DEC-80

SQL> select * from emp where job='MANAGER';

     EMPNO ENAME      JOB              MGR HIREDATE         SAL       COMM     DEPTNO
---------- ---------- --------- ---------- --------- ---------- ---------- ----------
      7566 JONES      MANAGER         7839 02-APR-81       2975                    20
      7698 BLAKE      MANAGER         7839 01-MAY-81       2850                    30
      7782 CLARK      MANAGER         7839 09-JUN-81       2450                    10

SQL> select ename,sal from emp where comm=1400;

ENAME             SAL
---------- ----------
MARTIN           1250

SQL> select * from emp where comm>sal;

     EMPNO ENAME      JOB              MGR HIREDATE         SAL       COMM     DEPTNO
---------- ---------- --------- ---------- --------- ---------- ---------- ----------
      7654 MARTIN     SALESMAN        7698 28-SEP-81       1250       1400         30

SQL> select empno from emp where hiredate < '01-JAN-1987';

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

SQL> select * from emp where job='ANALYST';

     EMPNO ENAME      JOB              MGR HIREDATE         SAL       COMM     DEPTNO
---------- ---------- --------- ---------- --------- ---------- ---------- ----------
      7788 SCOTT      ANALYST         7566 19-APR-87       3000                    20
      7902 FORD       ANALYST         7566 03-DEC-81       3000                    20

SQL> select * from emp where sal>2000;

     EMPNO ENAME      JOB              MGR HIREDATE         SAL       COMM     DEPTNO
---------- ---------- --------- ---------- --------- ---------- ---------- ----------
      7566 JONES      MANAGER         7839 02-APR-81       2975                    20
      7698 BLAKE      MANAGER         7839 01-MAY-81       2850                    30
      7782 CLARK      MANAGER         7839 09-JUN-81       2450                    10
      7788 SCOTT      ANALYST         7566 19-APR-87       3000                    20
      7839 KING       PRESIDENT            17-NOV-81       5000                    10
      7902 FORD       ANALYST         7566 03-DEC-81       3000                    20

6 rows selected.

SQL>

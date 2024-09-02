# Reading-Assignment

# Table of contents

# Assignment 1

240902 | 교재 1.1 ~ 1.5, 1.7

## 1.2. File system vs. DBMS

## 1.3. DBMS 발전 과정

# Terminologies

- database
    
    a usually large collection of data oraganized especially for rapid search and retrieval(as by a computer).
    
- DBMS
    
    A database management system (DBMS) is a system or **software or system software or software package** designed to manage a database, and **run operations** on the data requested by **numerous clients**.
    
- schema, metadata, structure, intension, system catalog(얘는 엄밀히는 다름)
    
    ```sql
    DEPARTMENT(DEPTNO: integer, DEPTNAME: char(10), FLOOR: integer)
    EMPLOYEE(EMPNO: integer, EMPNAME: char(10), TITLE: char(10), **DNO**: integer, SALARY: integer)
    ```
    
    교재18p. system catalog는 저장된 데이터베이스의 스키마 정보를 유지한다. 사용자가 새로운 테이블을 만들거나 기존의 테이블에 새로운 attribute를 추가하는 작업 등을 수행하면 system catalog에 이를 반영하는 schema 정보가 삽입된다. 8장에서 자세하게 설명한다.
    
- state, extension, operational data, stored data
    
    **DEPARTMENT**
    
    | DEPTNO | DEPTNAME | FLOOR |
    | --- | --- | --- |
    | 1 | 영업 | 8 |
    | 2 | 기획 | 10 |
    | 3 | 개발 | 9 |
    
    **EMPLOYEE**
    
    | EMPNO | EMPNAME | TITLE | DNO | SALARY |
    | --- | --- | --- | --- | --- |
    | 2106 | 김창섭 | 대리 | 2 | 2000000 |
    | 3426 | 박영권 | 과장 | 3 | 2500000 |
    | 3011 | 이수민 | 부장 | 1 | 3000000 |
    | 1003 | 조민희 | 대리 | 1 | 2000000 |
    | 3427 | 최종철 | 사원 | 3 | 1500000 |
- SQL; Structured Query Language
    
    SQL is a domain-specific language used to manage data, especially in a relational database management system(RDBMS).
    
- non-procedural language; 비절차적 언어
    
    어떤 데이터를 원하는가만 명시하고 데이터를 검색하는 방법은 명시하지 않는 언어. SQL이 여기에 속한다.
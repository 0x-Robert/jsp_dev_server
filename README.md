# jsp_dev_server
jsp_test_server


JSP 구축 



시스템 환경변수추가 

JAVA_HOME C:\Program Files\Java\jdk1.8.0_221

PATH: C:\Program Files\Java\jdk1.8.0_221\bin

eclips 톰캣 폴더 설정 톰캫 8.5 



mysql installer 설치



mysql 3306 

id : root
pw : root


mysql> CREATE DATABASE BBS;


mysql> USE BBS;

CREATE TABLE USER (
 userID VARCHAR(20),
 userPassword VARCHAR(20),
 userName VARCHAR(20),
 userGender VARCHAR(20),
 userEmail VARCHAR(50),
 PRIMARY KEY (userID)
);

mysql> show tables;

mysql> desc user;

mysql> INSERT INTO USER VALUES('gildong','123456','홍길동','남자','gildong@naver.com');

mysql> SELECT * FROM USER;

mysql >  commit;

프로젝트 우클릭 프로퍼티즈 설정 
Java build path : 


mysql> 
CREATE TABLE BBS(
bbsID INT,
bbsTitle VARCHAR(20),
userID VARCHAR(20),
bbsDate DATETIME,
bbsContent VARCHAR(2048),
bbsAvailable INT,
PRIMARY KEY (bbsID)
);

pacakage bbs;

public class Bbs {

private int bbsID;
private String bbsTitle;
private String userID;
private String bbsDate;
private String bbsContent;
private int bbsAvailable;

}

소스(getter and setters)
beans 데이터베이스랑 비슷 함 









loginAction.jsp
response.sendRedirect("main.jsp");


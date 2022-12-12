# Oracle database-study

day 1
* SQL Table
* DDL
* DML
* DCL

-Oracle은 table단위로 객체를 저장. table에 접근하기 위해서는 그 table을 소유하고 있는 user에 접속해야함

DCL (Data Control Language)
-user를 추가, 삭제하고 권한을 주거나 회수하는 명령어

-새 계정 만들기 ( system 권한으로 가능)
create user identified by password account unlock 

ex)
create comstudy identified by comstudy account unlock
conn comstudy/comstudy -> comstudy 사용자 접속

-권한 생성 : 생성한 사용자에게 객체 접근권한이나 접속 권한을 부여함 (system 권한으로 가능)
ex) grant dba to comstudy ( dba 권한을 comstudy 에게 부여)

-권한 삭제 : 생성한 사용자의 접근권한을 회수
ex) revoke dba from comstudy

DDL (Data Definition Language)
CREATE : 테이블 생성
DROP : 테이블 삭제
ALTER : 테이블 수정
TRUNCATE : 테이블에 있는 모든 데이터 삭제

ex) create table table_name(
column_name datatype constrain,
..,
..,
)







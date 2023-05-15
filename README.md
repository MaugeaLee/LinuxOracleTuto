# LinuxOracleTuto
## 리눅스 버전별 차이
1. Oracle Personal Edition(PE)

- CPU 개수와 상관없이 단일 사용자만 사용이 가능함
- 개발자용 버전
- 인터넷 / 네트워크와의 연결 불가능
- 교육용, 개발용으로 사용


2. Oracle eXpress Edition(XE)

- 개발 용도로 배포되는 무료버전
- 상업적 용도 사용 불가
- 최대 4GB의 사용자 데이터만 사용 가능
- 단일 인스턴스로 제한
- 초급 수준의 소규모 데이터 베이스


3. Oracle Standard Edition One(SE1)

- 2 CPU까지 확장 가능한 서버에 설치 가능
- 400명 미만의 사용자가 있는 회사 조직에 적합


4. Oracle Standard Edition(SE)

- 4 CPU까지 확장 가능한 서버에 설치 가능
- 1000명 미만의 사업장에 적당
- GB 데이터 베이스 크기에 적합


5. Oracle Enterprise Edition(EE)

- 4 CPU 이상 확장 가능한 서버에 설치 가능
- Oracle에서 제공하는 DB 성능중 최고 성능

6. Oracle Develope Edition

- 23c에서 새롭게 출시된 개발자용 무료 에디션
- XE보다 높은 성능을 발휘함

<div align="center">
  <b> PE, XE < SE < EE </b><br>
  에디션은 위와 같은 레벨로 정리 할 수 있음
</div>


## 오라클 Linux v8 설치
- Linux OS 중 Oracle 제공 소프트웨어 기능을 강화한 Oracle Linux OS를 설치한다.

1. OS의 가상 이미지 파일 다운
  - https://yum.oracle.com/oracle-linux-isos.html#Mirrors
  - 위 경로에서 가상 설치 파일을 다운로드 한다.

<img width="1017" alt="스크린샷 2023-05-15 오전 12 36 57" src="https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/937a9237-d6b2-429d-8497-54fcdb949475">

<p>
  
2. OS 부팅 USB 만들기
  - 부팅 USB MANAGER 소프트웨어를 통해 부팅 USB를 만든다.
  - https://balenaetcher.en.softonic.com
    - 부팅 Manager 소프트웨어 설치는 생략
  <br>
<img width="682" alt="스크린샷 2023-05-15 오후 6 33 47" src="https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/f8586f40-5375-4b7e-b2da-74dc769b0edf"><br>
    - 가상 이미지 파일
  <br>
<img width="912" alt="스크린샷 2023-05-14 오후 4 28 51" src="https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/7bbb46f5-3a2a-4ca2-a9d3-f44f073a71fb">
<img width="912" alt="스크린샷 2023-05-14 오후 4 28 55" src="https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/2c9dbc52-00e6-432c-bcf8-5e8c45d8f314">
<img width="912" alt="스크린샷 2023-05-14 오후 4 29 38" src="https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/7b3a4e6f-e904-44c2-b217-6992fe55e56a">
<img width="912" alt="스크린샷 2023-05-14 오후 4 32 28" src="https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/e7a35af7-cde1-4f74-a4d6-0766d8277e34">

<br>

3. OS 설치 PC의 바이오스 설정을 통해 부팅장치 순위 조정
  - 전주대 삼성 컴퓨터 바이오스 진입
    - PC Power On 직후 F2 연타
 
  - [부팅] -> [부팅 순위 정하기] -> [1순위 부팅: (부팅 USB)]
  - 저장 후 재부팅
  
<br>
  
4. Linux Oracle 설치 진행
 ![IMG_3832](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/90173306-1c7c-4147-b5db-4dfd3c2087e2)
![IMG_3834](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/90d0ba9c-8565-406e-b8c5-eec4f2863a5d)
![IMG_3835](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/537c39d9-005a-4a8d-be53-c20a60d0190f)
![IMG_3836](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/780391ce-c2e2-4b7c-9207-9834c1fd2dfd)
![IMG_3837](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/77dbdc1c-81a3-4853-b964-570c5afe0fde)
![IMG_3838](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/dde04b5f-41c6-4c32-bf7e-142405b927f9)
![IMG_3839](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/ce9c3a4b-cc37-415a-9b54-8575705b48a9)
![IMG_3840](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/f695c743-6e7a-4799-8d55-e9cabf06b7ee)
![IMG_3841](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/78c2e5d0-c287-43a5-9e13-22fcb0a79405)
![IMG_3842](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/dcb152f5-1bea-4670-a703-588f46d2e591)
![IMG_3843](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/b08d21fd-3cad-44b4-8522-6484eaa46a27)
  
  <br>
  
  
  
## Oracle DB 설치
0. sudo로 로그인
  
  ~~~ bash
  sudo -s
  ~~~
  
1. Oracle Linux v8 개발자 채널을 활성화
  
  ~~~ bash
  dnf install -y oraclelinux-developer-release-el8
  ~~~

![스크린샷, 2023-05-15 00-44-10](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/1e683a1d-4624-4497-8db0-bcb48afdfbaf)
  
2. Oracle DB 23c Developer preinstall RPM Download
  
  ~~~ bash
  dnf -y install oracle-database-preinstall-23c
  ~~~
  
3. Oracle DB 23c Developer free RPM Download
  
  ~~~ bash
  cd ~
  sudo wget -d https://download.oracle.com/otn-pub/otn_software/db-free/oracle-database-free-23c-1.0-1.el8.x86_64.rpm
  ~~~
  
4. Oracle DB 23c Free install
  
  ~~~ bash
  dnf -y localinstall oracle-database-free-23c-1.0-1.el8.x86_64.rpm
  ~~~
  
5. Oracle DB install 확인

  ~~~ bash
  cd /etc/init.d/
  ls -al
  oracle-free-23c 파일 확인
  ~~~
  
  ![스크린샷, 2023-05-15 00-50-50](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/5b292586-4854-49a2-bee8-67d4b8c77986)

6. PC 재부팅
  
  ~~~ bash
  sudo reboot 
  ~~~
  
7. Oracle DB server 작동 확인
  - Active: inactive (dead) 라면 작동 정지 상태
  
  ~~~ bash
  systemctl status oracle-free-23c
  
  or
  
  /etc/init.d/oracle-free-23c status
  ~~~
  
  ![스크린샷, 2023-05-15 01-01-33](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/43886b77-df77-4d7b-9bee-8221ceef99dc)
  
8. Oracle DB server 작동 시작
  
  ![스크린샷, 2023-05-15 01-01-35](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/b7270d91-dca5-4c3a-8636-eea5676df01c)
  
  ~~~ bash
  systemctl start oracle-free-23c
  
  or
  
  /etc/init.d/oracle-free-23c start
  ~~~

  
## Oracle DB 작동
  1. Oracle DB 설정
    - 오라클 DB의 root 사용자를 생성한다.
      - root 계정의 비밀번호 입력시에 글씨가 표시되지 않는 것이 정상이다.
  
  ~~~ bash
  sudo -s 
  /etc/init.d/oracle-free-23c configure
  ~~~
  
![스크린샷, 2023-05-15 00-51-05](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/15389bda-c16a-409e-93ba-53de9d490828)
![스크린샷, 2023-05-15 00-55-04](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/f1f7c8eb-bf15-4d43-975e-554871c87e05)

  
  2. Oracle DB 환경 변수 설정
    - 이전 버전의 Oracle DB에서는 복잡한 방법으로 환경 변수를 설정해 줘야 했지만 Oracle DB 23c 에서는 Oracle DB에서 환경 변수 설정을 위한 가상환경 기능을 제공한다.
  
  ~~~ bash
  export ORACLE_SID=FREE 
  export ORAENV_ASK=NO 
  . /opt/oracle/product/23c/dbhomeFree/bin/oraenv
  ~~~
  
  ~~~
  (출력)-> ORACLE_SID = [root] ? FREE (입력)
  (출력)-> ORACLE_HOME = [] ? /opt/oracle/product/23c/dbhomeFree
  (출력)-> The Oracle base has been set to /opt/oracle (이렇게 출력되면 완료)
  ~~~
  
  3. Oracle DB 실행
    - 23c의 가상환경 기능의 불편한 점은 Oracle에 접속하는 유저가 한 차례 가상환경을 실행해 주어야 한다는 점이다.
  
  ~~~ bash
  [j211@localhost ~]$ sudo -s
  [root@localhost ~]# su - oracle
  [oracle@localhost ~]$ . /opt/oracle/product/23c/dbhomeFree/bin/oraenv
  ORACLE_SID = [] ? FREE # 한 차례 입력한 SID가 입력되면 가상환경이 셋팅된다.
  the Oracle base has benn set to /opt/oracle 
  ~~~
  
  ![스크린샷, 2023-05-15 01-51-32](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/2a12c162-efc7-4f04-aab0-407e77b2feab)

  ~~~ bash
  [oracle@localhost ~]$ sqlplus "/as sysdba"
  sql > # 성공
  ~~~
    
  - 가상환경이 제대로 실행되지 않는다면 아래와 같은 에러가 발생할 수 있다.
  ![스크린샷, 2023-05-15 01-07-39](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/15a5220a-73c6-4170-8845-485f4c681ae5)

  
  ~~~ bash
  su - oracle
  # 오라클 유저로 변경
  ~~~
  
  - 오라클 사용자로 변경하는 방식은 전용 사용자로 변경함으로써 다른 사용자와의 패키지 설정 중복을 및 환경 변수 설정 충돌을 방지 하기 위하여 진행한다.
  - 이러한 문제점을 고려하지 않는다면 root 및 다른 사용자에서도 oracle DB에 접속할 수 있다.
  
  
  ~~~ bash
  [root@localhost ~]# su - j211 # j211 유저로 변경
  [j211@localhost ~]$ . /opt/oracle/product/23c/dbhomeFree/bin/oraenv
  ORACLE_SID = [] ? FREE
  the Oracle base has been set to /opt/oracle
  [j211@localhost ~]$ sqlplus "/as sysdba"
  sql>
  ~~~
  
  
  4. Oracle DB CharSet
    - 23v의 OracleDB 설정은 한글 출력을 지원하지 않도록 설정되어 있다.
    - 때문에 Linux OS 시스템을 통해 한글이 출력되어야 할 상황에서 ???로 Char 깨짐이 발생한다.
  
  ![스크린샷, 2023-05-15 03-02-24](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/03329e94-de9d-471a-a2fe-2630f49336fa)
<br>
    - 이 때 환경변수를 셋팅해줌으로써 텍스트 포멧 코드를 설정해 줄 수 있다.
    - OracleDB oraenv로는 설정해 줄 수 없어 .bashrc 파일에 코드를 추가해야 한다.
  
  ~~~ bash
  [oracle@localhost ~]$ nano ~/.bashrc
  export NLS_LANG=KOREAN_KOREA.AL32UTF8
  [oracle@localhost ~]$ source ~/.bashrc
  ~~~
  
  - 사용자를 oracle 유저로 한정하지 않고 전체 사용자에게 적용시키고 싶다면 아래의 진행을 따른다.
  
  ~~~bash
  [root@localhost ~]# nano /etc/bashrc
  export NLS_LANG=KOREAN_KOREA.AL32UTF8
  [root@loaclhost ~]# source /etc/bashrc
  ~~~
  
  
  - 이후 한글 문자열 깨짐이 발생하지 않게 된다.
  
  ![스크린샷, 2023-05-15 02-23-29](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/007f2c87-ddda-4e21-aa03-d953146e7258)

  
## Oracle DB 사용
  1. Oracle DB의 유저 생성
    - Oracle DB를 처음 실행했을때 가장 먼저 user-name 및 password의 작성을 요구한다.
  
  ~~~ bash
  user-name: system # default
  password :        # OracleDB configure 시에 정한 pw
  ~~~
  
 ![스크린샷, 2023-05-15 02-23-14](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/b0206bf9-e225-4347-9dcd-d510284d3821)

  
    - 이러한 작업에서 옳은 user-name과 pw를 입력해도 계속해서 오류가 발생할 수 있다.
      - ex) ORA-01017: 사용자명/비밀번호가 부적합, 로그온 할 수 없습니다.
      - ex) ORA-01017: invalid username/password; logon denied.
    - 그럴 때는 oracle-free-23c 서버가 실행되지 않았을 가능성이 높다.
  
  ~~~bash
  [oracle@localhost ~]$ systemctl start oracle-free-23c
  [oracle@localhost ~]$ systemctl status oracle-free-23c # 동작상태 확인
  [oracle@localhost ~]$ sqlplus "/as sysdba"
  ~~~
  
![스크린샷, 2023-05-15 02-23-14](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/a1dda21b-acc0-4125-82f8-243fbe3f2cfc)
  <br>
  
  2. Oracle DB 관리자 모드
    - Oracle DB의 관리자 모드를 위해선 아래와 같이 입력한다.
  
  ~~~ bash
  [oracle@localhost ~]$ sqlplus "/as sysdba"  # Oracle DB 실행시 관리자 모드로
  
  or
  
  sql> conn/as sysdba # Oracle DB 실행 도중 관리자 모드로 변경
  ~~~
  
![스크린샷, 2023-05-15 02-23-29](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/21450fb7-8482-4fe2-afa4-aa94de776279)
<br>
  
  3. Oracle DB 계정 추가
    - 다수의 유저가 DB를 사용한다면 계정을 추가생성 할 수 있어야 한다.
      - 이 때 DB의 공통 계정 분류를 위해 오라클에서는 계정 명 앞에 C##을 붙이도록 권장하고 있다.
      - ex) C##j211
  
  ~~~ sql
  SQL> create user [id] identified by [pw];
  # create user C##j211 identified by 1004;
  ~~~
  
  ![스크린샷, 2023-05-15 02-26-00](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/db9dd2c2-1ce0-4a1f-b9bc-32f7f53ce325)

  <br>
  
  4. Oracle DB 계정 권한 부여
    - 막 생성한 계정은 읽기 기능만을 가지고 있다.
    - 일반적인 DB의 CRUD를 위해 읽기/쓰기 기능을 부여해야 한다.
      - connect : 접속 권한
      - resource : 객체 및 데이터 조작 권한
      - dba
  
  ~~~ sql
  SQL> grant [권한] to [id];
  # grant connect, resource, dba to C##j211;
  ~~~
  
  ![스크린샷, 2023-05-15 02-27-38](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/327fc12d-b723-45a2-9708-b3af38fb16f6)
<br>
  
  5. Oracle DB 변경 내용 커밋 하기
    - Oracle DB는 수정 내용을 즉시 수행하지 않는다
    - 즉시 수행을 위해서 commit 명령을 지시해야 한다.
  
  ~~~ sql
  SQL> commit;
  ~~~
  
![스크린샷, 2023-05-15 02-27-47](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/25a38e77-f50b-4a41-8e7d-cc919a05d2c6)
<br>
  
  6. 계정 확인
    - 이전 과정에서 생성한 user를 조회한다.
  
  ~~~sql
  SQL> select * from all_users;
  ~~~
  
  ![스크린샷, 2023-05-15 02-28-00](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/6e31f7a9-db3f-4f53-966c-b522189263f8)
  ![스크린샷, 2023-05-15 03-02-12](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/6a529254-4771-46ec-a24c-8cde6517c00e)

  <br>
  
  7. 테이블 생성
    - mysql과 같이 테이블을 생성할 수 있다.
  
  ~~~sql
  SQL> create TABLE test
  (
    test_id     NUMBER(4)     NOT NULL,
    test_data   VARCHAR2(10)  
  );
  ~~~
  
  ![스크린샷, 2023-05-15 02-54-34](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/4be5fa62-ac07-4065-8fcf-f6b6ba3b0e3c)

  
  8. 테이블에 데이터 입력
    - mysql과 같이 insert 문을 수행할 수 있다.
    - <b>문자열의 경우 쌍따옴표를 인식할 수 없어 따옴표로 진행해야 한다.</b>
  
  ~~~sql
  SQL> insert into test(test_id, test_data) values(0, 'hello');
  ~~~
  
  ![스크린샷, 2023-05-15 02-56-51](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/7493d06b-3463-4991-af3b-87c1f60a33c7)
  <br>
  
  9. 테이블의 데이터 조회
    - mysql과 같이 select 문을 수행할 수 있다.
  
  ~~~sql
  SQL> select * from test
  ~~~
  
![스크린샷, 2023-05-15 02-57-00](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/4ec00ec3-1f68-4e6c-ab60-c1c3b62cb024)

  
  10. Oracle DB version 확인
    - Oracle DB의 버전을 잊었다면 아래의 코드로 확인 할 수 있다.
  
  ~~~ sql
  SQL> select * from V$VERSION;
  ~~~
  
  ![스크린샷, 2023-05-15 03-17-22](https://github.com/MaugeaLee/LinuxOracleTuto/assets/92789013/0ed6d8a8-3564-485f-ba81-4db8909f813c)
  
  11. Oracle DB 종료
  
  ~~~sql
  SQL> exit
  ~~~
  

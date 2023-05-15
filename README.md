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
  
  ~~~ bash
  sudo -s 
  /etc/init.d/oracle-free-23c configure
  
  root 계정 pw 입력
  ~~~
  
  
  2. Oracle DB 환경 변수 설정
    - 이전 버전의 Oracle DB에서는 복잡한 방법으로 환경 변수를 설정해 줘야 했지만 Oracle DB 23c 에서는 Oracle DB에서 환경 변수 설정을 위한 기능을 제공한다.
  
  ~~~ bash
  
  

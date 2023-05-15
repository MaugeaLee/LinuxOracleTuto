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

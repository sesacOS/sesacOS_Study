## 1. 운영체제 (Operating System, OS)란?

- 컴퓨터 하드웨어 바로 위에 설치되어 사용자+소프트웨어와 하드웨어를 연결하는 소프트웨어 계층

  (사용자+소프트웨어) - (운영체제) - (하드웨어)
<br><br><br><br><br>





## 2. 운영체제의 목적 

- 사용자가 컴퓨터 시스템을 편리하게 사용할 수 있는 환경을 제공

- 컴퓨터 시스템의 자원을 효율적으로 관리 (=자원관리자)
주어진 자원으로 최대한의 성능을 내도록 형평성 있게 분배 한다
<br><br><br><br><br>





## 3. 운영체제의 분류

1. 동시 작업 가능 여부<br>
  • 단일 작업 (single tasking)<br>
    한 번에 하나의 작업만 처리, 한 명령이 끝나야만 다른 명령 수행 가능<br>
    ex) MS-DOS 

  • 다중 작업 (multi tasking)<br>
    동시에 두 개 이상의 작업 처리, 한 명령이 진행중이어도 다른 명령 수행 가능<br>
    ex) UNIX, MS Windows

<br>

2. 사용자의 수<br>
  • 단일 사용자 (single user)<br>
    ex) MS-DOS, MS Windows

  • 다중 사용자 (multi user)<br>
    ex) UNIX, NT server

<br>

3. 처리 방식<br>
  • 시분할 (time sharing)<br>
    여러 작업을 수행할 때 컴퓨터 처리 능력을 일정한 시간 단위로 분할하여 사용<br>
    일괄처리에 비해 짧은 응답시간을 가짐 (ex - UNIX)<br>
    interactive 방식 (바로 반응이 나오는 방식)<br>

  • 실시간 (Realtime OS)<br>
    정해진 시간 안에 반드시 결과가 나오는 것을 보장하는 시스템<br>
    ex) 미사일 제어, 반도체 장비, 로보트 제어, 원자로/공장 제어<br>
          Hard realtime system (경성 실시간 시스템) - 반도체, 미사일, 원자로<br>
          Soft realtime system (연성 실시간 시스템)  - 영화상영

  • 일괄 처리 (batch processing)<br>
    작업 요청을 일정량 모은 후 한번에 처리<br>
    작업이 완전 종료될 때까지 기다려야한다
<br><br><br><br><br>





## 4. 운영체제의 예시

- 유닉스 (UNIX)
   초기에는 대형컴퓨터, 여러 사용자들의 서버를 위한 운영체제
   대부분 C언어로 작성 (기계어와 유사)
   높은 이식성을 가지고 있음
   최소한의 커널 구조(메모리를 적게 차지)를 가져 확장에 용이하다
   소스 코드가 공개되어 있음


- DOS / MS Windows
개인용 컴퓨터를 위해 만들어짐

- DOS
단일 사용자용 운영체제
주기억장치의 용량이 640KB에 불과

- MS Windows
다중 작업용 GUI 기반 운영 체제
풍부한 소프트웨어를 지원한다
<br><br><br><br><br>





## 5.운영체제의 구조

- CPU<br>
CPU 스케줄링<br>
CPU를 누구에게 줄지 정하는 것


- Memory<br>
메모리 관리<br>
프로그램이 원활하게 실행되기 위해서 어느정도 수준 이상의 메모리는 주는 것


- Disk<br>
파일관리<br>
디스크 스케줄링

-  I/O device<br>
입출력 관리<br>
각각의 입출력 장치와 컴퓨터 간에 어떻게 정보를 주고 받게 할지

- etc<br>
프로세스 관리
<br><br><br><br><br>





<hr>
<a href="http://www.kocw.net/home/search/kemView.do?kemId=1046323">출처 : 이화여자대학교 반효경 교수님 운영체제 수업 </a>



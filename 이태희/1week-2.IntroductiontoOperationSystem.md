Introduction on Operating Systems

1. 운영체제란 무엇인가
2. 운영체제의 목적
3. 운영체제의 분류
4. 운영체제의 예
5. 운영체제의 구조

---

### 1. 운영체제란 무엇인가

컴퓨터 하드웨어 바로 위에 설치되어 사용자 및 다른 모든 소프트웨어와 하드웨어를 연결하는 소프트웨어 계층.

     ● 협의의 운영체제(커널)
         운영체제의 핵심 부분으로 메모리에 상주하는 부분

     ● 광의의 운영체제
         커널 뿐 아니라 각종 주변 시스템 유틸리티를 포함한 개념

<p align="center"> <img src=https://velog.velcdn.com/images%2Fsunil1369%2Fpost%2F51b2b179-6fcf-4df8-9f33-f9a7c15abdff%2Fimage.png width =300>

---

### 2. 운영 체제의 목적

###### 컴퓨터 시스템의 <u>자원을 효율적으로 관리</u> ★

    § 프로세서, 기억장치, 입출력 장치 등의 효율적 관리
     ┖  사용자간의 형평성 있는 자원 분배
     ┖  주어진 자원으로 최대한의 성능을 내도록
    § 사용자 및 운영체제 자신의 보호
    § 프로세스, 파일, 메시지 등을 관리
    § 컴퓨터 시스템을 편리하게 사용할 수 있는 환경을 제공
     ┖  운영체제는 동시 사용자/프로그램들이 각각 독자적 컴퓨터에서 수행되는 것 같은 환상을 제공
     ┖  하드웨어를 직접 다루는 복잡한 부분을 운영체제가 대행

---

### 3. 운영체제의 분류

    <고려할 사항>
       1. 동시 작업 가능 여부
       2. (지원해주는)사용자의 수
       3. 처리방식

### 1 동시작업 가능 여부

● <U> 단일 작업(single tasking) </U> : 한 번에 하나의 작업만 처리
ex) MS-DOS 프롬프트 상에서는 한 명령의 수행을 끝내기 전에 다른 명령을 수행시킬 수 없음.  
 ● <U>다중 작업(Multi tasking)</U> : 동시에 두 개 이상의 작업처리
ex) UNIX, MS Windows 등에서는 한 명령의 수행이 끝나기 전에 다른 명령이나 프로그램을 수행할 수 있음

### 2. (지원해주는) 사용자의 수

● <U>단일 사용자(single user)</U> ex.MS-DOS, MS Windows  
 ● <U>다중 사용자(multi user)</U> ex.UNIX , NT server

### 3.처리 방식

●<U> 일괄 처리(batch processing) </U> (☞ OMR카드 모아서 전산소에 제출)
작업 요청의 일정량 모아서 한꺼번에 처리
작업이 완전 종료될 떄까지 기다려야 함
ex. 초기 Punch Card 처리 시스템

● <U>시분할(time sharing) </U> ★
여러 작업을 수행할 떄 컴퓨터 처리 능력을 일정한 시간 단위로 분할하여 사용
일괄 처리 시스템에 비해 짧은 응답 시간을 가짐 ex)UNIX
interactive한 방식

● <U>실시간(Realtime OS) </U> ★
정해진 시가 안에 어떠한 일이 반드시 종료됨이 보장되어야 하는 실시간 시스템을 위한 OS
ex)원자로/공장 제어, 미사일 제어, 반도체 장비, 로보트 제어

● <U> 실시간 시스템의 개념 확장 </U>  
 Hard realtime system(경성 실시간 시스템)
Soft realtime system(연성 실시간 시스템)

####~ 몇 가지 용어 ~

1. Multitasking
2. Multiprogramming
3. Time sharing
4. Multiprocess

> 구분 : 위의 용어들은 컴퓨터에서 여러 작업을 동시에 숭행하는 것을 뜻한다.
> Multiprogramming은 여러 프로그램이 메모리에 올라가 있음을 강조
> Time Sharing은 CPU의 시간을 분할하여 나눈어 쓴다는 의미를 강조

Multiprocessor : 하나의 컴퓨터에 CPU(processor)가 여러 개 붙어 있음을 의미

---

### 4. 운영체제의 예 (유닉스계역, 윈도우계열)

**● 유닉스(UNIX)** - 코드의 대부분을 C언어로 작성 - 높은 이식성 - 최소한의 커널 구조 - 복잡한 시스템에 맞게 확장 용이 - 소스 코드 공개 - 프로그램 개발에 용이 - 다양한 버전
System V, FreeBSD, SunOS, Solaris, Linux  
**● DOS(Dist Operating System)** - Ms사에서 1981년 IBM-PC를 위해 개발 - 단일 사용자용 운영체제, 메모리 관리 능력의 한계(주 기억 장치 :640KB)  
**● MS Windows** - MS사의 다중 작업용 GUI 기반 운영 체제 - Plug and Play, 네트워크 환경 강화 - DOS용 응용 프로그램과 호환성 제공 - 불안정성 - 풍부한 지원 소프트웨어  
**● Handheld device를 위한 OS** - palmOS, Pocket PC(WinCE), Tiny OS

---

### 5. 운영체제의 구조

<p align="center">  <img src=https://velog.velcdn.com/images%2Fsunil1369%2Fpost%2F531c349e-bee1-4e00-891d-8e08218dea07%2Fimage.png width=300>

● CPU = "누구한테 CPU를 줄까?", [CPU 스케쥴링]  
● MEMORY = "한정된 메몸리를 어떻게 쪼개어 쓰지?, [메모리 관리]  
● DISK = "디스크에 파일을 어떻게 보관하지", [파일 관리]  
● I/O device = "각기 다른 입출력장치와 컴퓨터 간에 어떻게 정보를 주고 받게 하지", [입출력 관리]

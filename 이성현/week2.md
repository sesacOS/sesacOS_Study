### 컴퓨터 시스템 구조

<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fk.kakaocdn.net%2Fdn%2F0AvAi%2FbtrQptLgccS%2FFpm39G97UM4V6UpalI3KX0%2Fimg.png" width="500" height="500"/>

<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fk.kakaocdn.net%2Fdn%2FSG9wE%2FbtrQmhykhZQ%2FT3sBP7viIWnbfrn9a7hl30%2Fimg.png" width="500" height="500"/>

- 메모리는 CPU의 작업공간 이다.
- Disk의 속도가 CPU보다 현저하게 느리기 때문에 device controller(CPU)에서 기능을 관장한다.
- CPU에는 register가 존재한다.
- mode bit는 CPU를 운영체제가 가지고 있는지, 사용자 프로그램이 가지고 있는지 확인해 준다.
- interrupt line은 CPU가 Memory에 있는 프로그램만 실행하기 때문에, 동시에 I/O device에서 실행된 일을 할 수 있도록 도와준다.

Q. CPU가 Disk에서 보내온 신호는 어떻게 읽을까?

- Disk의 device controller에서 신호를 받아서 CPU를 돌린다.

Q. 만약 Memory에서 무한 루프를 돌리는 프로그램을 실행하면 어떻게 될까?

- CPU가 다른 프로그램에 넘어가지 못해서 timesharing을 구현할 수 없게된다.
- 그래서 컴퓨터 안에서는 timer라는 hardware를 구현해 놓았다.
- Memory가 CPU를 독점하는것을 막는 역할을 한다.
- 처음 컴퓨터를 키면 OS가 CPU를 독점하다가 timer에 특정 값을 세팅한 다음에 다른 프로그램이 실행되면 CPU를 넘겨준다.
- 그러면 timer에 할당된 시간만큼 CPU를 사용하고, 세팅된시간이 끝나면 timer가 CPU가 interrupt를 실행한다.
- 그리고 CPU 사용이 중단된다.

Q. 운영체제가 CPU를 얻게 되면 어떻게 되는가?

- timer에 세팅된 시간에 따라 CPU를 쓰다가 시간이 만료되면, timer interrupt가 들어오고, 다음 프로그램이 실행된다.

### Mode bit

- 사용자 프로그램의 잘못된 수행으로 다른 프로그램 및 운영체제에 피해가 가지 않도록 하기 위한 보호 장치가 필요하다.
- Mode bit을 통해 하드웨어적으로 두 가지 모드의 operation을 지원한다.
- 1 사용자 모드: 사용자 프로그램 수행, 2 모니터 모드: OS 코드 수행
- interrupt나 Exception 발생시 하드웨어가 mode bit을 0으로 바꾼다.
- 사용자 프로그램에게 CPU를 넘기기 전에 mode bit을 1로 세팅한다.

### Timer

- 정해진 시간이 흐른 뒤에 운영체제에게 제어권이 넘어가도록 인터럽트를 발생시킨다.
- 타이머는 매 클럭 틱 때마다 1씩 감소한다.
- 타이머 값이 0이 되면 타이머 인터럽트가 발생한다.
- CPU를 특정 프로그램이 독점하는 것으로부터 보호한다.

- 타이머는 time sharing을 구현하기 위해서 널리 사용된다.
- 타이머는 현재 시간을 계산하기 위해서도 사용된다.

### Device Controller

- 해당 I/O 장치유형을 관리하는 일종의 작은 CPU이다.
- 제어 정보를 위해서 control register, status register를 가진다.
- local buffer를 가진다. (일종의 data register)
- Device controller는 I/O가 끝났을 경우에 interrupt로 CPU에 그 사실을 알린다.

### 입출력(I/O)의 수행

- 모든 입출력 명령은 특권 명령이다.
- I/O의 요청은 trap(소프트웨어 인터럽트)를 이용한다.

### 동기식 입출력과 비동기식 입출력

- 두 경우 모두 I/O의 완료는 인터럽트로 알려준다.

#### 동기식 입출력 (synchronous I/O)

- I/O 요청 후 입출력 작업이 완료된 후에야 제어가 사용자 프로그램에 넘어간다.

#### 비동기식 입출력 (asynchronous I/O)

- I/O가 시작된 후 입출력 작업이 끝나기를 기다리지 않고 제어가 사용자 프로그램에 즉시 넘어간다.

### 시스템콜(System Call)

- 사용자 프로그램이 운영체제의 서비스를 받기 위해 커널 함수를 호출하는 것이다.
- 사용자 프로그램이 운영체제 코드를 수행하는 것이 불가능하다.
- 사용자 프로그램이 interrupt line을 세팅하고, CPU 제어권이 OS에 넘어가기 때문에, 부탁한 일을 OS가 할 수 있게 된다.

### 인터럽트(Interrupt)

- 인터럽트 당한 시점의 레지스터와 program counter를 save한 후 CPU의 제어를 인터럽트 처리 루틴에 넘긴다.

### DMA(Direct Memory Access)

- 원래는 메모리를 접근하는 것이 CPU이지만, DMA controller도 메모리에 접근할 수 있다.
- 빠른 입출력 장치를 메모리에 가까운 속도로 처리하기 위해서 사용한다.
- CPU의 중재 없이 device controller가 device의 buffer storage의 내용을 메모리에 block 단위로 직접 전송한다.
- 바이트 단위가 아니라 block 단위로 인터럽트를 발생시킨다.

- CPU와 DMA conroller가 동시에 메모리에 접근하는 것을 방지하기 위해서 memory controlelr가 존재한다.
- DMA를 왜 달아 놨을까?
  - I/O 장치가 CPU를 자주 interrupt하는 것을 방지하기 위해서이다.
  - I/O 장치가 실행되면 버퍼가 메모리에 쌓이면, DMA controller가 CPU에게 interrupt를 1번 실행한다.
  - 그래서 메모리에 I/O에서 실행한 내용이 다 올라왔다고 DMA controller가 CPU에게 알려준다.
  - 그러면 CPU가 실행 중간에 interrupt 당하는 빈도가 줄어들어서 CPU를 효율적으로 사용할 수 있다.

### 서로 다른 입출력 명령어

-

### 저장장치 계층 구조

Primary(Executable) Register<br>
Primary(Executable) Cache Memory<br>
Primary(Executable) Main Memory<br>
Secondary Magnetic Disk<br>
Secondary Optical Disk<br>
Secondary Magnetic Tape<br>

- 위로 갈수록 속도가 빠르고, 가격이 비싸다, 용량이 적다, 휘발성이 높다.
- CPU가 직접 처리 못하는 것은 Secondary 영역에 있다.
- 캐싱은 재사용을 목적으로 한다.

### 프로그램의 실행(메모리 load)

- File system에 있는 실행파일 A, B가 Pysical memory에 커널영역, 프로세스 A, B로 올라간다.
- File system에 있는 실행파일 A, B가 Virtual memory에 각각 Kernel Adress space, Address space[stack, data, code]를 구성하여 Physical memory에 올라간다.
- 모든 프로그램은 독자적인 주소를 가지고 있다.

### 커널 주소 공간의 내용

#### code

- 커널 코드
- 시스템콜, 인터럽트 처리 코드
- 자원 관리를 위한 코드
- 편리한 서비스 제공을 위한 코드

#### data

- Process A(PCB), Process B(PCB), CPU, mem, disk
- PCB는 process control block의 약자이다.
- 프로그램마다 PCB가 1개씩 있고 프로그램을 관리한다.

#### stack

- Process A의 커널 스택
- Process B의 커널 스택

### 사용자 프로그램이 사용하는 함수

- 사용자 정의 함수 => 프로세스 A의 Adress space에서 code안에 들어간다.
- 라이브러리 함수 => 프로세스 A의 Adress space에서 code안에 들어간다.
- 커널 함수 => Kernel Address space의 code에 들어간다.

### 프로그램의 실행

<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fk.kakaocdn.net%2Fdn%2FcEtTns%2FbtrQn72ZR42%2FKqlNP3lHOK1lZJXY2RRff0%2Fimg.png" width="500" height="500"/>

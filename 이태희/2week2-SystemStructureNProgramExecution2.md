🟧운영체제강의 - 2차시  
2️⃣👉System Structure & Program Execution 2

- 컴퓨터 시스템 구조,[전강의eview 00:00]
- 인터럽트(Interrupt),[전강의review 04:40][🤗10:21]
- 동기식 입출력과 비동기식 입출력,[14:24]
- 시스템콜(System Call),[전강의review 09:00]
- DMA(Direct Memory Access), [26:15]
- 서로 다른 입출력 명령어, [30:00]
- 저장장치 계층 구조,[33:02]
- 프로그램의 실행(메모리 load),[39:15]
- 커널 주소 공간의 내용,[46:06]
- 사용자 프로그램이 사용하는 함수,[50:10]
- 프로그램의 실행[53:15] [54:40]

---

<p align="center"> 
<img src=https://saegeullee.github.io/static/9794b8622d268f3c45f639f843a6bc89/d945d/os-computer-system.webp width=800 >

---

🟪[07:24]  
mode bit = 0, cpu가 실행할 수 있는 모든 기계어 집합을 다 실행 가능 //운영체제가 cpu 가지고 있을 때
mode bit = 1, 한정된 기계어, instruction들만 수행가능 // 사용자 프로그램이 cpu를 가지고 있을 때

🟪I/O 작업을 하려고 운영체제에게 요청을 하려고 / 운영체제의 주소영역으로 점프를 해야하는데 / 그쪽으로 쩜프를 하려고 하는데 mode bit 이 1이어서 점프를 못하여 , / 사용자 프로그램이 운영체제에게 서비스를 요청할 때에는 '시스템 콜'이라는 것을 한다  
🟧시스템 콜 : 운영체제 함수를 호출할 때에는 의도적으로 Interrupt line을 세팅을 한다. [CPU의 제어권이 사용자의 프로그램으로 넘어가게 됨.]

🟪🤗중요!🤗[10:21] INTERRUPT 종류들  
INTERRUPT(하드웨어 인터럽트)  
TRAP(소프트웨어 인터럽트)∋ExceptionI (프로그램이 오류를 범한 경우), System Call(프로그램이 커널 함수를 호출하는 경우)

🟪[13:04]Timer가 인터럽트를 걸수도 있다~ex)

mode bit🆚timer  
🟨mode bit은 보안에 어긋나는 것을 막기 위한 것  
🟨timer는 사용자 프로그램이 쓸데 없이 cpu 낭비하는 것을 막기 위한 것 (제한시간을 두고 쓸데없는 짓을 하면 cpu를 뻇어옴)

🟪[14:24] 동기식 입출력 🆚 비동기식 입출력
요약 [18:20]  
동기식 입출력 : I/O 요청후, 입출력 작업이 완료된 후에야 제어가 사용자 프로그램이 다음일을 할 수 있음.  
비동기식 입출력 : I/O하라고 던져놓고, 바로 CPU넘겨와서 다른 일을 하는 것.  
[19:19]도해설명  
🟧 두 경우 모두 I/O의 완료는 인터럽트로 알려줌

🟪
[26:15] DMA(Direct Memory Access) :CPU가 효율적으로 작업하도록 도와주는 장치 & 메모리를 접근할수 있는 장치
메모리를 접근할 수 있는 장치는 CPU밖에 없어요.

🟪I/O장치들이 CPU와 교신할 필요성이 있을 때에는 interrupt를 걸어주고 , 여러가지 I/O 장치들이 (키보드, 모니터, 마우스 등등) 이 한꺼번에 인터럽트를 CPU에게 요청하게 되면 CPU가 효율적으로 동작하지 못하게 되므로 DMA Controller를 하나 붙여놓아서 DMA가 직접 Memory에 접근 할 수 있도록 함.

작은 일든은 BUFFER에서 모아서?

🟪[31:50]
{좌측 그림}  
메모리에 접근하는 명령어(instruction) 따로 있고  
i/o 명령어(instruction) 따로 있고  
{우측 그림}  
 ☞ Memory Mapped I/O라고 부름
메모리 주소에 있는 명령어(instruction)

---

저장장치 계층 구조

<p align="center"> 
<img src=https://oopy.lazyrockets.com/api/v2/notion/image?src=https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fa50b213e-c3f9-4c43-add1-bf54251fd95b%2FUntitled.png&blockId=69a133c6-0931-4682-a854-6cc6900b3917 width=800 >

🟪저장장치 계층 구조  
Primary - CPU가 직접 접근 가능  
Secondary - 먼저 주기억장치에 적재되어야 CPU가 접근 가능

🟪
{커널 코드 부분}  
인터럽트가 들어오면 CPU를 얻게 되는데, 인터럽트가 올때마다 CPU를 어떻게 처리해야하는지, 이것이 커널 코드에 함수형태로 구현이 되어있을 거에요.

{커널 데이터 부분}  
운영체제가 사용하는 여러가지 자료구조들이 정의 되어있다.
'관리'하기 위한 자료구조들(운영체제의 커널에) = PCB

{커널 스택 부분}  
운영체제도 함수구조로 코드가 짜여져 있기 때문에, 함수를 호출하거나 리턴 할 때, STACK영역을 사용하게 됩니다.

🟪
[50:10]  
사용자 프로그램이 사용하는 함수 : 모든 프로그램들이 함수형태로 짜여져 있다.
사용자 정의 함수 : 자신의 프로그램에서 정의한 함수
라이브러리 함수 : 기능이 유용해서 이미 만들어 놓은 함수, 가져다 쓰기만 하면 된다.
커널함수 : 운영체제 안에서 정의된 함수 , 시스템 콜을 통해서 호출, 사용 가능.

🟪🤗중요!!!!🤗
[53:15]프로그램의 실행.
메모리 주소를 바꾼다, 즉 점프를 한다는 것은 ,물리적인 차원에서의 점프가 아니라, 논리적인 메모리 상에서의 Virtual memory에서의 점프. +그래서 커널의 함수를 호출을 할 떄에는 '시스템 콜'을 통해서, 인터럽트 라인을 셋팅을 해서, CPU 제어권이 Kernel Address space로 넘어가게 해서 커널 함수를 실행하게 되는 것이죠.

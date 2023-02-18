## System Structure
- Computer
    - CPU
    - Memory
    
- IO Device
    - 디스크
    - 키보드
    - 프린터
    - 모니터
    
### Computer
📍 I/O로 명령

- **CPU**: memory와 local buffer 접근 가능
    - mode bit: 시스템에서 사용하는 것이 운영체제인지(0) 사용자인지(1) 구분
    
    	** 필요 이유:  사용자 프로그램의 잘못된 실행으로 인한 보안 오류 방지
    - interrupt line: 운영체제에게 CPU 제어권을 넘겨줌
    - register
-  **timer**: 특정 프로그램의 제어권 독점을 막기 위해 일정 시간이 지나면 제어권 반납 (time sharing)   
- **Memory**: CPU에만 접근 가능
    - memory controller: memory 교통정리
- **DMA Controller**

### I/O Device
📍 컴퓨터에서 온 명령 처리, 출력
📍 각 디바이스마다 device controller와 local buffer를 가지고 있음
** device controller: I/O 장치 관리가 목적인 작은 하드웨어
- Disk

- 키보드
- 프린터
- 모니터

### 인터럽트
현대의 OS는 인터럽트에 의해 구동된다!!
- Interrupt(하드웨어 인터럽트)
- Trap(소프트웨어 인터럽트)
    - exception: 프로그램이 오류를 범한 경우
    - 시스템 콜(System Call): 사용자 프로그램이 운영체제에게 명령(함수)를 호출하는 것

- 인터럽트 벡터
: 각 인터럽트 종류들이 어디에 명령을 생성해야하는지에 대한 주소를 가짐
- 인터럽트 처리 루틴
: 여러 인터럽트 종류가 어떤 루틴을 가져야하는지 정의된 함수

---

### 내가 이해한 구조
ex. 
??: CPU야 디스크 어쩌고를 읽어와라
cpu: 디스크야 너꺼 읽어와라
disk: 컨트롤러야 내꺼 읽어와라
Introduction to Operating System

운영 체제(Operating System, OS)

컴퓨터 하드웨어 바로 위에 설치되어 사용자 및 다른 모든 소프트웨어와 하드웨어를 연결하는 소프트웨어 계층

​

협의의 운영체제(커널)

운영체제의 핵심 부분으로 메모리에 상주하는 부분

​

광의의 운영체제

커널 뿐 아니라 각종 주변 시스템 유틸리티를 포함한 개념

​

운영 체제의 목적

1. 컴퓨터 시스템을 편리하게 사용할 수 있는 환경을 제공

 운영체제는 동시 사용자/프로그램들이 각각 도자적 컴퓨터에서 수행되는 것 같은 환상을 제공

 하트웨어를 직접 다루는 복잡한 부분을 운영체제가 대행

​

2. 컴퓨터 시스템의 자원을 효율적으로 관리

프로세서, 기억장치, 입출력 장치 등의 효율적 관리 

 - 사용자간의 형평성 있는 자원 분배

 - 주어진 자원으로 최대한 성능을 내도록

사용자 및 운영체제 자신의 보호

프로세스 파일 , 메시지 등을 관리

​

CPU는 실행중인 프로그램에게 짧은 시간씩 번갈아 할당

메모리는 실행중인 프로그램들에 공간을 적절히 분배

​

운영 체제의 분류

1. 동시 작업 가능 여부

2. 사용자의 수

3. 처리 방식

​

1. 운영체제의 분류(동시 작업 가능 여부)

단일 작업(single tasking)

한 번에 하나의 작업만 처리 (한 명령의 수행을 끝내기 전에 다른 명령을 수행시킬 수 없음)

​

다중 작업(multi tasking)

동시에 두 개 이상의 작업 처리(한 명령의 수행이 끝나기 전에 다른 명령이나 프로그램 수행 가능)

​

2. 운영체제의 분류(사용자의 수)

단일 사용자

ex) MS-DOS, MS Windows

​

다중 사용자

ex) UNIX, NT server

컴퓨터 한대를 여러 사용자가 접속해서 사용할 수 있음

​

3. 운영체제의 분류(처리방식)

실시간(Realtime OS)

정해진 시간 안에 어떠한 일이 반드시 종료됨이 보장되어야하는 실시간 시스템을 위한 OS

실시간 시스템의 개념 확장 

ex.원자로/공장 제어, 미사일 제어, 반도체 장비, 로보트 제어

Hard realtime system(경성 실시간 시스템)

Soft realtime system(연성 실시간 시스템)

​

시분할(time sharing)

- 여러 작업을 수행할 때 컴퓨터 처리 능력을 일정한 시간 단위로 분할하여 사용

- 일관 처리 시스템에 비해 짧은 응답 시간을 가짐

- interactive한 방식(상호적)

(일반적으로 사용하는 컴퓨터의 방식)

​

일괄처리(batch processing)

- 작업 요청의 일정량 모아서 한꺼번에 처리

- 작업이 완전 종료될 때까지 기다려야 함

​

용어정리

multitasking

하나의 프로그램이 끝나기 전에 다른 프로그램이 다른 컴퓨터에서 실행 가능한 경우

multiprogramming 

여러 프로그램이 메모리에 올라가 있음

Time sharing

CPU의 시간을 분할하여 나누어 쓴다는 의미

multiprocessor

하나의 컴퓨터에 CPU가 여러 개 붙어 있음을 의미

​

운영 체제의 예

유닉스(UNIX)

대형 컴퓨터를 위해 만들어진 운영체제

코드의 대부분을 C언어로 작성

높은 이식성

최소한의 커널 구조

복잡한 시스템에 맞게 확장 용이

소스 코드 공개

프로그램 개발에 용이

다양한 버전 - System V, FreeBSD, SunOS, Solaris

​

DOS(Disk Operating System)

MS사에서 1981년 IBM-PC를 위해 개발

단일 사용자용 운영체제, 메모리 관리 능력의 한계(주 기억장치 : 640KB)

​

MS Windows

MS사의 다중 작업용 GUI기반 운영 체제

Plug and Play, 네트워크 환경 강화

DOS용 응용 프로그램과 호환성 제공

불안정성

풍부한 지원 소프트웨어

​

운영 체제의 구조

CPU 스케줄링 : 어디에 CPU를 줄까

파일 관리 : 디스크에 파일을 어떻게 보관할까

메모리 관리 : 한정된 메모리를 어떻게 쪼개어 줄까

입출력 관리 : 각기 다른 입출력 장치와 컴퓨터 간에 어떻게 정보를 주고 받게 될까
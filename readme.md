<h1> [운영체제] </h1> 
  -운영체제란 컴퓨터 시스템과 사용자 사이에서 인터페이스 역할을 함 <br>
  -한정된 자원을 더 효율적으로 관리하여 시스템의 성능을 향상시키는 소프트웨어 <br>
  -운영체제도 하나의 프로그램임 + 운영체제는 하드디크스안에 있음 <br> <br>

  *인터페이스 : 2개 이상의 장치나 소프트웨어 사이에서 정보나 신호를 주고받을 때의 만나서 이어주는 부분 <br>

<h2> 운영체제의 목적 </h2>
  -처리량 향상 : 단위 시간동안 처리하는 작업량을 늘림 <br>
  -응답 시간 단축 : 작업을 맡긴 후 결과가 나올 때까지 소요되는 시간을 단축 <br>
  -유용성 증대 : 자원을 효율적으로 관리하여 제공가능한 자원의 양을 증대 <br>
  -신뢰성 향상 : 실패없이 안정적으로 수행할 수 있도록 하므로 신뢰성 증가 <br>

<h2> 운영체제의 구동 </h2>
  1단계 - 전원공급  <br>
  2단계 - BIOS 프로그램 실행 <br>
  3단계 - BIST 기능 실행 <br>
  4단계 - 주기억장치에 부트 로더 적재 <br>
  5단계 - 부트 로더가 운영체제에 적재 <br>
  6단계 - 운영체제 구동 <br> <br>
 
  *BIOS 프로그램 : Basic Input Output System Program의 약어로 기본 입출력장치들이 문제가 없는지 점검하는 것 <br>
  *BIST : BIOS내장 기능, Built In Self Test의 약어로 내장장치들이 문제 없는지 스스로 테스트해보는 것 <br>
  *Boot Loader : ROM에 위치 + ROM에서 RAM으로 옮겨진 후, HDD에 있는 OS를 RAM에 가져옴 <br> 
  
<h2> 운영체제의 역할 </h2>
  -자원과 UI를 관리 <br>
  -프로세스 관리 <br>
  -기억장치 관리 <br>
  -입출력장치 관리 <br>
  -정보 관리 <br> <br>
   
  *프로세스 : 사용중인 프로그램을 가리킴 <br>
  *UI : User Interface의 약어로, 사용자 편의성을 가리킴 <br>
   
<h2> 운영체제의 분류 </h2> 
  -일괄처리시스템(Batct System) : 자료들을 즉시 처리하지 않고, 일정기간이나 일정량을 모았다가 한꺼번에 묶어서 처리함 <br>
  -다중프로그래밍시스템(Multi Programming) : 하나의 CPU에 다수의 프로그래밍을 적재하여 번갈아 가며 사용하며 처리함 <br>
  -다중처리시스템(Multi processor) : 2개 이상의 CPU를 탑재하여 동시에 처리함 <br>
  -시분할 시스템(Time Sharing System) : 일정한 시간을 나누어 여러명이 번갈아 가며 CPU를 사용 <br> 
  -실시간 시스템(Real Time System) : 입력된 데이터를 즉시 처리함, 시간이 되게 중요한 응용프로그래밍에 사용 <br>
  -분산 처리 시스템(Distributed processing System) : 네트워크를 통해 연결된 다수의 컴퓨터에 분산하여 처리함 <br> <br>
     
  *다중프로그래밍시스템은 한 프로그램이 CPU를 사용하다 입출력장치를 사용하게 되었을 때, <br>
  다른 프로그램이 그시간에 CPU를 사용하는 방식으로 번갈아 가며 사용하는 것이고, <br>
  시분할시스템은 1억분의1초 단위로 시간을 나눠 번갈아 가며 사용하는 방식이다 <br>

<h2> 범용 운영체제 </h2>
  -유닉스 : 95%이상 C언어로 작성됨, 이식성이 좋음, 계층적 파일시스템, 다중 작업과 다중 사용자 지원 <br>
  -리눅스 : 공개형 오픈 소스 운영체제, 다중 작업과 다중 사용자 지원, 하나의 컴퓨터로 여러 프로그램 실행가능, 신뢰성이 좋음, 네트워크체제로 활용가능, 다양한 베포판이 존재 <br>
  -윈도우 : Ms-DOS에 다중작업기능과 GUI환경을 추가하여 만듬 <br>
  -맥OS : 애플의 자체 코드기반의 클래식 시리즈와 유닉스계열의 운영체제인 NEXTSTEP기반의 맥OS X로 나뉨 <br>

<h1> [프로세스] </h1>
  -실행중인 프로그램을 프로세스라고 한다. <br> 
  -프로그램이 주기억장치에 적재되어 처리를 시작할 때 프로세스라는 활동적 개체가 됨 <br> <br>
 
   *프로그램은 수동적 <br>
   *프로세스는 능동적 <br>

<h2> 프로세스 상태 </h2>
  -초기상태 (new state) : 프로세스 생성 <br>
  -준비상태 (ready state) : CPU를 할당받기 위해 기다리는 상태 <br>
  -실행상태 (running state) : 프로세스가 CPU를 차지하고 작업을 수행하는 상태 <br>
  -대기상태 (blocked state) : 실행상태에서 입출력처리같은 사건이 발생하면 CPU사용을 멈추고 CPU를 양도한 다음, 입출력이 완료될때까지 대기 큐에서 기다기는 상태 <br>
  -종료상태 (exit state) : 프로세스가 실행을 마친 상태 <br>

  *준비상태인 프로세스중 하나를 골라 CPU를 할당하는 것을 '디스패치(Dispatch)'라고함 <br>
  *프로세스의 준비-실행-대기가 반복되는 구간을 'CPU 싸이클(CPU Cycle)'이라고 함 <br>
  
<h2> 프로세스 제어 블록 </h2>
  -프로세스에 대한 정보를 운영체제에 제공하는 자료구조 <br>
  -프로세스가 생성될 때 만들어 졌다가 프로세스가 실행을 마치면 삭제됨 <br>
  
<h2> 병행 프로세스 </h2>
  -2개 이상의 프로세스가 동시에 실행되는 것을 병행 프로세스라고 한다 <br>
  -독립적으로 실행되면 독립적인 프로세스이고, 다른 프로세스에 영향을 주거나 받으면 협력적인 프로세스이다 <br>
  -동기화 : 병행 프로세스중 데이터불일치 상태에서 이상한 결과가 나오지 않게 일관성을 유지하려 처리 순서를 결정하는 것 <br>
  -임계 구역 : 병행 프로세스중 공유자원을 읽고 수정하는 등의 작업을 실행하는 구역 <br>
  -상호 배제 : 병행 프로세스중 하나의 프로세스가 공유 자원을 사용하는 동안에는 다른 프로세스가 사용하지 못하게 하는 것 <br>
  
<h2> 교착 상태 </h2>
  -하나 이상의 프로세스가 절대 일어나지 않을 특성 사건을 기다리고 있는 상태로 Dead Lock이라고도 불린다 <br>
  

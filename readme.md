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
  다른 프로그램이 그 시간에 CPU를 사용하는 방식으로 번갈아 가며 사용하는 것이고, <br>
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
  
<h1> [CPU 스케줄링] </h1>
  -CPU를 언제, 어느 프로세스에게 할당할 것인지 결정하는 작업 <br>
  
<h2> CPU 스케줄링의 목적 </h2>
  -스케줄링의 공정성 <br>
  -처리량 최대화 <br>
  -응답 시간 최소화 <br>
  -반환 시간 예측 가능 <br>
  -자원의 균형적인 사용 <br>
  -응답 시간과 자원 활용도의 조화 <br>
  -프로세스의 실행의 무한 연기 배제 <br>
  -우선순위에 따른 실행 보장 <br>
  -시스템의 과도한 부하 방지 <br>
  
<h2> CPU 스케줄링 기법 </h2>
  -FCFS (First Come First Served) - 프로세스 순서대로 CPU할당 <br> 
  -라운드 로빈 (Round Robin) - FCFS + 사용시간지정 <br>
  -SJF (Short Job First) - 실행시간이 짧은 순서부터 할당 <br>
  -SRT (Short Remaining Time) - 잔여 싱핼 시간을 비교하여 짧은 순서부터 할당 <br>
  -HRN (Highest Responese ratio Next) - 응답률을 계산하여 높은 순서부터 할당 <br>
  -우선순위 - 운선수위를 부여하여 높은 순서부터 할당 <br>
  -MLQ(Multi Level Queue) - 작업 특성에 따라 각 각 별도의 스케줄링 기법 <br>
  -MFQ(Multi level Feedback Queue) - 입출력 위주와 연산 위주 프로세스의 특성에 따라 CPU사용 시간을 다르게 부여하는 선점 방식의 스케줄링 기법 <br> <br>
  
  *응답률 = (대기 시간 + 실행 시간) / 실행 시간

<h2> CPU 스케줄링 기법의 성능 기준 </h2>
  -CPU활용률 <br>
  -처리율 <br>
  -반환 시간 <br>
  -대기 시간 <br>
  -응답 시간 <br>

<h1> [기억장치 관리] </h1>
  -주기억장치에서 사용 중인 공간과 사용하지 않는 공간을 파악하여 프로세스가 요구할 때 공간을 할당하고 사용이 끝나면 회수하는 작업을 말한다 <br>

<h2> 단일 프로그래밍 기법 </h2>
  -초기에 쓰인 단순한 방식으로 운영체제와 하나의 사용자 프로그램만 주기억 장치에 적재하는 기법 
  -빈공간이 많아 자원낭비가 심함 <br>
  -주기억장치의 용향보다 작은 프로그램만 실행할 수 있다 <br>

<h2> 다중 프로그래밍 기법 </h2>
  -주기억장치에 여러 개의 작업을 적재시킨 후 CPU가 작업을 오가며 동시에 실행하는 기법 <br> 
  -고정 분할 다중 프로그래밍 기법 : 주기억장치를 다수의 고정된 크기로 나눠 실행 중인 프로세스에게 할당하는 기법 <br>
  -가변 분할 다중 프로그래밍 기법 : 고정된 분할의 경계를 없애고 각 작업에게 필요한 만큼의 기억 공간을 할당하는 기법 <br> <br>
  
  *고정 분할 다중 프로그래밍 기법은 분할의 크기가 일치하지 않아 사용하지 못하는 빈 공간이 생길 수 있는데 이를 '단편화'
라고 한다 <br> 

<h2> 주기억장치 관리 전략 </h2>
  -요구 반입 전략 : 실행 중인 프로그램이 다른 프로그램이나 데이터를 참조(요구)할 때 가져온다 <br>
  -예상 반입 전략 : 실행 중인 프로그램이 참조할 가능성이 있는 프로그램이나 데이터를 미리 가져온다 <br> <br>
  
  -최초 적합 배치 전략 : 새로 반입된 프로그램이나 데이터를 적재할 수 있는 주기억장치의 빈 공간 중에서 가장 작은 곳에 배치한다 <br>
  -최악 적합 배치 전략 : 새로 반입된 프로그램이나 데이터를 적재할 수 있는 주기억장치의 빈 공간 중에서 가장 큰 곳에 배치한다 <br>
  
  -교체 전략 : 주기억장치에 새로 반입할 프로그램이나 데이터를 배치할 빈 공가니 없을 때, 배치 공간을 마련하기 위해 주기억장치에서 어떤 프로그램이나 데이터를 제거할지 결정하는 전략 <br>
  
<h2> 단편화 현상 </h2>
  -작업과 분할의 크기가 일치하지 않아 사용하지 못하는 빈 공간이 생기는 것을 '단편화 현상'이라고 한다 <br>
  -내부 단편화 : 분할에 작업을 적재한 후 빈 공간이 남는 단편화 <br>
  -외부 단편화 ; 적재할 작업보다 분할의 크기가 작아서 분할이 빈 공간으로 남게 되는 단편화 <br>
  
<h2> 가장기억장치 구현 기법 </h2>
  -실제 존재하는 기억장치가 아닌 가상기억장치에서 프로세스가 참조하는 가상 주소를 실제주소로 변환하는 것을 '동적 주소 변환'이라고 하고 동적 주소 변환을 통해 구현된다 <br>
  -페이징 기법 : 가상기억장치를 일정한 크기의 페이지로 나누어 관리하는 기법 + 연속적으로 배치되지 않기에 효율적이며 단편화 현상도 제거됨 <br>
  -세그먼테이션 기법 : 가상기억장치를 프로그램이나 데이터의 용도에 따라 가변적인 크기의 세그먼트(부분)로 분할하여 관리하는 기법 + 외부 단편화 현상 발생가능 <br>
  -페이징/세그먼테이션 혼합 기법 : 세그먼트를 다시 페이지 단위로 분할해 관리하는 기법 <br>
  
<h1> [정보 관리] </h1>
<h2> 파일 시스템 </h2>
  -사용자에게 편리한 인터페이스를 제공한다 <br>
  -사용자가 파일을 생성, 수정, 삭제할 수 있는 기능을 제공한다 <br>
  -적절한 제어 방법을 통해 다른 사람의 파일을 공유할 수 있는 기능을 제공한다 <br>
  -불의의 사고에 대비하기 위한 파일 백업 및 복구 기능을  제공한다 <br>
  =정보를 암호화하고 해독할 수 있는 기능을 제공한다 <br>
  
<h2> 파일구조 </h2>
  -레코드가 보조기억장치에 저장되는 방식을 '파일구조'라고 한다 <br>
  -순차 파일 : 레코드를 순차적으로 저장하고 검색한다, 레코드의 빈 공간이 없어 효율적 + 레코드를 삽입하거나 삭제하기 어려움 <br>
  -색인 순차 파일 : key값에 따라 순차 파일 구조와 직접 파일 구조로 나뉜다, 색인을 이용하여 접근하므로 처리 소고다 느림 + 색인 별도의 저장공간이 필요 <br>
  -직접 파일 : 특정 레코드에 직접 접근할 수 있는 파일 형태이다, 처리속도가 빠름 + 특정 레코드 삽입, 수정, 삭제 가능 <br>
  -분할 파일 : 다수의 순차적인 서브 파일로 구성됨, 서브 파일의 시작 주소는 디렉터리 레코드에 저장됨 <br>
  
<h2> 파일의 공간 할당 기법 </h2>
  -연속 할당 : 하드디스크의 빈 공간에 연속적으로 저장하는 기법 <br>
  -불연속 할당 : 파일이 한번 생성되면 이후 작업을 거쳐 크기가 커지거나 줄어들 수 있는데 이걸 처리할 때 유용함 <br>
  -섹터 단위 할당 : 불연속 할달이며, 섹터단위 나눠져있고 주소 포인터로 연결되어 할당함 + 하나의 파일이 디크스 전체에 분산되어 저장됨 <br>
  -블록 단위 할당 : 섹터를 여러개 묶은 블록단위로 할당함 + 연속 할당과 불연속 할당의 절충형 <br>
  
<h2> 파일보호 </h2>
  -접근 제어 행렬 : 개별 파일이나 디렉터리에 대한 접근이 가능한 사용자와 허용되는 동작을 기록한 것을 참좧여 접근 가능 여부를 결정 <br>
  -파일 명명 : 접근하려는 파일에 이름을 부여한 사용자가 아니거나 공유가 허용된 파일이라도 그 파일의 이름을 알지 못하면 접근하지 못하게 하는 방법 <br>
  -암호 : 사용자마다 서로 다른 암호를 제공하고 암호를 모르는 사용자는 접근하지 못하게 하는 방법 <br>
  -암호 기법 : 파일을 암호화하여 해독방법을 아는 사용자만 사용하게 하는 방법 <br>
  -백업 : 파일을 복사하여 다른 곳에 보존하는 방법 + 가장 마지막에 백업한 내용으로 해당 파일을 복구 + 백업이후 손상된 파일은 복구 불가능 + 백업 진행시에는 다른 작업을 중단해야함 <br>
 

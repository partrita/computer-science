# 변경 이력 (Change Log)

**참고**: 현재 커리큘럼은 v9 버전으로 넘어가기 위한 대대적인 검토를 진행 중입니다. 주요 작업은 우리의 추천 강좌들이 [커리큘럼 가이드라인(curricular guidelines)](CURRICULAR_GUIDELINES.md)에 미달하지 않는지 빡빡하게 검수하고, 누락된 주제들을 신규 발굴해 채워 넣으며, 쓸데없이 내용이 겹치거나 범위가 산으로 가는 잉여 강좌들을 모조리 쳐내는 작업들입니다. 이러한 노력의 일환으로 여러분의 코멘트 요청(Requests for Comment)이 완수될 때마다, 커리큘럼 상에 해당 내용은 즉시즉시 변경 및 반영처리 되고 있습니다. 이 길고 지루한 전면 재검토 작업의 마침표가 찍히는 날, 당당히 v9 이라는 이름으로 판올림 버전을 공표할 것입니다.

이 프로젝트의 역사에 기록될 만한 모든 스펙타클한 변동 사항들은 바로 이 파일에 박제될 것입니다.
본 프로젝트는 암묵적으로 다음의 [유의적 버전(Semantic Versioning)](http://semver.org/) 철학을 엄수합니다:
- "MAJOR (주 버전)" 판올림 업데이트: 특정 과목 코어 내의 주제를 통째로 갈아엎고 변경할 때.
- "MINOR (부 버전)" 판올림 업데이트: 가르치는 코어 주제 자체는 동일하지만, 그것을 가르치는 '강좌(courses)'만 다른 옵션으로 갈아치울 때.
- "PATCH (수정 버전)" 업데이트: 미관상, 미학적 변경이나 커리큘럼상 치명적이지 않은 기타 추가/삭제 조치, 혹은 진도 흐름을 더 매끄럽게 만들기 위해 강좌들의 수강 순서를 재배치할 때.

## [8.0.0] 2017-11-01
### 추가됨
- 부록(extras/readings): "시스템 디자인 입문서 (The System Design Primer)" 추가
- 부록(extras/readings): "프로그래머를 위한 카테고리 이론: 서문 (Category Theory for Programmers: The Preface)" 추가
- 부록(extras/readings): "프로그래밍 언어: 응용과 해석 (Programming Languages: Application and Interpretation)" 추가
- 부록(extras/readings): "프로그래밍 및 프로그래밍 언어 (Programming and Programming Languages)" 추가
- 기여자 가이드(CONTRIBUTING): 기여자 지침 안내처에 "Git 배우기 (Learning Git)" 카테고리 추가
- 코어 수학 파트: "선형대수의 본질 (Essence of Linear Algebra)" 영상을 기존 필수 과목이던 "선형대수: 기초부터 최전선까지 (Linear Algebra: Foundations to Frontiers)"에 진입하기 전 찍고 넘어가야 할 선수 강의로 지정해 추가

### 변경됨
- "수학적 사고 입문 (Introduction to Mathematical Thinking)" 녀석을 정규 트랙에서 쫓아내 부록방(extras/courses)으로 귀양 보냄
- "해킹 더 커널 (Hack the Kernel: ops-class)" 과정을 너무 어려워 보여서 처박아 뒀던 심화 시스템(Advanced Systems) 구역에서 다시 끌고 나와 정규 코어 시스템(Core Systems) 구역으로 멱살 잡고 편입시킴
- 코어 시스템 파트: 기존 괴물 교본 "운영체제: 3가지 쉬운 측면 (Operating Systems: Three Easy Pieces)"의 절대 필수 시청 강제 규정을 해제함. 대신 방금 편입된 "해킹 더 커널" 과정을 돌파할 때 곁들여 읽으면 피가 되고 살이 될 최적의 지원군 교재로서의 지위로 하향 조정
- 코어 이론 파트: 극악무도한 Coursera 플랫폼이 돈을 뜯어내려 다크 패턴을 교묘하게 쓴다는 발칙함을 포착, 이에 분노하여 스탠퍼드 알고리즘(Stanford Algorithms) 과정의 수강 플랫폼 호스트 링크를 모조리 Coursera에서 Lagunita 쪽으로 갈아치움

## [7.2.2] 2017-07-02
### 추가됨
- Haskell 을 편하게 돈으로 바르고 싶어 하는 분들을 위해 유료 대안 도서로 "첫 원리부터 배우는 하스켈 프로그래밍 (Haskell Programming from First Principles)" 서적판을 추가
- "씽크 파이썬 (Think Python)" 도서를 부록(extras/readings) 목록표에 추가
- 일부 강좌 내용 중 FAQ 엔트리 항목과 관련 도움 링크들 꼼꼼히 추가 기입
- "카테고리 이론: 부드러운 입문서 (Category Theory: A Gentle Introduction)" 도서를 부록(extras/readings) 목록표에 병합

## [7.2.1] 2017-05-14
### 변경됨
- 네트워킹(Networking) 코스의 예상 완주 소요 일자를 8주(8 weeks)로 대폭 조정
- 짜증을 유발하는 철자 오류 버그 패치 완료

### 추가됨
- 부록방([extras/courses](extras/courses.md)) 라인업에 Haskell 프로그래밍 입문 과정 신규 스카웃 입사

## [7.2.0] 2017-04-28
### 추가됨
- 소프트웨어 테스팅 (Software Testing) 과정 화려하게 데뷔
- 스탠퍼드 라구니타 출신의 알고리즘 과정(Algorithms: Design and Analysis) 직행 링크선 설치 완료
- 다변수 미적분학(Multivariable Calculus) 코스에 덤비다 박살 날 학생들의 등짝을 밀어주기 위해, MIT의 단일변수 미적분학 과정 중 '매개변수 방정식(parametric equations)'과 '극좌표계(polar coordinates)' 챕터 직통 링크를 추가로 발라주어 목숨 생존율 증대 도모

## [7.1.2] 2017-04-22
### 변경됨
- 프로젝트(Projects) 대문 마당에 메가 프로젝트 리스트(Mega Project List)로 통하는 차원문 링크 설치

## [7.1.1] 2017-04-11
### 변경됨
- 대규모 릴리스 출격을 위한 최종 와꾸 터치업 진행

## [7.1.0] 2017-04-10
### 변경됨
- 엉망으로 꼬였던 프로그래밍 언어(programming languages) 과목의 포맷 재구성본을 롤백(회군) 조치

### 추가됨
- 견고한 분산 알고리즘 (Reliable Distributed Algorithms) 강좌들 전격 채용
- 기가 맥힌 새로운 CS 입문 신규 강좌 코스 개장

## [7.0.2] 2017-03-30
### 변경됨
- 해도 그만 안 해도 그만인 선택 옵션형 학습 코스들을 분리 수거하여 부록방(extras/courses)의 새로운 찌그러진 공간으로 몽땅 유배 보냄
- 다른 컴퓨터 아키텍처 예비 코스 녀석 또한 부록방(extras/courses)으로 귀양 보냄

### 추가됨
- 심화 어플리케이션(Advanced applications) 구역에 스칼라(Scala) 특화 전문화(specialization) 코스를 신규 스카웃

### 삭제됨
- 머리통 터지는 커리큘럼을 심플하게 다이어트 시키기 위해 '필수 지정 독서물(required readings)' 들 중 단 하나만 남기고 나머진 무자비하게 청소 삭제해 버림

## [7.0.1] 2017-03-11
### 변경됨
- 죽어버린 브래드필드(Bradfield) 사제 컴퓨터 공학 가이드 웹페이지의 연결 링크 파이프 수리 패치 완료

### 추가됨
- 미적분학(Calculus One) 코스 하단에 수많은 에러타(오류들) 수정표 보고서와 코스 공략 진도 권장 가이드 링크들의 노트 구문 투척
- 부록(extras) 영역에 선택적 엑스트라 강좌들 구겨 넣기:
  - 길버트 스트랭의 선형대수 렉처
  - UC 버클리 출신의 '컴퓨터 프로그램의 구조와 해석 (Structure and Interpretation of Computer Programs)'
- 부록(extras) 영역에 선택적 엑스트라 독서본 책 구겨 넣기:
  - 밴 로이(Van Roy)의 역작 '고급 프로그래밍 (advanced programming)' 개론서
  - P&H 님의 컴퓨터 구조학 (computer architecture) 서적
  - 스키에나(Skiena)의 무서운 알고리즘(algorithms) 해설서
  - 길버트 스트랭(Strang) 성님의 선형대수학 교본
  - 데이터베이스 매니지먼트 시스템(Database Management Systems) 책자
  - 타르(Tarr)가 지은 나만의 '도메인 특화 언어(Domain-specific language)' 창조 비법서
  - 수많은 구루 저자들이 쓴 분산 시스템(distributed systems) 성서 파편 모음집들

## [7.0] 2017-03-09
프로그램 아키텍처 전반의 지각 변동 및 완벽 오버홀(Complete overhaul) 가동

### 변경됨
- 산만하던 기여자들의 행동 수칙 지침(contributor guidelines) 가이드를 보기 좋게 청소해 별도의 파일로 완벽히 떼어 내 격리시킴
- 수십 개로 난도질해 흩뿌려져 있던 과목 카테고리들을, 무수히 많은 주제를 포용하는 단 4개의 거대한 기둥(4개 과목 풀) 체재로 대통합 흡수 통폐합 시행
- 사방에 널렸던 free-books.md와 paid-books.md 종이 쪼가리들을 하나의 거대한 readings.md 책자로 묶어 물리적 컴파일 결합
- free-courses.md와 paid-courses.md 파편 쪼가리들을 courses.md 본체 합체 통폐합 달성
- 구닥다리 쓸모없던 "How to Code" 놈을 처형하고 새롭고 강렬한 "How to Code" (소프트웨어 개발 마이크로 마스터즈 과정 코스)로 위대한 세대교체 달성
- 프린스턴 알고리즘(Princeton Algorithms) 형님을 대체 과정 부록방([alternative courses](#extras/courses.md))으로 퇴출시키고, 스탠퍼드 알고리즘(Stanford Algorithms) 놈을 메인 무대로 끌고 옴

### 추가됨
- 모든 코스 수강생들이 피를 보지 않게끔 각 과목 앞치마에 선수 과목 (prerequisites) 필수 요건 꼬리표 강력 부착 명시 지시
- 학구열 불태우기: 코스/주제별 필수 요구 조건과 프로젝트 과제 필수 달성 목표 사항(Requirements) 기준 확립 통지
- 하스켈(Haskell), 프롤로그(Prolog), 운영체제(Operating Systems) 필수 독서 지정 지침서 추가
- 코스 신설: Dan Grossman 형님의 프로그래밍 언어들 (Programming Languages)
- 코스 신설: 맨땅 헤딩 창조물 '낸드에서 테트리스까지(From Nand to Tetris)' 투입
- 선택 과목 개방: 병렬 프로그래밍 입문 (Intro to Parallel Programming)
- 선택 과목 개방: 완벽을 위한 LAFF 프로그래밍 (LAFF: Programming for Correctness)
- 선택 과목 개방: 수학적 사고 입문 (Introduction to Mathematical Thinking)
- 선택 과목 개방: 공포의 전자기학 (Electricity and Magnetism)
- 선택 과목 개방: MIT발 연산 기초 논리 망치 (MIT's Computation Structures)
- 선택 과목 개방: 악몽의 다변수 미적분학 (Multivariable Calculus)
- 선택 과목 개방: 운영체제 갈아 넣기 (ops-class.org)
- 선택 과목 개방: 오토마타 기계 이론 (Automata Theory)
- 선택 과목 개방: 논리학 입문 (Introduction to Logic)
- 선택 과목 개방: 연산 기하학 (Computational Geometry)
- 선택 과목 개방: 정형 개념 분석 (Formal Concept Analysis)
- 선택 과목 개방: 인간의 게임 이론 (Game Theory)
- 선택 전문화 심화 루트 (Elective specializations) 테크트리 추가 신설:
  - 로보틱스 (Robotics)
  - 데이터 씹어먹기 (Data Mining)
  - 거대한 빅 데이터 (Big Data)
  - 사물 지능 인터넷 (Internet of Things)
  - 클라우드 컴퓨팅 (Cloud Computing)
  - 풀스택 웹 대마왕 (Full Stack Web Development)
  - 데이터 사이언스 (Data Science)
- 구루 프로급(Pro spec) 전문화 강제 훈련 코스들 신설:
  - R로 소프트웨어 마스터링하기 (Mastering Software Development in R)
  - 인공지능 엔지니어 조기 육성 (Artificial Intelligence Engineer)
  - 머신 러닝 장인 육성 (Machine Learning Engineer)
  - 사이버보안 특공대 (Cybersecurity)
  - 안드로이드 노예 개발자 (Android Developer)

### 삭제됨
- 폐허가 된 시체 링크들(dead links)과 트렌드에 폐기된 고기능 쓰레기 강좌들 전면 소각 청소
- 피로도만 올리던 과목당 개별 미니 프로젝트 억지 필수 요구 조항 (per-course project requirement) 족쇄 파기
- 처형 대상 강좌: Java로 객체 지향 프로그래밍 하기 (Object-Oriented Programming in Java)
- 처형 대상 강좌: 스칼라(Scala)로 짓는 함수형 프로그래밍 (Functional Programming in Scala)
- 처형 대상 강좌: 컴퓨터 구조학 (Computer Architecture) (다만 추모의 의미로 하단 주석 footnotes 한 줄로는 목숨 유지시킴)
- 처형 대상 강좌: 이론 컴퓨터 수학 입문 (Intro to Theoretical Computer Science)
- 처형 대상 강좌: 소프트웨어 설계 공정과 애자일 신앙 (Software Processes and Agile Practices)
- 처형 대상 강좌: 운영 체제 깎고 시스템 프로그래밍하기 (Operating Systems & System Programming)
- 처형 대상 강좌: 사이버보안 세상 입문 (Introduction to Cyber Security)
- 처형 대상 강좌: 병렬 컴퓨터 구조론 및 프로그래밍 (Parallel Computer Architecture and Programming)
- 처형 대상 강좌: 모바일쟁이를 위한 UX 디자인 기초 (UX Design for Mobile Developers)

## [6.0] 2016-10-09
### 변경됨
- 그 미친 '미적분학 1(Calculus One)' 지뢰밭을 '컴퓨터 논리 수학 입문(Mathematics for Computer Science)' 보다 아예 앞단이자 교차 병행 과목으로 멱살 잡아다 끌어올려 배치시켜 버림
- "과목들 수강 순서 규정 (Order of the classes)" 단락의 설명을 사람이 읽을 수 있도록 세련되게 치장 재건축함

### 추가됨
- 새로운 OSSU 제국 버전에 맞춘 삐까번쩍한 대문 Trello 투명 보드 개국 선포
- 초심자용 "이 미친 가이드를 조종하는 법(How to use this guide)" 매뉴얼 어귀 안에 "어떻게 내 학습 노하우 진행도를 증명할 것인가(How to track and show your progress)" 가이드 단락 전격 신설 추가
- 대망의 거대 과제 모음 `PROJECTS.md` 선언문 파일 탄생
- 커리큘럼 곳곳의 찢어져 있던 잔여 프로젝트 섹션 내용물들을 이 신생 `PROJECTS.md` 몸통 안으로 모두 영혼 복제 이식 완료

### 삭제됨
- 더 이상 쓸 데 없어진 "다음 나아갈 목표치 (Next Goals)" 오지라퍼 단락 강제 삭제형 집행
- 버려져 썩어가던 원조 OSSU 웹 앱 링크(OSSU web app)의 흔적조차 모조리 지워버림

## [5.1.0] 2016-08-20
컴퓨터 논리 과학 이과 수학의 끝판왕 코스를 최신 기통으로 엔진 업그레이드 조치:

### 변경됨
- 타깃 섹션: **수학 코어 (이산 수학 - Discrete Math)**
  - '컴퓨터 과학도를 위한 수학 (Mathematics for Computer Science)' 폼체인지

## [5.0.0] 2016-08-20
썩은 코어 하나를 도려낸 탓에 아래 연쇄 업데이트 파동 발생:

### 삭제됨
- 타깃 섹션: **자연어 유린기 (Natural Language Processing)**
  - '자연어 처리기 본체 (Natural Language Processing)' 적폐 코스 폭파 삭제

### 추가됨
- 타깃 섹션: **자연어 유린기 (Natural Language Processing)**
  - 그 자리에 대체재인 '자연어 처리의 세계 입문 (Introduction to Natural Language Processing)' 신규 엔진 부품 탑재

## [4.1.0] 2016-08-05
Coursera 저 악랄한 돈벌레 플랫폼의 지형도 개편 도발로 인해, 아래와 같이 보수 공사 강제 진행:
### 해결됨
- 타깃 섹션: **거대 데이터 판 엎기 (Big Data)**
  - '빅 데이터 입문 (Introduction to Big Data)' 주소선 추적 복구 완료

## [4.0.0] 2016-07-30
Coursera의 2차 플랫폼 구조 개편 학살로 인해 당사가 입은 피해 보수 내역:

### 삭제됨
- 타깃 섹션: **이론 수학 증명 (Theory)**
  - '오토마타 (Automata)' 학살당함
- 타깃 섹션: **수학 (선형 대수 결계 - Linear Algebra)**
  - '매트릭스 찢어발기기: 컴퓨터를 조종하는 선형 대수 (Coding the Matrix: Linear Algebra through Computer Science Applications)' 학살당함
- 타깃 섹션: **병렬 연산 가동기 (Parallel Computing)**
  - '이종 잡종 병렬 프로그래밍 (Heterogeneous Parallel Programming)' 학살당함
- 타깃 섹션: **자연어 뜯어먹기 (Natural Language Processing)**
  - '자연어 본체 (Natural Language Processing)' 학살당함

### 해결됨
- 타깃 섹션: **컴퓨터 거미줄 네트워킹 (Computer Networks)**
  - '컴퓨터 네트워크 망 (Computer Networks)' 고아된 링크 복원
- 타깃 섹션: **코드 번역기 컴파일러 (Compilers)**
  - '컴파일러 본체 (Compilers)' 고아된 링크 복원

### 추가됨
- 타깃 섹션: **이론 수학 증명 (Theory)**
  - '이론 컴퓨터 시스템 과학 입문로 (Intro to Theoretical Computer Science)' 신규 파이프 개통
- 타깃 섹션: **수학 (선형 대수 결계 - Linear Algebra)**
  - '선형 대수 지옥 - 베이스캠프부터 프론티어 최전선까지 (Linear Algebra - Foundations to Frontiers)' 신규 개통
- 타깃 섹션: **병렬 연산 가동기 (Parallel Computing)**
  - '병렬 컴퓨터 코어 구조론과 프로그래밍 삽질 (Parallel Computer Architecture and Programming)' 신규 개통
- 타깃 섹션: **자연어 뜯어먹기 (Natural Language Processing)**
  - '자연 언어 해체 머신 프로세싱 (Natural Language Processing)' 새로운 주소지로 입주 세팅 완

## [3.0.0] 2016-05-04
### 삭제됨
- 타깃 섹션: **컴퓨터 공학 신병 입문 (Introduction to Computer Science)**:
	- '파이썬을 휘두르는 컴퓨터 공학과 프로그래밍 찍먹 (Introduction to Computer Science and Programming Using Python)' 방출
	- '초초 밑바닥 낸드 소자부터 고상한 테트리스까지 (From Nand to Tetris - Part 1)' 방출

### 추가됨
- 타깃 섹션: **컴퓨터 공학 신병 입문 (Introduction to Computer Science)**:
	- 하버드발 자존심 '에센스 컴퓨터 입문 - CS50 (Introduction to Computer Science - CS50)' 황제 스카웃 등극

## [2.0.1] 2016-04-04
### 해결됨
- 이제 오합지졸 수강생분들은 저희가 손수 다이아몬드급으로 직조해 놓은 OSSU [커스텀 웹 앱 포털(web app)](https://ossu.firebaseapp.com)에 로그인해 수강 증명을 등록하시기 바랍니다.

## [2.0.0] 2016-03-17
### 해결됨
- 프로그램 아키텍처 디자인 섹션(Program Design section) 밑에 널브러져 있던 이질적 코스들의 촌스러운 이름 장부와 불량 링크들을 무자비하게 교정 타격함

### 삭제됨
- 극대노 대규모 학살 방출 리스트:
- **컴퓨터 신병 기초 (Introduction to Computer Science)**:
	- '컴퓨터 베이직 입문 (Introduction to Computer Science)'
	- '컴퓨터적 알고리즘 마인드 탑재와 데이터 과학 훑기 (Introduction to Computational Thinking and Data Science)'
- **알고리즘 (Algorithms)**
	- '알고리즘 분해 분석론 (Analysis of Algorithms)'
- **프로그래밍 관념 철학 (Programming Paradigms)**
	- '리액티브 역동적 프로그래밍의 실체 (Principles of Reactive Programming)'
- **미적분학 (Math - Calculus)**
	- '초절정 다변수 미적분 계산기 (Multivariable Calculus)'
- **소프트웨어 뼈대 조립 아키텍처 (Software Architecture)**:
	- '웹 구사 어플리케이션 아키텍처 본질들 (Web Application Architectures)'
- **소프트웨어 공장 엔지니어링 (Software Engineering)**:
	- '루비 온 레일즈 찍먹과 애자일 숭배론 - 기초편 (Agile Development Using Ruby on Rails - Basics)'
	- '루비 온 레일즈 뼛속까지 파먹고 애자일 숭배론 - 심화편 (Agile Development Using Ruby on Rails - Advanced)'
	- '스타트업 영웅 엔지니어링 짓 (Startup Engineering)'
- **컴퓨터 하드웨어 아키텍처 (Computer Architecture)**:
	- '하드웨어와 소프트웨어가 만나는 중간 계층 다리 (The Hardware/Software Interface)'
- **운영 뇌 체제 (Operating Systems)**:
	- '운영 체제 갈아 넣는 엔지니어링 짓 (Operating System Engineering)'
- **컴퓨터 거미줄 망 네트워킹 (Computer Networks)**:
	- '컴퓨터 전산 망 네트워킹 도화선 입문 (Introduction to Computer Networking)'
- **암호화 매직 (Cryptography)**:
	- '응용 실전 스텔스 암호학 (Applied Cryptography)'

**은밀한 알림(ps)**: 이렇게 빗자루질당한 쓸모없어진 강좌 귀신들은 모조리 부록방에 포장되어 [엑스트라 부록관 링크(extras)](https://github.com/ossu/computer-science/tree/master/extras) 묘지에 매장 조치되었습니다.

## [1.3.12] 2016-03-17
### 추가됨
- 협동 안내 지침(How to collaborate): 여분 강좌 링크 조공품들을 부록방(extras section)에 던져넣는 예법 헌장 조문 추가

## [1.3.11] 2016-03-06
### 해결됨
- 낸드부터 테트리스 지옥(Nand to Tetris) 강의: 구질구질한 네이밍과 url 세탁
- UC 버클리표 애자일 숭배론 개발기(UC Berkeley Agile development): 네이밍과 url 세탁
- 스페셜라이제이션(특화 강좌 묶음) 심연으로 통하는 단축 터널 다이렉트 링크 공사 완

## [1.3.10] 2016-03-06
### 해결됨
- '체계적 프로그램 설계 마스터리 2부 (Systematic Program Design Part 2)'로 향하는 썩은 나루터 링크 선로 교체 보수공사

## [1.3.9] 2015-11-09
### 해결됨
- 자연어 해체 처리반 (Natural Language Processing) 강좌로 가는 진짜 오리지널 정석 주소 링크망으로 추적 수정

## [1.3.8] 2015-11-07
### 추가됨
- 이리 치이고 저리 치일 동지들을 위해 무한한 레퍼런스가 창고처럼 쌓인 "프로젝트 제안/추천 목록 (Project Suggestions)" 구조선 섹션 거점 추가 파밍 완료

## [1.3.7] 2015-11-01
### 삭제됨
- 더럽혀지던 project.md 파일을 부숴버리고, 온전하게 짐을 싸서 통째로 **help(지원용 부속)** 리포지토리 망으로 격리 이주 추방 시킴

## [1.3.6] 2015-10-22
### 추가됨
- 따끈따끈하게 포장된 따끈한 최신 엔진 버전의 "CS 162 지옥, 운영 체제 및 뇌 시스템 프로그래밍 파먹기(Operating Systems and System Programming)" 코스 납품 입고 완료

## [1.2.6] 2015-10-19
### 추가됨
- Awesome 영웅들 리스트 보드 직행 고속 배지/단축 포털 하이퍼링크 문신 새김

## [1.2.5] 2015-10-16
### 해결됨
- 명패 이름이 병신 같던 불량 섹션 네이밍들의 각을 바로잡고 이쁘장하게 광택 나는 하이퍼링크 초칠 교정 마감

## [1.2.4] 2015-10-14
### 삭제됨
- 거슬리는 '대중적 약속 서약 (public commitment)' 웅앵웅 인용구 문구 오글거려서 찢어버림

## [1.2.3] 2015-10-12
### 변경됨
- 선수 과목 무기고 (prerequisite section)를 똥 멍청이도 단박에 이해할 수 있게끔 크리스탈 클리어한 텍스트로 무지막지하게 해체 및 재조립 패치함

## [1.2.2] 2015-10-12
### 해결됨
- 호구 학생들의 코스 수강 등록 이슈 창구를 위한, 튼튼하고 어여쁜 핫라인 신규 파이프 링크 배관 설치 공사 완

## [1.2.1] 2015-10-11
### 추가됨
- 선수 필수 지식 감옥방(prerequisite section) 안에 전 세계의 근간인 "Git - 개초보를 위한 옹알이 단순 바이블 가이드 (Git - the simple guide)" 구원 아티클 전격 이식

## [1.1.1] 2015-10-11
### 해결됨
- 치명적 타이핑 어그로 버그타파 (Fix typos):
  - 무식하게스리 MOOC이란 말 자체가 뒤에 Course(C)가 붙은 "거대 공개 온라인 코스(Massive Open Online Course)"라는 뜻인데 거기에 또 'MOOC 강좌' 따위로 역겹게 중복해서 쓰던 문법 파괴 첩어들 싹 다 도려냄
  - "레알 현실 문제(real problem)" 란게 도대체 뭔지 애매했던 문맥을 상세하게 늘려 풀어 설명함
  - 작지만 개빡치는 미세 문법 및 워딩 어색충 버그들 일망타진

## [1.1.0] 2015-10-08
### 추가됨
- 당신의 차가운 뇌를 달구기 위한 뇌 예열 동기 부여 & 맨몸 육체 가동 준비 운동장 섹션 (의무 아님 선택형 자원 optional resources) 개장
  - 자극 포르노 아티클판: 당신의 한계 돌파를 위한 MIT 챌린지 썰 (Article: MIT Challenge)
  - 코스 도장 깨기판: 멍청한 뇌를 학습형 뇌로 바꾸는 "학습법 자체를 학습하는 스킬 (Learning How to Learn)" 코스 유치

## [1.0.0] 2015-10-08

대망의 전 세계 구원을 위한 완벽무결 마그나 카르타 1.0 컴공 마스터 커리큘럼 성서 버전 천하 제1 배포 **(Release of the first complete version)**

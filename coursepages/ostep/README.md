# 운영 체제: 세 가지 쉬운 부분 (Operating Systems: Three Easy Pieces)

감사의 말: [palladian](https://github.com/palladian1)

## 소개

솔직히 말해서, 운영 체제에 대한 독립적인 온라인 과정을 찾기는 정말 어렵습니다. OSTEP은 지금까지 우리가 찾은 최고의 과정입니다. 아래에서는 대부분의 학생에게 적합한 "기본" 접근 방식과 시스템 프로그래밍을 전문으로 하려는 학생에게 적합한 "확장" 접근 방식, 두 가지 접근 방식을 설명합니다.

"기본" 접근 방식은 우리의 모든 운영 체제 커리큘럼 요구 사항을 다루며 약 80시간의 작업이 소요됩니다.

"확장" 접근 방식은 기본 접근 방식의 모든 작업과 그 이상을 포함합니다. 매우 진지한 C 및 x86 어셈블리 학습과 커널 프로그래밍에 대한 깊이 있는 탐구를 포함합니다. 훨씬 더 많은 시간(200시간 이상)이 소요되며 훨씬 더 어렵습니다. 이 컴퓨팅 분야에 관심 있는 학생들에게는 매우 보람 있는 과정이기도 합니다.

## 기본 접근 방식

1. 무료 온라인 교재 [운영 체제: 세 가지 쉬운 부분](https://pages.cs.wisc.edu/~remzi/OSTEP/)을 읽으십시오.
2. 각 장의 끝에 있는 숙제 문제를 완료하십시오. (숙제에 대한 [Github 저장소](https://github.com/remzi-arpacidusseau/ostep-homework)가 있습니다.)

이 작업은 약 8주, 주당 10시간이 소요됩니다. 이것이 전부입니다!

유닉스/리눅스 시스템, 몇 가지 기본 명령줄 도구 및 C 컴파일러(예: GCC 또는 Clang)가 필요합니다. Windows에서는 가상 머신에 Ubuntu를 설치하거나 WSL(Windows Subsystem for Linux)을 사용할 수 있습니다. Mac OS는 유닉스 계열이므로 사용해도 괜찮습니다.

### 과정 링크

* [책](https://pages.cs.wisc.edu/~remzi/OSTEP/)
* [숙제](https://pages.cs.wisc.edu/~remzi/OSTEP/Homework/homework.html)
* [숙제 소스 코드 저장소](https://github.com/remzi-arpacidusseau/ostep-homework)
* [숙제 해답](https://github.com/xxyzz/ostep-hw)

### C 언어

**질문**: 이 책에 C 코드가 좀 있던데, C 언어를 얼마나 알아야 하나요?

**답변**: 이 책에서 C 코드를 읽고 이해해야 합니다. 배열, 포인터 및 출력 형식에 대한 기본 이해가 필요합니다. 무료 책 [Dive into Systems: 1장 및 2장](https://diveintosystems.org/book/C1-C_intro/index.html)을 참조할 수 있습니다. [CS50 매뉴얼 페이지](https://manual.cs50.io)도 함수를 찾는 데 유용합니다. C 언어 학습에 너무 많은 시간을 할애해서는 안 됩니다.

읽게 될 코드는 상당히 간단하며 짧은 단편으로 제공됩니다. 이 책은 프로세스 API, 스레드 API 등과 같은 많은 C API를 수동으로 소개하여 많은 도움을 줍니다. 코드 단편을 입력, 컴파일 및 실행하고 해당 설명을 읽을 수 있습니다. 이 책은 재미있게 읽을 수 있는 대화체 스타일로 매우 자세하게 설명합니다.

약간의 C 코드도 작성하게 됩니다. 전체 장의 일부(약 50개 중 10개)만이 C 코드를 작성하도록 요구하며 (다른 장에서는 제공된 시뮬레이션 코드를 실행하고 질문에 답하도록 요구합니다). 이들은 일반적으로 해당 장에 제시된 코드를 약간 수정하여 모방한 간단하고 짧은 C 프로그램입니다.
숙제를 시작할 준비가 되면 [reverse 프로젝트](https://github.com/billmei/ostep-projects/tree/billmei/patch-1/initial-reverse)부터 시작하십시오. 이는 나머지 프로젝트를 수행할 준비가 되었는지 확인하는 좋은 테스트가 될 것입니다. 나머지 숙제 프로젝트는 과정 링크 아래의 링크를 사용하십시오.

이러한 문제에 막히면 너무 많은 시간을 할애하지 마십시오. 훌륭한 해답 세트가 [여기](https://github.com/xxyzz/ostep-hw)에 있습니다. 이에 대한 명예 규정은 없으므로 자유롭게 해답을 사용할 수 있습니다. 너무 많은 시간을 소비하고 있다면 대신 해답을 읽고 이해하십시오. 주요 우선 순위는 운영 체제 개념을 이해하는 것이지 C 코딩을 마스터하는 것이 아닙니다.

## 확장 접근 방식

이 옵션을 선택했다면, OSSU 커리큘럼에서 이전에 수강한 과정 외에 시작하기 전에 스스로 몇 가지 선수 과목을 학습해야 하는 첫 번째 과정입니다. 또한 숙제 데모 및 프로젝트 솔루션 테스트를 위한 스크립트를 실행하는 데 몇 가지 문제가 발생할 수 있습니다(지금까지 대부분 해결되었기를 바랍니다).

즉, 선수 과목에 필요한 시간을 할애할 수 있다면 그 보상은 노력할 가치가 있다고 생각합니다. 이 과정은 흥미롭고 재미있으며 다른 컴퓨터 과학 및 프로그래밍 분야에도 매우 유용합니다. 이 과정의 가장 큰 매력 중 하나는 단순하지만 완벽하게 작동하는 유닉스 계열 운영 체제를 실제로 보고 그 안에 담긴 개념과 설계 결정, 그리고 저수준 구현 세부 정보를 이해할 수 있는 기회입니다.

모든 강의 비디오를 시청하거나 교재의 1장부터 47장까지 읽어야 하며(걱정하지 마십시오. 각 장은 보통 몇 페이지에 불과합니다), 아래 나열된 프로젝트도 완료해야 합니다. 또한 과정 웹사이트나 책의 장에 할당된 대로 숙제 연습 문제를 수행하는 것을 강력히 권장합니다. Coursera나 edX와 같은 사이트의 강의 비디오 중간에 나오는 "이해 확인" 질문과 같다고 생각하십시오.

### 선수 과목

이 수업은 C 프로그래밍 경험이 많이 필요합니다. 이 과정을 시작하기 *전에* [아래 자료](#c-언어-1)에 나열된 C 책 중 하나를 완료해야 합니다. 과정 자료와 동시에 C를 배우려고 하면 벅차다고 느낄 가능성이 높습니다. 이전에 C를 사용해 본 적이 없다면 많은 시간을 할애해야 할 것으로 예상됩니다. 각 개인에게 얼마나 걸릴지 예측하기는 어렵지만 대략적으로 주당 8-10시간씩 3-5주 정도 걸릴 수 있습니다. 항상 다른 OSSU 과정과 함께 C를 배우거나 다른 과정의 연습 문제를 C로 다시 풀어보면서 연습할 수 있습니다.

또한 이 과정을 시작하기 전에 Nand2Tetris의 두 부분을 모두 완료해야 합니다. OSTEP은 실제 x86 및 x86_64 아키텍처에 중점을 두므로 Nand2Tetris에서 배운 개념을 새로운 아키텍처로 전환하기 위해 몇 가지 공백을 메워야 합니다. 아래 x86 자료를 사용하여 그렇게 할 수 있지만, 모두 C를 알고 있다고 가정하므로 먼저 C를 배우십시오. 총 6-8시간 정도 소요됩니다.

### 과정 링크

* [과정 웹사이트](https://pages.cs.wisc.edu/~remzi/Classes/537/Spring2018/)
* [책](https://pages.cs.wisc.edu/~remzi/OSTEP/)
* [강의 비디오](https://pages.cs.wisc.edu/~remzi/Classes/537/Spring2018/Discussion/videos.html)
* [숙제](https://pages.cs.wisc.edu/~remzi/OSTEP/Homework/homework.html)
* [숙제 소스 코드 저장소](https://github.com/remzi-arpacidusseau/ostep-homework)
* [숙제 해답](https://github.com/xxyzz/ostep-hw)
* [프로젝트](https://github.com/remzi-arpacidusseau/ostep-projects)
* [xv6](https://github.com/mit-pdos/xv6-public)

### 로드맵

이 과정은 원래 OSTEP 교재의 저자가 위스콘신 대학교에서 CS 537로 가르쳤으므로, 프로젝트는 위스콘신 학생들에게 강의실 및 사무실 시간과 같은 교내 자료에 접근할 수 있는 최적의 시기에 따라 과정에 할당됩니다. 즉, 강의나 교재 장에서 다루는 내용과 완벽하게 일치하지 않습니다. 대신 다음 순서대로 과정을 진행하는 것이 좋습니다.

[읽기 순서](Reading-order.md)

* OSTEP 교재의 1장과 2장을 읽고 강의 1의 전반부(소개)를 시청하십시오.
* `initial-utilities` 프로젝트를 수행하십시오. 이 수업을 듣기 전에 C에 충분히 익숙한지 확인하기 위한 리트머스 테스트입니다. 도움이 필요하면 토론 1을 시청하십시오. 코드 작성에 2시간 이상 걸리면(토론 시간 및 디버깅 시간 제외) 과정 진행 전에 C 학습에 더 많은 시간을 할애하는 것을 고려해야 합니다. (더 많은 연습을 원하면 `initial-reverse`도 수행할 수 있지만 필수는 아닙니다.)
* OSTEP 교재의 1강부터 5강까지 시청하고 3장부터 24장까지 읽으십시오. 과정 달력이나 책의 장에 나오는 대로 숙제를 하는 것이 좋습니다.
* 토론 3을 시청하고 5장을 다시 읽은 다음 `processes-shell` 프로젝트를 수행하십시오.
* 아래 자료 섹션에 링크된 xv6 주석 가이드를 처음부터 읽고 `시스템 호출: 프로세스` 섹션 이후에 중단하십시오.
* 토론 2를 시청한 다음 `initial-xv6` 프로젝트를 수행하십시오.
* 토론 5를 시청한 다음 `scheduling-xv6-lottery` 프로젝트를 수행하십시오.
* 토론 7을 시청한 다음 `vm-xv6-intro` 프로젝트를 수행하십시오.
* 6강부터 9강까지 시청하고(선택적으로 복습 강의도 시청) 25장부터 34장까지 읽으십시오. 다시 말하지만 숙제를 하는 것이 좋습니다.
* 토론 10을 시청한 다음 `concurrency-xv6-threads` 프로젝트를 수행하십시오.
* 토론 11과 12를 시청한 다음 `concurrency-mapreduce` 프로젝트를 수행하십시오.
* 10강부터 14강까지 시청하고(선택적으로 두 번째 복습 강의도 시청) 35장부터 47장까지 읽으십시오. 강의나 장과 함께 숙제를 하는 것을 잊지 마십시오.
* `filesystems-checker` 프로젝트를 수행하십시오.

### 프로젝트 실행

이 과정은 원래 OSTEP 교재의 저자가 위스콘신 대학교에서 CS 537로 가르쳤으므로 숙제와 프로젝트는 해당 학생들을 대상으로 작성되었으며 특정 소프트웨어 버전이 미리 설치된 위스콘신 실험실 컴퓨터에서 실행되도록 설계되었습니다. 이 섹션에서 다른 컴퓨터에서도 실행할 수 있도록 수정되었기를 바라지만, 모든 컴퓨터에서 테스트하지는 않았으므로 다른 문제가 발생하면 [Discord 채널](https://discord.gg/MJ9YXyV)에 알려주시면 도와드리겠습니다.

리눅스 또는 macOS에서 숙제와 프로젝트를 실행하려면 다음 프로그램이 모두 설치되어 있어야 합니다.

* `gcc`
* `gas`
* `ld`
* `gdb`
* `make`
* `objcopy`
* `objdump`
* `dd`
* `python`
* `perl`
* `gawk`
* `expect`
* `git`

또한 `qemu`를 설치해야 하지만 xv6 작성자가 제공하는 패치된 버전을 사용하는 것이 좋습니다. 자세한 내용은 [이 링크](https://pdos.csail.mit.edu/6.828/2018/tools.html)를 참조하십시오.

macOS에서는 x86 ELF 바이너리를 생성할 수 있는 교차 컴파일러 `gcc` 제품군을 설치해야 합니다. 자세한 내용은 위 링크를 참조하십시오.

Windows에서는 숙제 및 프로젝트에 리눅스 가상 머신을 사용할 수 있습니다. 이러한 패키지 중 일부는 아직 Apple M1 컴퓨터에서 지원되지 않으며 가상 머신 소프트웨어는 아직 새 프로세서 아키텍처로 이식되지 않았습니다. 일부 학생들은 대신 VPS를 사용하여 숙제와 프로젝트를 수행했습니다.

다음으로 `ostep-homework` 및 `ostep-projects` 저장소를 복제합니다.
```sh
git clone https://github.com/remzi-arpacidusseau/ostep-homework/
git clone https://github.com/remzi-arpacidusseau/ostep-projects/
cd ostep-projects
```

각 xv6 관련 OSTEP 프로젝트의 디렉토리에 [`xv6-public` 저장소](https://github.com/mit-pdos/xv6-public)를 복제해야 합니다. 모든 프로젝트에 동일한 복사본을 사용할 수 있지만 이전 프로젝트가 이후 프로젝트에 버그를 유발하는 것을 방지하기 위해 별도의 복사본을 사용하는 것이 좋습니다. `initial-xv6`, `scheduling-xv6-lottery`, `vm-xv6-intro`, `concurrency-xv6-threads` 및 `filesystems-checker` 디렉토리 *각각*에서 다음 명령을 실행하십시오.

```sh
mkdir src
git clone https://github.com/mit-pdos/xv6-public src
```

### 프로젝트 힌트 및 팁

- `initial-reverse`: 테스트를 통과하는 데 필요한 오류 메시지가 잘못되었습니다! 제공된 텍스트에는 `"error: ..."`라고 되어 있었지만 테스트에서는 `"reverse: ..."`를 예상했으므로 코드에서 테스트의 예상과 일치하는지 확인하십시오.
- [`processes-shell`에 대한 힌트 및 팁](Project-2A-processes-shell.md)
- [프로젝트 1B: `initial-xv6`에 대한 힌트](Project-1B-initial-xv6.md)
- [`scheduling-xv6-lottery`에 대한 힌트](Scheduling-xv6-lottery.md)
- [`vm-xv6-intro`에 대한 힌트](vm-xv6-intro.md)

### 자료

#### C 언어

GeeksforGeeks, TutorialsPoint 또는 Hackr.io와 같은 사이트에서 C를 배우려고 하지 마십시오(여기서는 링크조차 하지 않겠습니다). 이러한 사이트는 다른 언어에는 훌륭한 자료이지만 C에는 너무 많은 함정이 있으며 온라인 C 튜토리얼은 종종 위험한 오류와 잘못된 코딩 관행으로 가득 차 있습니다. 아래 권장 사항을 위해 많은 C 자료를 살펴보았고 안타깝게도 *많은* 나쁘거나 안전하지 않은 자료를 발견했습니다. 여기에는 최고의 자료만 포함하므로 더 이상 찾지 마십시오!

Jens Gustedt의 *Modern C* 전체를 통해 C를 배우는 것을 권장합니다. 이 책은 [온라인에서 무료로 제공](https://inria.hal.science/hal-02383654v2/file/modernC.pdf)됩니다. 이 책은 비교적 짧으며 C 언어 자체와 현대적인 코딩 관행에 대해 빠르게 익힐 수 있도록 해줍니다. 각주에 있는 모든 연습 문제를 반드시 수행하십시오!

위의 책이 기본 권장 사항이지만, K.N. King의 [*C Programming: A Modern Approach*](http://www.knking.com/books/c2/)를 두 번째로 더 초보자 친화적인 옵션으로 권장합니다. 몇 가지 단점이 있습니다. 훨씬 길고(거의 850페이지), 무료로 제공되지 않으며(사본을 찾기 어려울 수 있음), *Modern C*만큼 최신은 아니지만(그럼에도 불구하고 여전히 관련성이 있음) 그럼에도 불구하고 추가 연습을 원한다면 더 많은 연습 문제가 있으며 각 장 끝의 Q&A 섹션에는 C 지혜의 진주와 C FAQ에 대한 답변이 가득합니다. 또한 거의 모든 C 언어와 표준 라이브러리를 다루므로 참조 책으로도 사용할 수 있습니다.

CS 50은 OSTEP에 충분한 C를 다루지 않지만 이미 CS 50을 수강했다면 위의 책으로 보충할 수 있습니다.

추가 (***선택 사항***) 자료는 다음과 같습니다.
* [CS 50 매뉴얼 페이지](https://manual.cs50.io): C 라이브러리 함수를 찾는 데 유용한 참조 자료입니다. 대부분의 함수에는 일반적인 매뉴얼과 초보자 친화적인 "덜 편안한" 옵션이 모두 포함되어 있습니다("덜 편안한" 버전에서는 `string`을 `char *`의 별칭으로 사용한다는 점에 유의하십시오).
* [cdecl](https://cdecl.org): C 전문 용어를 영어로 번역하는 도구입니다.
* [exercism.org의 C 트랙](https://exercism.org/tracks/C): 추가 연습 문제입니다.
* [C 및 C++의 보안 코딩 관행](https://www.amazon.com/dp/0321822137): 다른 C 자료가 왜 그렇게 안전하지 않은지 이해하고 싶다면 이 책을 참조하십시오.
* [*The C Programming Language*](https://www.amazon.com/dp/0131103628): C 제작자들이 쓴 C에 대한 원조 책입니다. OSTEP에는 너무 구식이지만 사본을 찾을 수 있다면 읽어볼 만합니다.

#### x86 아키텍처 및 어셈블리 언어

Nand2Tetris는 이미 시스템 및 컴퓨터 아키텍처를 이해하는 데 필요한 대부분의 개념을 소개했으므로 이제 해당 지식을 실제 (32비트) x86 아키텍처로 옮기기만 하면 됩니다.

가장 쉬운 방법은 *Computer Systems: A Programmer's Perspective* 과정의 일부 강의를 시청하거나 (또는 같은 이름의 [교재](https://www.amazon.com/dp/013409266X)에서 해당 장을 읽는 것)입니다. 필요한 강의는 다음과 같습니다.

* [기계 수준 프로그래밍 I: 기본](https://scs.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=6e410255-3858-4e85-89c7-812c5845d197)
* [기계 수준 프로그래밍 II: 제어](https://scs.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=fc93c499-8fc9-4652-9a99-711058054afb)
* [기계 수준 프로그래밍 III: 프로시저](https://scs.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=2994255f-923b-4ad4-8fb4-5def7fd802cd)
* [기계 수준 프로그래밍 IV: 데이터](https://scs.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=03308c94-fc20-40d8-8978-1a9b81c344ed)
* [기계 수준 프로그래밍 V: 고급 주제](https://scs.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=3f0bf9ca-d640-4798-b91a-73aed656a10a)
* [연결](https://scs.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=0aef84fc-a53b-49c6-bb43-14cb2b175249)

또한 다음 실습을 수행하는 것이 좋습니다. 이러한 실습은 어셈블리 작업 방법을 가르치기 위한 것입니다.
* **폭탄 실습**: [설명서](http://csapp.cs.cmu.edu/3e/bomblab.pdf), [자습용 유인물](https://csapp.cs.cmu.edu/3e/bomb.tar).
  > "바이너리 폭탄"은 학생들에게 개체 코드 파일로 제공되는 프로그램입니다. 실행하면 사용자에게 6개의 다른 문자열을 입력하라는 메시지가 표시됩니다. 이 중 하나라도 잘못되면 폭탄이 "폭발"하여 오류 메시지를 출력하고 채점 서버에 이벤트를 기록합니다. 학생들은 프로그램을 디스어셈블하고 리버스 엔지니어링하여 6개의 문자열이 무엇이어야 하는지 확인하여 자신의 고유한 폭탄을 "해체"해야 합니다. 이 실습은 학생들에게 어셈블리 언어를 이해하도록 가르치고 디버거 사용법을 배우도록 강요합니다. 또한 매우 재미있습니다. CMU 학부생들 사이에서 전설적인 실습입니다.
* **공격 실습**: [설명서](http://csapp.cs.cmu.edu/3e/attacklab.pdf), [자습용 유인물](https://csapp.cs.cmu.edu/3e/target1.tar).
  > 학생들에게는 버퍼 오버플로 버그가 있는 고유하게 사용자 지정 생성된 x86-64 바이너리 실행 파일 쌍인 대상이 제공됩니다. 한 대상은 코드 주입 공격에 취약합니다. 다른 대상은 반환 지향 프로그래밍 공격에 취약합니다. 학생들은 코드 주입 또는 반환 지향 프로그래밍을 기반으로 익스플로잇을 개발하여 대상의 동작을 수정하도록 요청받습니다. 이 실습은 학생들에게 스택 규율에 대해 가르치고 버퍼 오버플로 공격에 취약한 코드를 작성하는 위험에 대해 가르칩니다. **참고:** 대상이 존재하지 않는 채점 서버에 연결하려고 시도하지 않도록 -q 플래그를 사용하여 대상을 실행하십시오.

추가 (***선택 사항***) 자료는 다음과 같습니다.
* [CPU 레지스터 x86](https://wiki.osdev.org/CPU_Registers_x86): 특정 레지스터를 찾는 데 유용합니다.
* [*PC 어셈블리 언어*](https://pdos.csail.mit.edu/6.828/2018/readings/pcasm-book.pdf): x86 어셈블리에 대한 짧은 책입니다.
* [GCC 인라인 어셈블리 HOWTO](https://www.ibiblio.org/gferg/ldp/GCC-Inline-Assembly-HOWTO.html): C 프로그램 내에서 어셈블리 코드를 작성하는 방법에 대한 안내서입니다.
* [*Intel 80386 프로그래머 참조 매뉴얼*](https://pdos.csail.mit.edu/6.828/2018/readings/i386.pdf): Intel의 공식 (그리고 방대한) 자료입니다.

#### xv6

OSTEP을 시작하기 전까지는 xv6에 대해 아무것도 읽을 필요가 없습니다. 사실, 가상화에 대한 전체 섹션을 마칠 때까지 xv6 관련 프로젝트를 보류하는 것이 좋습니다. 그 후에는 소스 코드를 안내해 줄 가이드가 필요합니다.

xv6 작성자는 소스 코드와 함께 읽을 수 있는 [책](https://pdos.csail.mit.edu/6.828/2018/xv6/book-rev11.pdf)을 제공합니다. 또한 각 함수나 상수가 정확히 어디에 사용되는지 볼 수 있는 인덱스가 있는 편리한 줄 번호가 매겨진 [PDF 버전](https://pdos.csail.mit.edu/6.828/2018/xv6/xv6-rev11.pdf)의 코드도 있습니다.

그러나 해당 책은 사용된 고급 C 기능, x86 아키텍처별 명령어 및 동시성 측면(OSTEP의 해당 섹션을 xv6 프로젝트 시작 전에 마치지 않은 경우)을 포함하여 코드의 많은 세부 정보를 간과합니다. 이 문제를 해결하기 위해 전체 xv6 코드를 살펴보고 사용된 C 기능, 하드웨어 사양 및 x86 규칙에 대한 설명과 함께 한 줄씩 분석하는 [xv6 주석 가이드](https://github.com/palladian1/xv6-annotated)를 제공합니다. 즉, 공식 xv6 책보다 길므로 전부 읽을 필요는 없지만(그리고 장치 드라이버에 관심이 없다면 선택적 섹션은 건너뛰어도 됩니다), 코드의 일부에 대해 머리를 긁적이고 있다면 참조로 사용할 수 있습니다.

[여기](https://github.com/YehudaShapira/xv6-explained)는 xv6 코드에 대한 또 다른 심층적인 설명입니다.

또한 [여기](https://www.youtube.com/playlist?list=PLbtzT1TYeoMhTPzyTZboW_j7TPAnjv9XB)는 xv6 코드의 많은 부분을 안내하는 훌륭한 비디오 시리즈입니다.

#### 기타

xv6용 Makefile을 사용하려면 Makefile이 작동하는 방식에 대한 일반적인 이해가 필요합니다. [이 튜토리얼](https://makefiletutorial.com)은 필요한 것보다 훨씬 많은 내용을 다룹니다. "시작하기" 및 "대상" 섹션만 읽고 나중에 필요한 경우 나머지를 다시 참조하십시오(하지만 그럴 필요는 없을 것입니다).

추가 (선택 사항) 자료는 다음과 같습니다.
* [GCC 명령 옵션](https://gcc.gnu.org/onlinedocs/gcc-11.1.0/gcc/Invoking-GCC.html#Invoking-GCC): GNU C 컴파일러 `gcc`의 명령줄 플래그에 대한 안내서입니다.
* [링커 스크립트](https://sourceware.org/binutils/docs/ld/Scripts.html#Scripts): GNU 링커 `ld`용 스크립트 작성 안내서입니다.
* [OSDev 위키](https://wiki.osdev.org): 모든 종류의 OS 개념 및 구현 세부 정보에 대한 훌륭한 자료입니다.
* [*리눅스 커널 개발*](https://www.amazon.com/dp/0672329468): xv6 지식을 리눅스 커널에 기여하는 데 적용하고 싶다면 OSTEP 이후에 읽어볼 만한 훌륭한 책입니다.

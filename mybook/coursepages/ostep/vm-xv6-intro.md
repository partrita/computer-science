크레딧은 [palladian](https://github.com/palladian1) 님께 있습니다

## xv6 가상 메모리의 공포 속으로 (Intro To xv6 Virtual Memory)

### 경고 (WARNING):

*이 프로젝트 템플릿의 내용과 현재 저희가 제공하는 xv6 소스 코드 사이에는 치명적인 미스매치가 존재합니다. 이미 최신 배포 소스에는 이 프로젝트가 완료된 상태로 모조리 흡수 구현되어 버린 끔찍한 상태입니다!*

이를 수습하기 위해 [palladian](https://github.com/palladian1) 님이 필사적으로 위스콘신 대학 모 학생의 깃허브 하수구까지 파고들어 전혀 훼손되지 않은 또 다른 원시 xv6 소셜 코드를 발굴해 냈습니다. 이놈을 구동시키기 위해 억지로 `Makefile` 배을 갈라서 QEMU 실행 파일 구동 경로가 어긋나지 않도록 짜깁기를 가해야만 했습니다. 살인적인 메모리 무방비 상태(lack of memory safety)의 공포를 피부에 각인시키기 위해, 유저 세상(`user` 폴더) 안에 미끼용 파일 `null.c`를 은밀히 박아넣고 (추가로 그 안에 서식하는 `makefile.mk` 지시서도 손을 댔습니다) 모든 함정을 팠습니다.

모든 여정을 [`start.zip`](https://github.com/spamegg1/reviews/raw/master/courses/OSTEP/ostep-projects/vm-xv6-intro/start.zip) 라는 보급품 덩어리를 압축 해제하며 시작하십시오. 덩어리가 풀리면 터미널을 열고 폭풍처럼 `make clean` 과 `make qemu-nox` 를 차례로 때려 박으세요. 마침내 시스템 안에 영혼이 갇히게 되면 `null` 이란 문자를 갈겨보며 그 메모리 지뢰밭의 공포를 눈으로 영접하십시오! 만약 당신이 진짜 변태여서 이 망가진 `null` 덩어리와 실제 기계어 파편의 조각을 현미경으로 대조해 뜯어보고 싶다면, 자비 없이 `objdump -d user/null.o` 를 찍어 누르면 그 처참한 내부 시체가 전부 열거될 것입니다.

참고로 뼛골 아프게도, 당신이 이 저주받은 코드 쪼가리들을 한 줄 한 줄 교정해 나갈 때마다 멍청한 기계는 그걸 자동으로 인지하지 못합니다. 매번 미친 사람처럼 수동으로 지겹게 `make clean` 과 `make qemu-nox` 를 반복하며 부활 의식을 치러야만 할 것입니다.

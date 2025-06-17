감사의 말: [palladian](https://github.com/palladian1)

## xv6 가상 메모리 입문

### 경고:

***이 프로젝트는 현재 사용 가능한 xv6 소스 코드와 일치하지 않으며, 해당 소스 코드에는 이미 이 프로젝트가 구현되어 있습니다!***

[palladian](https://github.com/palladian1)은 위스콘신 대학교 학생의 Github 페이지에서 다른 xv6 소스를 찾아냈습니다. QEMU 실행 파일을 올바르게 찾도록 `Makefile`을 편집해야 했습니다. `user` 폴더에 `null.c`를 추가했으며(거기서 `makefile.mk`도 편집함), 이는 메모리 안전성 부족을 보여줍니다.

[`start.zip`](https://github.com/spamegg1/reviews/raw/master/courses/OSTEP/ostep-projects/vm-xv6-intro/start.zip)에 있는 코드로 시작하십시오. 압축을 풀고 `make clean` 및 `make qemu-nox`를 실행하십시오. 그런 다음 xv6 시스템 내부에서 `null`을 실행하여 안전성 부족을 확인하십시오! `null`의 결과를 실제 기계 코드와 비교하고 싶다면 `objdump -d user/null.o`를 실행할 수 있습니다.

코드를 변경할 때마다 `make clean` 및 `make qemu-nox`를 수동으로 실행해야 할 수도 있습니다.

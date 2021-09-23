# CURL이란?

* curl = Client URL
: 서버와 통신할 수 있는 커맨드 명령어

## 요청 보내기
### options
* -i : 응답 헤더 출력
* -v : 중간 처리 과정, 오류 메시지, 요청 메시지와 응답 메시지를 헤더와 본문을 포함해 전체 출력
* -X : 요청 메소드를 지정 (옵션 없으면 기본값은 GET)
* -H : 요청 헤더를 지정
* -d : 요청 본문을 지정 (옵션 없으면 요청 본문 없음)

#### 예제
``` shell
curl -X GET http://127.0.0.1:3000/api/users/bakyeono
curl -X POST http://127.0.0.1:3000/api/languages/ansi-common-lisp
curl -X PUT http://127.0.0.1:3000/api/resources/1789
```

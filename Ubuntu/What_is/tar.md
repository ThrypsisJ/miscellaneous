## tar command
tar, tar.gz 압축 및 압축해제 명령어

### tar로 압축하기
```shell
tar -cvf [압축파일명.tar] [압축대상폴더]
```

### tar 압축풀기
```shell
tar -xvf [파일명.tar]
```

### tar.gz 압축하기
```shell
tar -zcvf [파일명.tar.gz] [압축대상폴더]
```

### tar.gz 압축풀기
```shell
tar -zxvf [파일명.tar.gz]
```

### 자주 사용하는 option
* -c : 압축
* -x : 압축 풀기
* -z : tar.gz 사용 시 추가
* -C : 경로를 지정
* -p : 파일 권한 저장
* -v : 압축/해제과정 출력
* -f : 파일 이름

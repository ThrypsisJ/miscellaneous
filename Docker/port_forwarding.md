## 외부에서 호스트 IP로 접근 -> 호스트의 00포트가 컨테이너의 00포트로 포워딩 -> 서버 접근
```shell
docker run -it --name {container_name} -p 00:00 {image_name}
```

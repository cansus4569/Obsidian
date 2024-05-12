
참고 URL
[https://server-engineer.tistory.com/764](https://server-engineer.tistory.com/764)

※ 공개키 설정없이 또는 잘못된 password를 이용하여 SSH 접속 시 출력 에러 메세지

> Permission denied (publickey,gssapi-keyex,gssapi-with-mic,password)

ssh 접속시, 패스워드를 입력하지 않고 접속하기 위해서는 아래와 같이 공개키 설정이 필요하다.

필자는 192.168.3.156 서버에서 192.168.7.17 서버로의 공개키를 설정하겠다. (192.168.3.156 → 192.168.7.17)

```
ssh-keygen
ssh-copy-id -i ~/.ssh/id_rsa.pub jun@192.168.60.200
ssh aimir@192.168.7.17
```

![https://blog.kakaocdn.net/dn/bAGJ4R/btqOP4UGT6h/gtjzUCqVMV7wqTBbyvzVMK/img.png](https://blog.kakaocdn.net/dn/bAGJ4R/btqOP4UGT6h/gtjzUCqVMV7wqTBbyvzVMK/img.png)

출처:

[https://server-engineer.tistory.com/764](https://server-engineer.tistory.com/764)

[임대리 개발일지]
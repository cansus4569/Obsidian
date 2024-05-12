
참고 URL
[https://answer-id.com/ko/53830173](https://answer-id.com/ko/53830173)

- 라이브러리 위치 검색

```bash
$ /sbin/ldconfig -p | grep stdc++

libstdc++.so.6 (libc6) => /usr/lib/libstdc++.so.6
```

- 버전 검색

```bash
$ strings /usr/lib/libstdc++.so.6 | grep LIBCXX

GLIBCXX_3.4
GLIBCXX_3.4.1
GLIBCXX_3.4.2
...
```
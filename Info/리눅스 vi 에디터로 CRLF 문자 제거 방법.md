
리눅스는 개행 문자가 LF = ‘\n’ = 0x0A이고,

윈도우는 CRLF = ‘\r’ + ‘\n’ = 0x0D 0x0A 인데,

파일 안에 LF와 CRLF가 섞여있으면 vi 에디터는 CRLF를 ^M으로 표시한다.

:%s/^M//g (^M은 Ctrl + V + M을 입력) 명령을 수행하면 ^M 문자가 제거된다.
### Self Test

1. HTTP/2.22와 HTTP/2.3 중에서 어떤 버전이 더 높은 버전인가?

2. TRACE 메서드로 서버에서 클라이언트에서 보낸 메세지를 본문에 담아서 되돌려 받는 방식으로 요청 메세지가 올바르게 전달되는지 확인하는 이 방법은?

3. HTTP 요청 메시지의 필수 구성 요소가 아닌 것은 무엇인가?

- (1) 시작줄
- (2) 헤더
- (3) 본문
- (4) 캐리지 리턴과 개행 문자

4. HTTP 헤더 **`Content-Length`**의 주요 역할은 무엇인가?

- (1) 메시지 본문의 길이를 바이트 단위로 나타낸다.
- (2) 서버가 응답으로 보낼 파일의 종류를 지정한다.
- (3) 메시지의 캐싱 여부를 결정한다.
- (4) 클라이언트가 요청한 리소스의 최종 수정 시간을 나타낸다.

### CRLF(Carriage Return Line Feed)

HTTP 메세지

```
HTTP/1.1 200 OK\r\n
Date: Wed, 15 Jan 2025 12:00:00 GMT\r\n
Content-Type: text/html\r\n
Content-Length: 137\r\n
\r\n
<html>
  <head>
    <title>Example</title>
  </head>
  <body>
    <p>Hello, World!</p>
  </body>
</html>
```

### (1) **Carriage Return (CR, `\r`)**

- **캐리지를 왼쪽 끝으로 이동**시키는 동작.
- 그러나 종이가 한 줄 올라가지는 않음(즉, 현재 줄의 맨 앞 위치로 이동).
- 타자기에서 캐리지라는 것을 이용해서 줄바꿈을 한다.

### (2) **Line Feed (LF, `\n`)**

- 캐리지는 그대로 둔 상태에서, **종이를 한 줄 위로 이동**시키는 동작.
  - 종이를 한 줄 위로 올려야, 타자기의 펜은 아래 줄 부터 글을 작성할 수 있다.
- 줄바꿈이 이루어지지만, 캐리지는 맨 앞으로 돌아가지 않음.

둘은 타자기에서 유래된 용어기에 아래 영상을 재미로 한번 봐주시면 기억에 잘 남을 것 같습니다.

https://www.youtube.com/watch?v=jDz438iIoCI

https://www.youtube.com/watch?v=02vRo_SCSYk

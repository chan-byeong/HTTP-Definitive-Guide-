1. ssl/tls 계층을 추가함, 기본포트가 443포트임, 비대칭키, 대칭키로 암호화하는 과정이 있음.
2. X - 비밀키가 필요하다.
3. 속도가 비대칭키 보안보다 빠르다. 먼저 https 연결을 할 때 비대칭키를 이용해 암호화를 하고, 인증서를 받는다. 이후 대칭키를 서로 주고 받는다. 데이터를 전송하고 수신할 때에는 대칭키를 이용해 서로 연결한다.
4. O, CONNECT 메서드를 이용해 HTTPS 터널링 프로토콜을 성립해야 한다.
1.  웹 서버
    HTTP 프로토콜을 구현하여 클라이언트의 요청을 처리하고 응답을 반환한다.
    웹 리소스를 관리하여 요청된 정적 또는 동적 콘텐츠를 제공한다.
    웹 서버 관리 기능을 제공하여 설정, 로깅, 보안 기능을 관리한다.

    운영체제  
    컴퓨터 시스템의 하드웨어를 관리하여 메모리, CPU 등의 자원을 운영한다.
    TCP/IP 네트워크 지원을 통해 웹 서버가 네트워크 통신을 수행할 수 있도록 한다.
    웹 리소스를 유지하기 위한 파일 시스템 관리를 수행하여 웹 서버가 파일을 저장하고 읽을 수 있도록 지원한다.
    현재 연산 활동 제어를 위한 프로세스 관리를 통해 웹 서버의 프로세스와 쓰레드를 운영한다.

    TCP 커넥션 관리
    운영체제는 TCP/IP 프로토콜을 처리하고, 커넥션을 열고 닫는 저수준 네트워크 처리를 담당한다.
    웹 서버는 운영체제가 설정한 TCP 커넥션을 활용하여 HTTP 요청을 처리하고, 필요에 따라 커넥션을 유지하거나 닫을 수 있다.

2.  4번

3.  모든 커넥션을 감시하며, 상태 변화가 있을 때만 처리를 수행한다.이 방식은 비동기 방식으로 동작하며, 불필요한 리소스 낭비를 줄일 수 있다.

4.  Reverse DNS (역방향 DNS 조회)

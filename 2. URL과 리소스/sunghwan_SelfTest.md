# 셀프 테스트

1. 상대 URL과 상대 경로를 합치면 찾을 수 있는 절대 URL이 된다 (O / X)
2. URL에서 안전하지 않은 문자는 퍼센티지 기호로 시작하는 이스케이프 문자로 바꾼다. (O / X)
3. 프래그먼트(#)는 서버로 전송되어 한정된 파일만 가져오도록 도와준다 (O / X)
4. 질의 문자열(???=??)의 경우 http 프로토콜에서 서버로 전송되는 URL 중 가장 마지막에 위치한다. (O / X)

# 궁금한 점

websocket의 경우 http로 먼저 연결된 다음 websocket으로 업그레이드하는 데, 이럴 때 스킴을 지키면서 업그레이드 되는걸까?
프레그먼트는 서버로 전달되면 대역폭을 아끼고 클라이언트는 더 빠르게 로딩될 수 있을 텐데 그러지 않았을까?
### 1. 클라이언트의 IP 주소만으로 사용자를 식별하는 것이 어려운 이유는 무엇인가?

- 클라이언트 IP 주소는 동적 IP 할당, 공유 네트워크, 프록시/VPN 사용, NAT(Network Address Translation) 등의 이유로 사용자가 변경될 가능성이 높아 정확한 사용자 식별이 어렵습니다. 따라서 쿠키, 세션, OAuth 토큰과 같은 추가적인 인증 방법이 필요하다.

### 2. 뚱뚱한 URL(Fat URL)을 사용하면 발생하는 보안 문제는 무엇이며, 이를 대체할 수 있는 안전한 방법은 무엇인가?

- 뚱뚱한 URL 방식은 브라우저 히스토리 저장, Referrer(참조 페이지) 노출, 로그 파일 기록, URL 공유 시 세션 유출, 캐싱 문제 등 보안 취약점을 초래한다.
- 이를 방지하기 위해 쿠키 기반 세션 관리(Set-Cookie 사용) 또는 Authorization 헤더를 활용한 토큰 기반 인증을 적용하는 것이 안전한 대안이다.

### 3. 세션 쿠키(Session Cookie)와 지속 쿠키(Persistent Cookie)의 차이점은 무엇이며, 보안을 강화하기 위해 어떤 속성을 추가할 수 있는가?

- 세션 쿠키(Session Cookie)는 브라우저가 닫히면 자동 삭제되기에 Expires나 Max-Age 속성이 없다.
- 지속 쿠키(Persistent Cookie)는 Expires 또는 Max-Age를 설정하여 특정 기간 동안 유지된다.
- 보안을 강화하기 위해 Secure(HTTPS 전용), HttpOnly(JavaScript 접근 차단), SameSite=Strict(CSRF 방지) 등의 속성을 추가하는 것이 좋다.

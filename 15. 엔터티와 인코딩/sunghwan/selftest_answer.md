1. deflate와 같은 압축, chunk encoding 등 (헤더 전송 비용을 아낄 수 있음)
2. 이전에는 커넥션을 닫음으로써 정상적으로 종료처리했지만, 현재는 커넥션을 계속 열어 놓은 상태에서 전송을 하기 때문이다. 파일 혹은 메시지가 어디에서 종료되는 지 알 수 없기 때문이다.
3. Content-Type: multipart/form-data, Content-Type: multipart/mixed
4. Accept-Encoding
5. If-Match / If-None-Match (ETag 기준으로 맞던지 / 틀리다면 사본을 보내라.)
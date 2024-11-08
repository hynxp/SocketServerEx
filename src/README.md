# 소켓 서버 예제

## 구현
- 바닐라 Java 사용
- 소켓 서버 생성
- chrome 브라우저를 통해 해당 서버 접속
- 요청 시 들어온 data 출력 해보기
- 소켓 서버를 생성 후에 클라이언트가 접속
- 요청 바디 내용을 출력해보기
- 이 과정에서 소켓 서버의 생성 플로우를 잘 학습해주시고, 메시지의 내용으로 어떤 내용이 출력되는지 유심히 봐주시면 되겠습니다!

## 클래스
`ServerSocket`: 클라이언트-소켓 연결에서 서버 측의 구현을 제공하는 클래스

`Socket`: 클라이언트 측의 구현을 제공하는 클래스

## 과정
Step 1. Server Socket 생성, 포트 바인딩
Step 2. 클라이언트로부터의 연결을 기다리고(Connect Listen) 요청이 오면 수락
Step 3. 클라이언트 Socket에서 가져온 InputStream(클라이언트 쪽에서는 OuputStream 이 됩니다)을 읽음
Step 4. 응답이 있다면 OutputStream을 통해 클라이언트에 데이터를 보냄
Step 5. 클라이언트와의 연결을 닫음
Step 6. 서버 종료
출처: https://woolbro.tistory.com/29 [개발자 울이 노트:티스토리]
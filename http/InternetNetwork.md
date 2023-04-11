# Internet network

IP - Internet protocol

: IP-address에 데이터 전달, packet이라는 통신 단위로 전달

- 클라이언트 패킷과 서버 패킷의 경로는 서로 다를 수 있다
- 한계
  - 비연결성: 패킷을 받을 대상이 없어도 패킷 전송 가능
  - 비신뢰성: 중간에 패킷 소실 가능, 패킷 전달 순서 문제 발생 가능

-----

TCP - Transmission control protocol

: 전송 제어 프로토콜

- 연결지향 - TCP 3 way handshake(가상 연결)
- 데이터 전달 보증 -> 데이터를 전송하고 잘 받았다는 신호를 보낸다.
- 순서 보장 -> 패킷이 순서대로 오지 않으면 다시 보내라는 요청을 보낸다.
- 신뢰 가능한 프로토콜!!



인터넷 프로토콜 스택의 4계층

- 애플리케이션 계층 - HTTP, FTP
- 전송 계층 - TCP, UDP
- 인터넷 계층 - IP
- 네트워크 인터페이스 계층



TCP 3 way handshake

1. SYN: 접속 요청

2. SYN + ACK

3. ACK: 요청 수락



UDP - User datagram protocol

: 사용자 데이터그램 프로토콜

- 기능이 거의 없음
- 연결 지향!! -> 3 way handshake X
- 데이터 전달 보증 X
- 순서 보장 X
- 단순하고 빠름
- IP와 비슷

-----

PORT

: IP가 겹치는 여러가지 패킷에 대해 프로세스로 구분해주는 것

- 패킷 정보에는 IP주소와 PORT 번호가 같이 저장
- 0~65535 할당 가능
- 0~1023 잘 알려진 포트 -> 사용하지 않는 것이 좋음
  - FTP - 20, 21
  - Telnet - 23
  - http - 80
  - https - 443

-----

DNS - Domain name system

: IP 주소와 기억하기 쉬운 domain 이름을 매칭해주는 시스템

- IP는 기억하기 어려우며 언제든 변경 가능
- dns에서 해당 도메인으로 요청이 들어오면 IP로 매칭시켜준다
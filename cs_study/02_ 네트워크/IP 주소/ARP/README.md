# ARP

## IP 주소로 부터 MAC 주소를 구하는 IP와 MAC 주소의 다리 역할을 하는 프로토콜

1. 컴퓨터와 컴퓨터의 통신은 무엇을 기반으로 하는 걸까?

- IP 주소에서 ARP를 통해 MAC 주소를 찾아, MAC 주소를 기반으로 통신한다.
- ARP를 통해 가상 주소인 IP 주소를 실제 주소인 MAC 주소로 변환
- RARP를 통해 실제 주소인 MAC 주소를 가상 주소인 IP 주소로 변환

2. Example

- 장치 A가 ARP Request 브로드캐스트를 보낸다.
- IP 주소인 120.70.80.3에 해당하는 MAC 주소를 찾는다
- 해당 주소에 맞는 장치 B가 'ARP reply 유니캐스트'를 통해 MAC 주소를 변환
- IP 주소에 맞는 MAC 주소를 찾는다

### **브로드캐스트**

> 송신 호스트가 전송한 데이터가 네트워크에 연결된 모든 호스트에 전송되는 방식

### **유니캐스트**

> 고유 주소로 식별된 하나의 네트워크 목적지에 1:1로 데이터를 전송하는 방식

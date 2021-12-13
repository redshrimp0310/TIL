<img src="https://images.unsplash.com/photo-1542382257-80dedb725088?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1228&q=80" width="50%" height="50%"></img><br/>

NETWORK BASIC
=============

### 포트포워딩이란?
포트 매핑이라고도 불리며 NAT의 응용이다.
하나의 IP주소와 포트 번호이 결합이 게이트웨이를 지나면서 다른 주소와 포트 번호의 결합으로 변환 되는 기술을 말한다.
- - -
### 공인 IP와 사설 IP란?
공인 IP는 유일한 네트워크 주소로서 인터넷에서 사용된다. 사설 IP 주소는 내부네트워크에서 사용된다. 공인 IP와 사설 IP를 이용하면 IPv4의 주소 개수 부족과 보안상의 문제를 해결해 줄수 있다.
- - -
### 게이트웨이란?
다른 네트워크로 가기 위한 문이다.
- - -
### NAT이란?
Network Address Translation 의 약자로 라우터에 설정해 IP주소와 포트 숫자의 변환을 통해 IPv4의 주소 부족 문제와 보안성을 향상시키기 위해 고안되었다.
- - -
### Port Forwarding과 Port Triggering의 차이?
둘은 비슷하지만 다르다. Port Forwarding은 특정 IP를 설정하여 외부 패킷이 들어오면 IP를 지정하여준 특정 PC로 패킷을 Forwarding 할수 있게 도와주는 반면 Port Triggering은 내부 네트워크의 
여러 PC중 특정 예약포트를 감지되면 특정포트를 먼저사용한 PC로 사용포트를 포트포워드해주는 기능이다.
- - -
### 왜 공인 IP 주소를 이용하여야 하나요?
Router는 다른 네트워크를 연결해 주는 기기이며 라우터를 기점으로 라우터 외부와 라우터 내부는 다른 네트워크이다. 즉, 라우터 내부의 네트워크 주소를 알아야 외부에서 내부로 접속이 가능하다. 
하지만, 보안상의 이유로 내부 IP는 외부로 알려져서는 안된다. 또한 공인IP와 사설IP로 나누어 외부에서는 공인IP만 보이게 한다면 IPv4의 주소 부족 문제도 어느정도 해결할수 있다. 
- - -
### ISP란?
Internet Service Provider. 쉽게 생각해 KT와 SKT 같은 인터넷 서비스 제공업체이다.
- - -
### Virtual Server vs Port Forwarding?
둘다 동일한 기술이다.
- - - 
### 참고
* https://ooeunz.tistory.com/104
* https://m.blog.naver.com/firstpw/221696768532
* https://ko.natapa.org/difference-between-port-forwarding-and-port-triggering-556

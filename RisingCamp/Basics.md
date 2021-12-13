<img src="https://images.unsplash.com/photo-1513506003901-1e6a229e2d15?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MXx8YmFzaWN8ZW58MHx8MHx8&auto=format&fit=crop&w=500&q=60" width="50%" height="50%" title="Basics" alt="Basics"></img>

BASICS
======

### Domain과 DNS?
도메인은 인터넷에 연결된 컴퓨터의 IPv4주소를 사람이 쉽게 기억하고 입력할 수 있도록 문자로 만든 인터넷주소이다.
DNS는 Domain Name System의 줄임말로서 Domain과 IPv4를 서로 변환해주는 체계를 말한다.
- - -
### let's encrypt란?
Certificate Authority (CA). 즉, 인증기관으로 보다 쉬운 방법과 무료로 TLS/SSL 인증서를 발급해서 HTTPS 통신을 가능하게 해주는 서비스 기관이다.
- - -
### TLS/SSL 인증서란?
SSL(Secure Sockets Layer)은 1999년 TLS(Transport Layer Security)이전의 인터넷 통신을 통한 보안을 제공하기 위해 가장 널리 배포 된 암호화 프로토콜이었다.
SSL 프로토콜의 사용이 중단되고 대신 TLS가 채택되었지만 사람들은 여전히 이 유형의 기술을 'SSL'이라고 한다. SSL은 인터넷 또는 내부 네트워크를 통해 
작동하는 두 컴퓨터 또는 장치간에 보안 채널을 제공하며, 일반적인 예로는 "SSL을 사용하여 웹 브라우저와 웹 서버 간의 통신을 보호"하는 경우다.
웹사이트에 SSL인증서를 사용하게 되면, 웹 사이트 주소가 HTTP에서 ‘보안’을 의미하는‘S’가 추가되어 HTTPS 로 통신할 수 있다.
- - -
### certbot이란?
Let's Encrypt 인증서를 자동으로 발급 및 갱신을 해주는 봇 프로그램이다.
- - -
### 서브도메인이란?
서브도메인은 말 그대로 우리가 사용하는 도메인의 하위 도메인이다. CNAME 레코드나 A 레코드로 하위도메인을 추가할 수 있다. 
- - -
### 참고
* https://opentutorials.org/module/288/2802
* https://ko.wikipedia.org/wiki/Let's_Encrypt
* https://www.ucert.co.kr/ssl/info
* https://elfinlas.github.io/2018/03/19/certbot-ssl/
* https://cgntv.tistory.com/entry/%EC%84%9C%EB%B8%8C-%EB%8F%84%EB%A9%94%EC%9D%B8%EC%9D%B4%EB%9E%80

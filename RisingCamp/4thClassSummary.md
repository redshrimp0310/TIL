<img src="https://images.unsplash.com/photo-1610072947120-8736bbfc56e1?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=730&q=80" 
     width="60%" height="60%"></img><br/>

4th Rising Camp Class
=====================

### 잘 짜여진 좋은 쿼리란?
Application Server에서 SQL문을 실행하였을 때 이 SQL문은 DB로 보내어 지고 DB에서 **SQL파싱** 그리고 **옵티마이징**을 거쳐 데이터를 찾고 가공하여 우리들에게 보여지게 된다. 그렇다면, 잘 짜여진 좋은
쿼리란 위의 일련의 과정을 가장 빠르게 소화할 수 있는 쿼리일것이다.

*여기서 **SQL파싱**이란 SQL문법체크 및 SQL문이 DB에서 실행되어질 수 있는 형태로의 가공해 주는 것을 말한다.
그리고 **옵티마이징**이란 가장 데이터를 빠르고 잘 찾을 수 있는 방법을 찾아내는 것을 말한다.*
- - -
### 일반적으로 서브쿼리를 조인문으로 바꾸면 속도가 향상 된다는 인식이 있다.
*서브쿼리란? </br> 아래와 같이 하나의 SQL 문에 포함되어 있는 또 다른 SQL 문을 말한다.*
```
SELECT C1, C2, C3
FROM T1
WHERE C1 = (SELECT C1
            FROM T2
            WHERE C2 = '3')
ORDER BY C1, C2, C3;
```
- - - 
### 외래키 사용의 단점?
* 관리의 비용 문제가 생긴다. </br> 부모 테이블의 구조를 변경해야 하는 경우 자식테이블의 구조에 이상이 없을지 다 확인해야 한다.
* 실행계획을 제어할 수 없다. </br> DBA라면 DB를 제어할 수 있어야 하고 실행계획을 제어할 수 있어야 합니다. 즉, 쿼리가 언제 끝나는지, 수행하면서 이슈는 없는지에 대해 파악 할 수 있어야 하는데, 외래키를 사용하면 제어가 힘들다.
</br></br>
**하지만 외래키 사용여부는 외래키의 장점들도 고려하여 각각의 DB 설계에 따라 회사의 정책에 따라 결정하면 된다.**
- - -
### API란?
Application programming interface의 약자로 프로그램들이 서로 상호작용하는 것을 도와주는 매개체이다. 비유를 들어보면, 레스토랑에 있는 점원이라고 생각해 볼 수 있다. 점원은 손님에게 메뉴를 알려주고, 주방에 주문받은 요리를 요청 한 후 주방에서 완성된 요리를 손님께 다시 전달한다. 
API는 손님(프로그램)이 주문할 수 있게 메뉴(명령 목록)를 정리하고, 주문(명령)을 받으면 요리사(응용프로그램)와 상호작용하여 요청된 메뉴(명령에 대한 값)를 전달한다.
</br>즉, API는 다음과 같은 역할을 한다. 

1. API는 서버와 데이터베이스에 대한 출입구 역할을 한다.
: 데이터베이스에는 소중한 정보들이 저장된다. 모든 사람들이 이 데이터베이스에 접근할 수 있으면 안 되므로 API는 이를 방지하기 위해 서버와 데이터베이스에 대한 출입구 역할을 하며, 허용된 사람들에게만 접근성을 부여해준다.
2. API는 애플리케이션과 기기가 원활하게 통신할 수 있도록 한다.
: 여기서 애플리케이션이란 우리가 흔히 알고 있는 스마트폰 어플이나 프로그램을 말한다. API는 애플리케이션과 기기가 데이터를 원활히 주고받을 수 있도록 돕는 역할을 한다.
3. API는 모든 접속을 표준화한다.
API는 모든 접속을 표준화하기 때문에 기계/운영체제 등과 상관없이 누구나 동일한 액세스를 얻을 수 있다. 쉽게 말해, API는 범용 플러그처럼 작동한다고 볼 수 있다.
- - -
### HTTP 특성?
* Client - Server 
* 캐시를 달아 줄 수 있다.
* 상태없음 (Stateless) : 서버는 클라이언트를 식별할 수가 없는 상태
* 비연결성 (Connectionless) : 클라이언트와 서버가 한 번 연결을 맺은 후, 클 라이언트 요청에 대해 서버가 응답을 마치면 맺었던 연결을 끊어 버리는 성질.
- - -
### REST API란?
여기서 REST는 'Representational State Transfer' 의 약자이며 HTTP URI(Uniform Resource Identifier)를 통해 자원(Resource)을 명시하고, HTTP Method(POST, GET, PUT, DELETE)를 통해 해당 자원에 대한 CRUD Operation을 적용하는 것을 의미한다. 그럼 REST API란, REST 기반으로 서비스 API를 구현한 것을 말한다.
</br></br> **REST 특징**
* Server-Client 구조
* Stateless
* Cacheable
* Layered System
* Code on demand(Optional)
* Uniform Interface
</br>또한, 우리가 RESTful이란 표현을 사용하는데, RESTful은 일반적으로 REST라는 아키텍처를 구현하는 웹 서비스를 나타내기 위해 사용되는 용어이다.
‘REST API’를 제공하는 웹 서비스를 ‘RESTful’하다고 할 수 있다.
RESTful은 REST를 REST답게 쓰기 위한 방법으로, 누군가가 공식적으로 발표한 것이 아니다.
즉, REST 원리를 따르는 시스템은 RESTful이란 용어로 지칭된다.
- - -
### 참고
* https://velog.io/@ggomjae/%EC%BF%BC%EB%A6%AC-%EC%84%B1%EB%8A%A5-%EC%A7%84%EB%8B%A8%EC%9D%80-%EC%B5%9C%EC%A0%81%ED%99%94%EC%9D%98-%EA%B8%B0%EC%B4%88#%EC%8B%9C%EC%9E%91
* https://mozi.tistory.com/233
* https://mozi.tistory.com/344
* http://blog.wishket.com/api%EB%9E%80-%EC%89%BD%EA%B2%8C-%EC%84%A4%EB%AA%85-%EA%B7%B8%EB%A6%B0%ED%81%B4%EB%9D%BC%EC%9D%B4%EC%96%B8%ED%8A%B8/
* https://victorydntmd.tistory.com/286
* https://gmlwjd9405.github.io/2018/09/21/rest-and-restful.html

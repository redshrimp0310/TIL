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

### 참고
* https://velog.io/@ggomjae/%EC%BF%BC%EB%A6%AC-%EC%84%B1%EB%8A%A5-%EC%A7%84%EB%8B%A8%EC%9D%80-%EC%B5%9C%EC%A0%81%ED%99%94%EC%9D%98-%EA%B8%B0%EC%B4%88#%EC%8B%9C%EC%9E%91
* https://mozi.tistory.com/233
* https://mozi.tistory.com/344

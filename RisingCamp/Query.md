<img src="https://images.unsplash.com/photo-1489875347897-49f64b51c1f8?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MXx8cXVlcnl8ZW58MHx8MHx8&auto=format&fit=crop&w=500&q=60" 
     width="60%" height="60%"></img><br/>

QUERY
=====

### Inner Join과 Outer Join?
쉽게 말하자면 inner join은 교집합 그리고 outer join은 합집합이라고 할 수 있다.
inner join은 같은 컬럼 값을 가질 경우에만 조인이 가능하다.
outer join에는 left join과 right join이 있는데 left join은 왼쪽 테이블을 기준으로 right join은 오른쪽 테이블을 기준으로 join하는것이다.
inner join과 달리 같은 컬럼 값을 가지지 않는 경우에도 조인이 된다.
- - -
### MySQL CASE문?
프로그래밍 언어에서 스위치(switch)문과 비슷하다. 

아래와 같이 사용한다.
CASE
	WHEN 조건
	THEN 반환 값
	WHEN 조건
	THEN 반환 값
	ELSE 위의 WHEN 조건들에 해당 안되는 경우 반환 값
END

ELSE가 없고, 조건에 맞지 않아서 반환 값이 없으면 NULL를 반환한다.
- - -
### 참고
* https://jetalog.net/28
* https://extbrain.tistory.com/46

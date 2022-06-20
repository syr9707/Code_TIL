# 코딩테스트에 대한 나의 공부 기록 



[마법의 슈퍼마리오](https://m.blog.naver.com/PostList.naver?blogId=kks227) 블로그를 참조하자! 

[박트리](https://baactree.tistory.com/14) 블로그 역시! 



## 동빈나의 Tip! 

> [동빈나 유튜브 참조](https://www.youtube.com/watch?v=ukkLCl9yBvE)



### 백준 문제 풀기

1. 그리디
2. 탐색
   * 완전 탐색
   * BFS
   * DFS

3. 기본 동적 프로그래밍 

---> 각각 50 문제씩 

3. 삼성전자 역량 테스트 

* 그래프 이론
* 중급 및 고급 동적 프로그래밍 
* 문자열 



### 프로그래머스

1. 카카오 기출



----------------------------------------------------



**코드포스 블루레벨 정도면 코딩테스트 합격 가능**

**또는 삼성 역량 테스트 B형**



---------------------------------------



## 알고리즘 초급

* 완전 탐색
* DP(Dynamic Programming) 초급
* 큐, 스택
* DFS
* BFS
* 탐욕법



## 알고리즘 중급

* 분할 정복 
* 이분 탐색
* DP 중급
* 등등... 



------------------------------------------------------



## 개념 

### StringTokenizer 클래스란?

> 하나의 문자열을 여러 개의 토큰으로 분리

**사용법**

```java
1. StringTokenizer st = new StringTokenizer(문자열);
---> 띄어쓰기 기준으로 문자열을 분리
    
2. StringTokenizer st = new StringTokenizer(문자열, 구분자);
---> 구분자를 기준으로 문자열을 분리

3. StringTokenizer st = new StringTokenizer(문자열, 구분자, true/false);
---> 구분자를 기준으로 문자열을 분리할 때, 
	구분자도 토큰으로 넣을 지(true),
	구분자는 분리된 문자열 토큰에 포함 안 시킬 지(false)
   * 디폴트 : false 
```



**예제**

```java
String str = "IT 블로그 추천 -홍길동의 블로그:www.asvdsasa.com";
StringTokenizer st = new StringTokenizer("-:");

while(st.hasMoreTokens()) {
    System.out.println(st.nextToken());
}
```

*구분자는 하나의 문자로 구성될 필요는 없다*



* hasMoreTokens() : 남아있는 토큰이 있다면 true 리턴, 아니면 false
* nextToken() : 객체에서 다음 토큰을 반환



### 삼항 연산자

> 변수 = (조건문) ? (true일 때의 연산) : (false일 때의 연산);

---> 속도가 빨라지는 것은 아님




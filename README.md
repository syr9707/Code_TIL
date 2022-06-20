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

### 입출력 (BufferedReader)

> BufferedReader는 엔터만 경계로 인식 --> 받은 데이터 String으로 고정 (다른 타입 입력 받을 시 형변환!)
>
> BufferedReader를 사용하는 것이 Scanner를 사용하는 것보다 빠름
>
> readLine() 사용 시 : 예외처리 필수! 



**종합 활용법 예제 : (배열 크기) (배열 숫자들...)**

```java
BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
int N = Integer.parseInt(st.nextToken()); // 배열 크기 받기
int[] arr = new int[N];

StringTokenizer st = new StirngTokenizer(br.readLine());
for(int i = 0; i < N; i++) {
    arr[i] = Integer.parseInt(st.nextToken());
}

br.close(); 
```



**BuffrerdReader 사용법**

```java
BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
Strng input = br.readLine();
```

**int 타입 받을 시** 

```java
BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
int i = Integer.parseInt(br.readLine());
```

**또 다른 예제 : 공백 단위로 데이터 가공**

```java
BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
StringTokenizer st = new StirngTokenizer(br.readLine());
int N = Integer.parseInt(st.nextToken());
int M = Integer.parseInt(st.nextToken());
```





### StringTokenizer

> StringTokenizer가 BufferedReader보다 빠르게 사용 될 수 있음

**예제**

<StringTokenizer 사용>

```java
BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
StringTokenizer st = new StirngTokenizer(br.readLine());

String A = st.nextToken();
String B = st.nextToken();
String C = st.nextToken();
String D = st.nextToken();
```



<BufferedReader 사용>

```java
BufferedReader br = new BufferedReader(new InputStreamReader(system.in));
String[] input = br.readLine().split(" ");
```



### split() 

> 문자열 구분

**사용법 (예제)**

```java
String str = "alksjdalkfj@jsdaklfj";
String[] strAry = str.split("@");

for(String s : strAry) 
    System.out.println(s);
```



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




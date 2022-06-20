# 자주 사용 하는 것들

## import

> 런타임 속도는 영향을 미치지 않음! (컴파일 속도는 느려짐)

```java
import java.util.*;
import java.io.*;
```



## 입출력 (BufferedReader)

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



## sort

> 숫자 배열의 정렬 : 숫자 크기 순으로 정렬 

```java
int[] arr = {1, 3, 4, 5, 6};
Array.sort(arr);
```



## Math

> answer을 항상 최고값으로 사용할 때

```java
int answer = 1;
ansser = Math.max(answer, 100);
// answer : 10
```



## 
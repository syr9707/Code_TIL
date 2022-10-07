# Java 자주 쓰는 것들, 새로 알게된 것들

### 1. Integer.toBinaryString(n); 
> 10진수 -> 2진수 String
``` java
int n = 78;
String str = Integer.toBinaryString(n);
System.out.println(str);

// 결과 : 1001110 
```

### 2. int bitCount = Integer.bitCount(n);
> binary로 변환후, 1의 수를 반환
``` java
int n = 78;
int bitCount = Integer.bitCount(n);
System.out.println(n);

// 결과 : 4 
```
``` java
// 예제 2 : n과 1의 개수가 같은 숫자 중 바로 다음 큰 수 
int n = 78;
int bitCount = Integer.bitCount(n);

for(int i = n + 1; ; i++) {
    if(Integer.bitCount(i) == bitCount) {
        answer = i;
        break;
    }
}
```
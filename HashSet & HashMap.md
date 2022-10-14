## ⭐ HashMap
* 키는 맵에 오직 유일
* 값은 중복되어도 상관 없음

예제
```java
import java.util.HashMap;
import java.util.Map;
public class Main {
	public static void main(String[] ar) {
		Map<String,Integer> map=new HashMap();	//<키 자료형, 값 자료형>
		map.put("A", 100);
		map.put("B", 101);
		map.put("C", 102);
		map.put("C", 103); //중복된 key가 들어갈때는 이전 키,값을 지금의 것으로 업데이트
		System.out.println(map);
		System.out.println(map.get("A"));
		System.out.println(map.get("B"));
		System.out.println(map.get("C"));
	}
}

// 결과
/*
{A=100, B=101, C=103}
100
101
103
*/
```
```java
//Map 안에 값 넣기
Map.put(key,value);

//Map 안의 값 가져오기
Map.get(key);

//Map 크기 확인
Map.size();

//Map 안의 내용 변경하기
Map.replace(key, value);

//Map 안에 특정 Key, Value 들었는지 확인
Map.containsKey(key);
Map.containsValue(value);

//Map의 크기가 0인지 확인
Map.isEmpty();

//Map 안의 내용 삭제
Map.remove(key);
```

## ⭐ HashSet
* 이 클래스의 가장 큰 특징은 중복을 허용하지 않는다는 것 
```java
import java.util.HashSet;
import java.util.Iterator;

public class HashSetTest {
	public static void main(String[] args)  {	
		// Integer
		HashSet<Integer> set = new HashSet<Integer>();	
		
		set.add(1);
		set.add(2);
		set.add(3);
		set.add(1);
		System.out.println("set의 값 : " + set);
				
		// String
		HashSet<String> set2 = new HashSet<String>();

		set2.add("a");
		set2.add("b");
		set2.add("c");
		set2.add("a");
		System.out.println("set2의 값 : " + set2);
		
		// Integer 출력
		Iterator iter = set.iterator();
		while(iter.hasNext()) {
			System.out.print(iter.next() + " ");
		}
		
		System.out.println("");

		// String 출력
		Iterator iter2 = set2.iterator();
		while(iter2.hasNext()) {
			System.out.print(iter2.next() + " ");
		}
	}
}

// 결과
/*
set의 값 : [1, 2, 3]
set2의 값 : [a, b, c]
1 2 3 
a b c 
*/
```
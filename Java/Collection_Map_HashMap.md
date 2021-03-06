# HashMap

## HashMap
Map의 인터페이스를 구현한 대표적인 Map 컬렉션으로서, 엔트리(Entry)객체를 저장하는 자료구조로 키 객체의 해시코드를 이용한다.
HashMap 이름대로 해싱(Hashing)을 사용하기 때문에 많은 양의 데이터를 검색하는 데 있어서 뛰어난 성능을 보입니다.

## 해싱이란   
데이터를 Key, value값으로 저장하는 구조의 해시테이블에 저장을 해서,   
하나하나 값을 비교하면서 검색을 하는 것이 아닌,   
키에 산술적인 연산을 적용하여 항목이 저장되어 있는 테이블의 주소를 계산하여 항목에 접근하는 것.

## 사용이유
HashMap은 삽입, 검색에 시간복잡도 O(1)이다.
즉 성능이 빠르기 때문이다.

## 예제
- HashMap 선언
```
HashMap<키 자료형, 값 자료형> map이름 = new HashMap<키 자료형, 값 자료형>();

HashMap<String, String> mapA = new HashMap<String, String>(); // 예시
```

- 값 추가
```
변수 이름.put(Key, Value);

mapA.put("1", "Hi"); //예시
```

- 해당 키 삭제
```
Map이름.remove("키");
```

- 모든 값 제거
```
Map이름.clear();
```

## 그 외의 메소드
- isEmpty()    
HashMap에 element가 있는지를 판단한다.   
없으면 true, 있으면 false를 반환한다.
   
- containsKey(Object Key)    
Map의 엘리먼트 중 Key를 포함하고 있는지 여부를 확인한다.

- containsValue(Object value)      
인자로 주어진 Value를 가진 Key가 현재 HashMap에 존재하는지를 판단하여 boolean값을 반환한다

- size()     
HashMap에 저장된 엘리먼트의 개수를 반환한다.

- clone()    
해당 Map의 엘리먼트를 복제한다.

- get(Object Key)      
get은 Key값에 대한 엘리먼트를 가져온다.

- putAll()    
Map에 해당하는 모든 요소를 HashMap에 저장한다.

- replace()    
키값과 바꿀 값을 제공하면 해당 키의 값을 변경한다.

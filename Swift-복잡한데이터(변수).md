# 복잡한데이터

- 배열array
-> 여러 값을 한꺼번에 묶어서 사용하는 타입
-> typealias를 사용해서 데이터 구조를 나타낼수 있습니다.

```sh
typealias PersonTuple = (name : String, age : Int)
let eric : PersonTuple = ("eric", 150)
```

- 연관된 항목들 중에 하나 enum
-> 추후에 다를 경우에 다시 정리하겠습니다.

#### 한꺼번에 많은 값을 담아보자

- 배열 array
-> 동일한 데이터 타입을 연속해서 담아놓고 순서대로 접근하는 콜렉션

```sh
var ageArray = [10, 20, 30, 40, 50]
print(ageArray[0])
```
이 경우에는 ageArray의 첫번째 값인 10이 출력됩니다.

- 사전 dictionary
-> 동일한 데이터 타입을 키값과 함께 담아놓코 키값으로 접근하는 콜렉션

```sh
var gradeDic = ["a" : 90, "b" : 80, "c" : 70, "d" : 60]
print(grade["a"])
```

이 경우에는  gradeDic의 "a" 값인 90이 출력이 됩니다. 하지만 만약 "a" 값이 nil일때 default값을 출력하고 싶다면 어떻게 할까요?

```sh
print(grade["a"] ?? default값)
```

이렇게 한다면 "a" 값이 nil값이였을때 옆에 설정해둔 default값이 대신 출력 됩니다.

- 집합 set
-> 동일한 데이터 타입을 순서없이 집합에 담아놓고 포함되어 있는지 확인하는 콜렉션
```sh
var aSet: set = [11, 12, 13]
aSet.contains(12)
```
포함되 있을 경우 true 아니면 false 값이 출력이 됩니다.

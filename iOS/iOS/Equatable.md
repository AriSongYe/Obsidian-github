Equatable [[protocol]]에 대해 알아봅시다.

우리가 흔히 사용하는 가장 기본적인 자료형들은
[[String]], [[Int]], [[Double]] 안에는 [[Swift]] 언어에서 이미 모두 채택되어 컴파일러가 자동으로 구현합니다.

Equatable protocol의 역할은 이러한 자료형들간 비교를 위해서 사용됩니다.
```
let A : Int = 1
let B : Int = 2
if (A == B) {
	print(정답입니다)
}
else {
	print(오답입니다)
}
```

이렇게 우리가 흔히 사용하는 [[Type]] 간에 비교 연산을 가능하게 만드는 protocol이 Equatable protocol 입니다!

Equatable 을 채택하면 기본 자료형을 넘어 [[struct]], [[Class]], [[Enum]] 등에서도 사용될 수 있습니다.

Equatable안에 [[Method]]를 구현하는 방법과 구현하지 않는 방법 2가지 사용법이 있습니다. 함께 살펴봅시다.

1. Method 구현 X
- [[Value Type]]인 struct은 Equatable을 채택하는 것으로 그 구조체 안에 [[Property]] 값들이 다 동일 하다면 같은 값으로 볼 수 있습니다.
- [[Reference Type]] 인 Class는 채택을 해도 자동으로 구현하지 않기 때문에 Method를 구현해야 합니다.
- 
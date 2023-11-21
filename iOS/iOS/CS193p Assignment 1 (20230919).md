## Swift tour

https://docs.swift.org/swift-book/documentation/the-swift-programming-language/guidedtour/

**Swift doc**를 **읽고 따라가는 것**이 과제입니다.

**Experiment**는 PlayGround를 통해 테스트 해보면 됩니다.
**따로 정답은 적어놓지 않았습니다!**
___ 
### 1.1 Introducing, Hello world

```
print("hello world!")
```
C나 C++에 익숙하다면 당연하게
<stdio.h> Library를 import or include 하여
print를 해야할 것만 같다.
하지만 Swift에서는 import의 필요도 main()문을 작성할 필요도 없다.

### 1.2 Simple Value
___ 
**변수**와 **상수**에 대해 알아보자

[[Constant]] (상수)
반드시 컴파일할 때 Constant 값을 알려줄 필요는 없지만
Constant 값은 반드시 한 번만 할당되어야 한다.

```
var myVariable = 42
myVariable = 50
let myConstant = 42
```

[[Type]]
Type을 명시할 필요가 없다.
Compiler가 알아서 Type을 infer(추론)하기 때문에 별다른 명시를 하지 않아도
추론과정을 통해 Type을 정의내려서 컴파일한다.

```
let implicitInteger = 70
let implicitDouble = 70.0
let explicitDouble: Double = 70
```

> **Experiment** **1.2.1**
> Create a constant with an explicit type of `Float` and a value of `4`.

[[Type Casting]], Convert to another type

```
let label = "The width is "
let width = 94
let widthLabel = label + String(width)
```

만약 타입 캐스팅을 원한다면 다음과 같은 방법으로 새로운 Instance를 만들어서 변환해주면 된다.

>**Experiment 1.2.2**
>Try removing the conversion to `String` from the last line. What error do you get?

Type Casting, **Convert to String type easily** , '\\(You want)'

```
let apples = 3
let oranges = 5
let appleSummary = "I have \(apples) apples."
let fruitSummary = "I have \(apples + oranges) pieces of fruit."
```

쉽게 String으로 타입 변환을 backslash'\\' + Parentheses '()' 를 통해 바꿀 수 있다.

> Experiment 1.2.3
> Use `\()` to include a floating-point calculation in a string and to include someone’s name in a greeting.
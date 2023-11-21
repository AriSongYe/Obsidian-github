### 1.2 Simple Value
**Multiple Lines을 String으로 만들고 싶을 때**
```
"""
A
B
C \(Apple + Orange)
D
"""
```
- Double Quotation 3개를 연달아 사용하면 여러 줄의 문자열을 만들 수 있다.

**Create Arrays**
```
var fruits = ["strawberries", "limes", "tangerines"]
fruits[1] = "grapes"
var occupations = [ "Malcolm": "Captain", "Kaylee": "Mechanic", ] occupations["Jayne"] = "Public Relations"
```
- Array를 만드는 법은 \[] square brakets(대괄호) 를 사용하면 된다.
- index, key 값으로 배열에 접근할 수 있다.
- 마지막에 콤마를 넣는 것도 허용이 됩니다.

```
fruits.append("blueberries")
print(fruits)
```
- .append method를 통해 배열에 요소를 넣을 수 있따.

빈 배열을 선언할 때는 Type 명시가 필요합니다.
```
let emptyArray: [String] = []
let emptyDictionary: [String: Float] = [:]
```

### Control Flow
프로그램의 흐름을 제어하기 위하여
조건문, 반복문은 기본적으로 {}를 통한 [[Body]]를 필요로 합니다.

**if** 문
if문은 조건부에 값은 boolean 값으로 표현 되어야 합니다.
- 0과 0이 아닌 값으로 되는가? 
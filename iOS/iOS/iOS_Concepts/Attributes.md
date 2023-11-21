## attribute란, 선언과 타입에 부가적인 정보를 제공하는 것입니다.
___ 
Swift 에는 두 종류의 속성(attributes)이 있습니다.

## 1. [[Declaration]]에 적용하는 속성
___ 
[[Function]], [[Class]], [[struct]], [[Enum]] 
### 형태
```
@attribute명
```

### **E.g)**
```
@discardableResult
func test() {
return "apple" }
test()
```

[[@discardableResult]],


## 2. [[Type]] 에 적용하는 속성
___


### E.g)
___
[[@autuclosure]], [[@convention]], [[@escaping]], [[@sendable]]


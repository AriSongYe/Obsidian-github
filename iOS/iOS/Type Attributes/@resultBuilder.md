**Swift 5.4에서부터 도입된 개념으로 컴마(,) 없이 배열을 구성하는 기능에 사용합니다.**

즉, 해당 프로퍼티 래퍼로 선언하면 필요한 buildBlock 메서드를 정의해야합니다.

```
@resultBuilder
struct SimpleStringBuilder {
	static func buildBlock(_ parts: String...) -> String {  
		parts.joined(separator: "\n")
	}
}
```
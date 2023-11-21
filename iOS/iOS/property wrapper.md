  
Property Wrapper 는 Swift 5.1 에 추가되었습니다.

프로퍼티 래퍼(Property Wrapper)는 Swift에서 프로퍼티의 값을 감싸고(wrap) 관리하며
값을 설정하거나 읽을 때 원하는 동작을 수행하도록 도와주는 기능입니다
이를 통해 코드 재사용성을 높이고 중복을 줄이며, 프로퍼티의 값을 보다 안전하게 처리할 수 있습니다.

> 핵심은 변수에 중복되는 코드를 proper wrapper를 통해 재사용성을 줄이는 것입니다

### Declaration
```
@propertyWrapper

struct NewPropertyWrapper {

    private var value : Int

    init() {

        value = 0

    }

    var wrappedValue: Int {

        get { return value}

        set { value = min(max(0, newValue), 100)}

    }

}
```
다음과 같이 Property Wrapper를 선언하여 사용할 수 있습니다

### Usage
```
struct MyStruct {

    @NewPropertyWrapper var value : Int

}
```

다음과 같이 우리가 사용하던 [[@State]] 등과 같은 Property Wrapper들을 선언하여 사용하면 됩니다.

### Advantages

사용하는 이점을 코드로 명확히 살펴 봅시다
```

struct SmallRectangle {
    private var _height = TwelveOrLess()
    private var _width = TwelveOrLess()
    var height: Int {
        get { return _height.wrappedValue }
        set { _height.wrappedValue = newValue }
    }
    var width: Int {
        get { return _width.wrappedValue }
        set { _width.wrappedValue = newValue }
    }
}
```

다음과 같은 변수가 반복될 경우 비효율적임을 알 수 있다.
```
struct SmallRectangle {
    @TwelveOrLess var height: Int = 2
    @TwelveOrLess var width: Int = 200
}
```

미리 선언된 @TwelbeOrLess 라는 Property Wrapper를 사용하면 다음과 같이 코드를 간략화 할 수 있다.
### Condition
- local stored variable 에서만 사용가능
- (global variable 또는 computed variable 에서 사용불가)

### Global Variable Error

![[property wrapper globalValue Error img.png]]

### Computed Property Error

![[property wrapper computed property error img.png]]


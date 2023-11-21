  
Structure(구조체)는 프로그래밍에서 사용되는 사용자 정의 [[DataType]] 중 하나로, [[Data]]의 구조를 정의하는 데 사용됩니다. 구조체는 다양한 데이터를 단일 단위로 묶어서 처리하고 저장할 수 있는 편리한 방법을 제공합니다. 구조체의 정의와 특징은 다음과 같습니다

```
struct Point {
    var x: Double
    var y: Double
}

```
1. **[[Member]] [[Property]]**: 구조체 내에서 데이터를 나타내는 멤버 프로퍼티를 정의할 수 있습니다. 각 프로퍼티는 이름과 데이터 타입을 가집니다. 구조체의 프로퍼티는 일반적으로 값을 변경할 수 있습니다.
    
2. **값 타입([[Value Type]])**: 구조체는 값 타입(value type)입니다. 이것은 구조체 인스턴스가 복사되어 전달되거나 할당될 때 원본 데이터를 복사하여 새로운 인스턴스를 생성한다는 의미입니다. 이로 인해 데이터의 불변성을 보장하며 예기치 않은 부작용을 방지합니다.
    
3. **초기화([[Initializer]])**: 구조체는 초기화 [[Method]]([[Initializer]])를 통해 인스턴스를 생성할 수 있습니다. 기본적으로 멤버 프로퍼티에 값을 할당하면서 초기화할 수 있습니다.
4. **메서드([[Method]])**: 구조체는 메서드를 가질 수 있으며, 이를 사용하여 구조체 내에서 데이터를 조작하거나 특정 동작을 수행할 수 있습니다.
	```
	struct Rectangle {
    var width: Double
    var height: Double
    func area() -> Double {
        return width * height
    }
}

5. **확장([[Extension]])**: 구조체에는 확장(extension)을 통해 새로운 멤버나 기능을 추가할 수 있습니다. 이를 통해 기존 구조체를 확장하고 기능을 확장할 수 있습니다.
```
extension Rectangle {
    func perimeter() -> Double {
        return 2 * (width + height)
    }
}
```


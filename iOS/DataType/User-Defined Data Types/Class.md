클래스(Class)는 객체 지향 프로그래밍(Object-Oriented Programming, OOP)에서 사용되는 중요한 개념 중 하나로, [[Data]] 와 해당 데이터를 다루는 동작을 함께 포함하는 사용자 정의 [[DataType]]입니다.
클래스는 객체(Object)의 템플릿이며, 객체는 클래스로부터 생성됩니다. 

클래스의 정의와 특징은 다음과 같습니다.

**정의**: 클래스는 프로그래밍 언어에서 키워드(예: `class`)를 사용하여 정의됩니다.
클래스는 속성([[Member]] [[Variable]]또는 [[Property]])과 [[Method]]([[Function]])를 포함하며
이러한 속성과 메서드는 클래스 내에서 정의됩니다.


**e.g)**
```
class Person {
    var name: String
    var age: Int
    ### member

    init(name: String, age: Int) {
        self.name = name
        self.age = age
    }
    ### initializer

    func sayHello() {
        print("Hello, my name is \(name) and I am \(age) years old.")
    }
    ### Method
}

```
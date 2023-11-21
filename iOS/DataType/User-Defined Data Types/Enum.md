"Enum(Enumeration)"은 프로그래밍에서 열거형 데이터 타입을 정의하는 데 사용되는 구조체([[struct]])입니다. 열거형은 서로 관련된 값들의 집합을 정의하고 명명한 것으로, 일반적으로 비슷한 종류의 항목을 그룹화하고 식별하는 데 사용됩니다. 열거형의 정의와 특징을 아래에서 설명합니다:

1. **정의**: 열거형은 프로그래밍 언어에서 키워드(예: `enum`)를 사용하여 정의됩니다. 열거형 안에는 여러 개의 "케이스(case)"가 포함되며, 각 케이스는 고유한 값을 나타냅니다 ``

2. **고유한 값**: 열거형의 각 케이스는 해당 케이스의 고유한 값을 가질 수 있습니다. 

열거형은 프로그램에서 가독성을 높이고 코드를 관리하기 쉽게 만드는 데 유용한 도구입니다. 이를 통해 서로 다른 유형의 값을 명확하게 구분하고 관리할 수 있으며, 코드의 오류를 줄이고 유지 보수성을 향상시킬 수 있습니다.


**e.g)**
 ```
 enum Day {
    case sunday
    case monday
    case tuesday
    case wednesday
    case thursday
    case friday
    case saturday
}

```

```
switch today {
    case .saturday, .sunday:
        print("It's the weekend!")
    case .monday... .friday:
        print("It's a weekday.")
}
```
일반적으로 다음과 같이 switch문과 같이 쓰입니다.
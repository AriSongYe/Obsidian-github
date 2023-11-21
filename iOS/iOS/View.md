
```
protocol View
```

### Summary
- 어플리케이션에서 User [[Interface]] 를 통해 제공하는 Design의 일종
- View를 통해 User Interface 그려질 [[drawing]] 을 관리합니다.
- View는 계층적인 구조를 가지고 있으며 User에 의한 [[Event]]가 발생했을 때 일어난 변화를 Update하여 User Interface에 그려주는 것이 View의 역할입니다.
```
public protocol View {
	associatedtype Body : View
	@ViewBuilder @MainActor var body: Self.Body { get }
}

```

- [[@ViewBuilder]] [[property wrapper]]를 통해 Child View들을 콤마없이 나열하여 화면에 구성할 수 있도록 도와줍니다.
- [[@MainActor]]


### Ref
[CustomView](https://developer.apple.com/documentation/swiftui/declaring-a-custom-view)
[View](https://developer.apple.com/documentation/swiftui/view/)

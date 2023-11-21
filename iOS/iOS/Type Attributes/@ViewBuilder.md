@ViewBuilder는 [[View]] [[protocol]] 의 Computed Property인
[[Body]] 에 child View들의 구성을 컴마 없이 나열하여 사용할 수 있도록 도와주고
View들을 화면에 구성합니다.

```
@resultBuilder public struct ViewBuilder {
	public static func buildBlock() -> EmptyView
	public static func buildBlock<Content>(_ content: Content) -> Content where Content : View }
```

이 때 @viewBuilder 안에 [[buildBlock]] 함수가 View들을 [[Generic]]하게 받아 실제 화면에 scene들을 그립니다.

이 때 공식 문서에서 @buildBlock 함수는 인자인 View의 개수에 따라 다양하게 존재하는 것을 확인할 수 있습니다.

[[@resultBuilder]] [[property wrapper]]를 통해 child View들의 구성을 컴마 없이 나열하여 사용할 수 있도록 도와줍니다.


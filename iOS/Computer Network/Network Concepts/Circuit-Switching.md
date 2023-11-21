
앞서 언급한 [[Packet-Switching]]과 다르게 전화처럼 데이터를 주고받는 방식입니다.

[[Data Packet]]은 어떠한 특정 [[Router]]를 정하는 것이 아닌 [[Routing]] 알고리즘에 따라 유연하게 전달되지만

**Circuit Switching은 미리 회선을 정하고** 데이터를 주고 받습니다.

이러한 데이터 송수신은 Data가 **Loss**가 되거나 **Delay**가 되지 않는 **장점**이 있습니다.

**하지만** shared link로 인해 Data를 **주고받는 회선은 다른 사용자가 접근할 수 없는** 치명적인 단점이 있습니다.

-> **Multi Access가 어려운 치명적인 단점**

![](https://blog.kakaocdn.net/dn/dFlyq9/btstX9OMPej/6qMMfyKZtWYQTCXkrQmkOK/img.png)

이러한 단점을 보완하기 위해 두 가지의 방법이 고안되었습니다.

[[Frequency Division Multiplexing(FDM)]] , [[Time Division Multiplexing(TDM)]]

하지만 이 두 가지 방법은 [[Internet]]에 사용되는 물리적인 한계가 명확하기에 사용되지 않았고

[[Packet-Switching]] 방법이 Internetwork에 채택됩니다.
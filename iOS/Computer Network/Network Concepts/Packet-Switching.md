[[store-and-forward]] 방식으로 [[Router]]를 통해 [[Data Packet]]을 전달하는 방법입니다.

Flat하게 연결되어 있는 Routers의 연결을 통해 Packet 단위로 데이터를 송수신하는 것을 Packet-Switching이라 합니다.

Packet은 Packet마다 다른 경로로 전달될 수 있습니다. Network 상황에 따라 **Flexible**한 장점이 있습니다.

Packet은 Router에 저장되고 [[Routing]] 알고리즘에 의해 [[Forwarding]] 됩니다.
하지만 이 속도보다 요청 속도가 빠른 다음 그림과 같은 경우가 생깁니다. 
![](https://blog.kakaocdn.net/dn/FiwH4/btstY7pDfaV/mKhUKaLxajX3g8xbqnObQK/img.png)

이 때 차곡차곡 Router 안에 있는 [[Queue]]에 Data Packet 들이 쌓이게 됩니다 -> Delay 발생.

하지만 Router의 Buffer Size는 물리적 한계가 있기 때문에 정해진 Queue 사이즈보다 더 많이 쌓일 경우에

그 패킷은 Drop되어 Loss 발생합니다.

Packet-Switching은
1. Delay
2. Packet Loss
두 가지 문제가 발생할 수 있습니다.
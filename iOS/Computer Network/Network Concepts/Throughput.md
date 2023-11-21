"Throughput(처리량)"는 시간 단위로 얼마나 많은 [[Data]]가 처리되거나 전송되는지를 나타내는 성능 지표입니다. Throughput은 주로 데이터 통신, [[Network]], [[Computer Systems]] 및 다양한 [[Application]]의 성능을 측정하고 평가하는 데 사용됩니다. Throughput은 데이터 처리량, 대역폭 활용률, 또는 작업률과 유사한 의미로 사용됩니다.

쉽게 말해 sender 와 receiver 간 네트워크의 속도에 대한 **성능 지표**를 Throughput이라 합니다.

![](https://blog.kakaocdn.net/dn/coy0iU/btsvYYJ4kyL/rB4CkpiCIIKDKj24n0EPG0/img.png)

다음과 같은 link들을 가진 네트워크에서 average throughput을 구한다면 어떤값이 더 클까 생각해 봅시다.
정답은 경로에 있는 link중에 가장 느린 link의 속도로 평균을 내면 됩니다.

**bottleneck link**

여러개의 link가 있고 속도가 각양각색이라면
> **end to end 사이에 가장 느린 link의 속도가 average throughput이 됩니다.**

가장 느린 link로 인해 **Congestion이** 발생하기 때문입니다.

호스, 관을 통해 물이 이동하는 것을 생각하면 이해하기 쉽습니다.
처음, 중간, 마지막 어디든 동일한 크기로 물이 통과할 수 있는 입구를 좁히면 동일한 속도로 물이 지나갑니다.
네트워크에서 packet이 전달될 때도 호스와 관을 지나가는 물과 같은 현상이 일어납니다.
![](https://blog.kakaocdn.net/dn/cwfN9B/btsvMJnGIn3/k3mFxyQuMYsk5Hx2SBZ7Z1/img.png)

Packet-Delay&Loss

**[[Packet-Switching]]**에서 **link**를 통해 **전달 속도**보다 **요청 속도**가 빠를 경우

**Queuing Delay**와 **loss**가 생길 수 있음을 알 수 있습니다.

#### **Packet Delay의 4가지 요소**

![](https://blog.kakaocdn.net/dn/CQqKY/btsvWSKBype/TvUMZZ9qh2E1f1dpQorVLK/img.png)

Four sources of packet delay

1. Processing

Routing 알고리즘 처리 및 bit error를 확인하는 과정입니다.

일반적으로 msec 단위의 시간이 소요됩니다.

2. transmission

Link에 의해 결정되는 속도입니다.

Physical 요소로서 선의 종류에 의해 결정되는 요소입니다.

3. propagation

전파 매질과 거리에 의해 결정되는 요소입니다.

**4. queue**

**상대적**으로 다른 delay 요소들에 비해 **queuing delay**가 가장 큽니다.

요청속도가 전송속도보다 높은 경우 발생하는 delaydlau

그 다음으로 큰 delay는 transmission Delay입니다.
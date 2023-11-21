Hash란 [[Data]]를 다루는 기법 중에 하나입니다.

Hash라는 [[Function]] 혹은 [[Encrypntion]]를 통하여 어떠한 Data가 담긴 암호화된 [[Key]] 값에 대응하는 HashTable(배열) 값에 Data를 저장하는 기법입니다.

![[Hash_Image.png]]
다음과 같은 예제가 가장 쉬운 Hash의 예입니다.
1. hashTable을 만듭니다
2. updeateValue 함수를 통해 Key&Value 값을 입력합니다.
3. 입력된 함수가 hash함수를 통해 정해진 새로운 index에 저장이됩니다.
4. hashTable을 열람할때는 getValue라는 함수를 통해 Key 값을 넣어 데이터를 Read 합니다.
5. getValue 함수는 hash함수를 통해 변형된 Key값의 인덱스를 통하여 hashTable에 접근합니다.

**장점**
일반적인 배열에서 특정 Data를 찾는다하면 O(N)의 시간이 걸리지만
hash를 사용한다면 O(1)의 시간이 걸린다.

**단점**
시간복잡도가 빨라지는 대신 공간복잡도 hashTable의 크기가 비효율적이다.
어떠한 hash알고리즘을 사용하는지에 따라 달라지지만 공간을 많이 필요로 한다

**한계점**
hash함수가 단순한 경우에 인덱스가 중복될 수 있다.
이때 해결할 수 있는 방법은
1. Key값을 같이 저장하여 연결리스트의 형태로 저장하는 방법
2. Linear Probing이라 하여 중복된 인덱스 부터 순회하여 빈 공간에 저장하는 방법
이 있다.

이러한 hash의 활용은 대규모 Data를 다루는데 특화되어있다.

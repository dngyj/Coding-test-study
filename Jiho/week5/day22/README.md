## 호텔 방 배정
처음에 머리 쓰기 귀찮아서 냅다 선형탐색 해버렸더니 당연하게도 시간 초과가 났다. 이럴 땐 메모리를 써서 연산 횟수를 줄이는 게 최고의 방법이 아닐까.. 그래서 생각했다. 어떻게 하면 연산 횟수를 줄일 수 있지? **특정 방의 다음 방 번호를 저장해두면 되지 않을까?**. 요 생각으로 풀었다.

- 다음 빈 방 정보 저장해둠
- 연결된 기존 방의 다음 빈 방 정보도 함께 업데이트(재귀)
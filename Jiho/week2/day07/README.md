## 미로만들기
### 문제 풀이
검정 블록은 가중치 1, 흰 블록은 가중치 0이라고 생각하면 된다.

따라서 **0-1 BFS**를 사용해 **가중치가 적은 경로를 우선 탐색**하도록 구현했다.

### 0-1 BFS
가중치 1을 만나면 큐의 뒤쪽에 추가하고 가중치 0을 만나면 앞쪽 큐에 추가함으로써 가중치가 적은 경우를 먼저 탐색할 수 있다.
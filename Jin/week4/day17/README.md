## 가장 큰 정사각형 찾기 문제
  
### 문제 풀이
- 왼쪽, 위쪽, 왼쪽 위 대각선이 모두 1인 경우 -> 2 * 2 정사각형을 만들 수 있음.
  - 2 * 2 정사각형이 되는 경우에 board의 현재 위치를 2로 업데이트
  -> 이 방식으로 board 배열 자체를 메모이제이션처럼 활용하면서 업데이트하기
  -> 왼쪽(left), 위쪽(up), 왼쪽 위 대각선(upLeft) 중 값이 가장 작은 값에 + 1을 하면서 만들 수 있는 정사각형의 한 변 길이를 저장
  - 마지막은 배열 내 최댓값을 제곱해서 넓이로 출력
    - 요새 stream 코드를 써보려고 노력 중입니다. 아직 익숙치 않아서.. 인터넷에 검색하면서 쓰고 있지만 이렇게 익숙해지는 거겠죠 ㅎㅎ

### 여담
- DP도 심각하게 약해서(ㅠㅠ) 책을 보면서 공부를 했는데 **`작은 문제로 크기를 줄여서 접근하라`** 는 말이 참 인상 깊었습니다.
    - 항상 문제를 보면 테스트 케이스만 보고 어떻게 풀어야 할 지 생각한다고 참 막막했는데, 작은 범위부터 차근차근 문제 조건을 생각하면서 풀면 조금 더 쉽게 접근하고 풀이할 수 있겠다는 걸 다시금 상기했네요ㅎㅎ
      다들 항상 고생 많으십니다!!! 화이팅 ㅎㅎㅎ!
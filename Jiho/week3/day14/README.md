## 다단계 칫솔 판매
- 다단계라니.. 너무 신박했음.
- 해시 + 재귀 이용해서 **부모 노드를 추적해가며 전체 벌어들인 금액을 업데이트**해주는 방식으로 구현했다.
### 아쉬운 점
- `amount1`, `amount2`.. 변수명이 이게 최선이었을까
- 그리고 재귀 코드도 뭔가 깔끔하지 못한 느낌
### 채찍피티에게 피드백 맡김
- 트리 초기화 부분 개선 가능: 바로 `referral`을 활용할 수도 있음. 하지만 가독성을 위해 따로 두는 것도 나쁘지 않음. 다만 `tree`를 `Map`을 사용하면 객체보다 조회 속도가 조금 더 최적화 될 수 있음.
- 불필요한 계산 제거 가능: Math.ceil(amount * 0.9)와 Math.floor(amount * 0.1) 대신 amount1 = amount - amount2를 사용하면 연산 횟수를 줄일 수 있음.
- `totalAmount` 초기화 방식 개선: `Object`가 아닌 `Map`을 사용하면 `Object.values(totalAmount)`를 반환할 때 순서를 보장할 수 있음

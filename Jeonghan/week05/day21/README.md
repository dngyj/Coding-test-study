### 문제 분석
부분 배열의 구간합이 특정값인 경우 탐색  
완전 탐색(n^2)은 시간 초과 발생 가능  
한번의 탐색으로 답이 나와야 하기 때문에 투포인터를 이용한 슬라이딩 윈도우 사용  

<br>

### 문제 조건
배열 최대 길이 1,000,000  
원소 최대 크기 1,000  
누적합 최대 크기 1,000,000,000  

<br>

### 문제 풀이
1. 배열 순회
2. 해당 구간의 누적합 계산
3. 누적합의 크기가 특정값보다 큰 경우 구간 축소
4. 누적합의 크기가 특정값인 경우 반환값 갱신

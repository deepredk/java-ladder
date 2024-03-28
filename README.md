# 사다리 게임

## 재구현 요구사항

> In->Out TDD, 책임 주도 설계 고려해서 처음부터 다시

사다리 열
- [X] 몇 번째 열인지 알고 있다
- [X] 어느 방향의 열과 연결되어 있는지 알고 있다
- [X] 연결되어 있는 열로 가는 인덱스를 반환한다

사다리 행
- [X] 여러 사다리 열을 알고있다
- [X] 유효한 행인지 검증한다
  - 열이 1개 이상 있어야 한다
  - 열의 연결이 빈쪽을 연결하고 있지 않아야 한다
  - 열 정합성을 만족해야 한다 (양방향 연결이 제대로 되어 있어야 한다)
- [X] 특정 열에 연결되어 있는 다음 열로 가는 인덱스를 반환한다

랜덤 사다리 행 생성기
- [X] 랜덤한 사다리 열을 N만큼 만든다
    - 단, 연결이 연속되지 않게 한다

사다리
- [X] 여러 사다리 행을 알고있다
- [X] 유효한 사다리인지 검증한다
  - 행이 1개 이상 있어야 한다
  - 모든 행의 열 개수가 같아야 한다
- [X] 사다리 결과(각 시작점에 대한 끝점의 매칭 결과)를 반환한다

랜덤 사다리 생성기
- [X] N개의 열을 가진 랜덤한 사다리 행을 M만큼 만든다

참가자
- [X] 몇번째인지 알고있다
- [X] 이름을 알고 있다
- [X] 통지받은 당첨 결과를 알고 있다
- [X] 당첨 결과를 통지받는다

참가자 일급 컬렉션
- [X] 참가자들을 알고 있다
- [X] i번째 참가자에게 당첨 결과를 통지한다

당첨 상품
- [X] 몇번째인지 알고 있다
- [X] 이름을 알고 있다

당첨 상품 일급 컬렉션
- [X] 당첨 결과들을 알고 있다
- [X] i번째 당첨 결과를 반환한다

사다리 심판
- [ ] 1 사다리 결과 2 참가자 일급 컬렉션 3 당첨 결과 일급 컬렉션을 이용하여 참가자에게 당첨 결과를 통지한다

사다리 콘솔
- [ ] 참여자 이름을 입력받는다
- [ ] 실행 결과를 입력받는다
- [ ] 최대 사다리 높이를 입력받는다
- [ ] 랜덤으로 사다리를 만들고 보여준다
  - 사다리 각 시작점에 참가자의 이름을 보여준다
  - 사다리를 보여준다
  - 사다리 각 끝점에 실행 결과를 보여준다
- [ ] 결과를 보여준다
  - 한 사람의 결과를 보여준다
  - 여러 사람의 결과를 보여준다

## 기능 요구사항

- [X] 사다리 게임에 참여하는 사람의 이름을 최대 5글자까지 부여할 수 있다
- [X] 사다리 1줄은 |-----|-----|과 같이 가로 라인이 겹쳐질 수 없다
- [X] N명의 참가자에 대한 유효한 사다리 1줄을 무작위로 만든다
- [X] N명의 참가자에 대한 유효한 사다리 M줄을 무작위로 만든다
- [X] UI 구현
- [X] 실행 결과(사다리 아럐쪽 부분)를 입력 받는다
- [X] 모든 참가자에 대한 사다리 결과를 알아낸다

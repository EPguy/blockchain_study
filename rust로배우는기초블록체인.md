자료: https://hackernoon.com/rusty-chains-a-basic-blockchain-implementation-written-in-pure-rust-gk2m3uri

1. 블록체인은 분산원장의 개념이 포함되어있다.
2. 블록체인에선 장부를 peer to peer 형태로 저장된다.
3. peer to peer 을 구현하기 위해 복잡한 기능들이 구현되어야 한다.
4. 블록체인에선 모든 트랜잭션의 기록들을 기록한다.
5. 기록된 모든 트랜잭션들을 실행하다 보면 최종상태를 얻을 수가 있는데, 이를 블록체인에선 world state 라고 부른다.
6. world state 는 트랜잭션의 전체 이력을 포함하지 않기에, 일반적으로 실제 블록체인보다 훨씬 작다.
7. 모든 트랜잭션을 재생하여 언제든지 world state 를 검색할 수 있기에, world state 를 반드시 저장할 필요는 없다.
8. 이렇게 정렬된 트랜잭션은 중간 트랜잭션(이전 체인)을 변경할 수 없는 방식으로 보안이 유지된다. 이를 불변상태(immutable state)라고 부른다.
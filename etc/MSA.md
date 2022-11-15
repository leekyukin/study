# 🏛️ MSA (Microservice Architecture)

## 📌 MSA란
    비즈니스 도메인을 중심으로 서비스를 모델링하고 구현하는 아키텍처 스타일

- 🌐 도메인 서비스 간 통신은 네트워크 기반의 HTTP API 또는 비동기 메시징 방식등으로 이뤄짐
- 💿 각 도메인 서비스가 각자 DB를 가짐 

### 반대격으로 불리는 monolithic은?
> 하나의 프로젝트 구조 안에서 모든 도메인을 구현하는 방식

---
<br>

## 📌 MSA 전환을 고려해야 하는 시점
1. 초기 스타트업에서 비즈니스 규모가 어느 정도 궤도에 오르는 시점
2. monolithic 구조의 단점이 부각되는 시점
  - 구현, 테스트, 배포 속도가 점점 느려지고 정기배포라는 절차가 생길 때
  - 한 repository에 코드베이스가 개개인이 감당할 수 없는 수준으로 커졌을 때
  - 이에 따라 코드 파악과 유지보수가 어려워질 때
  - 모든 측면에서 확장성이 떨어지게 될 때

### ⚡️ 그럼에도 불구하고 monolithic을 유지한다면...
> 기업 경쟁력은 점점 약해지고 나아가 생존하지 못할 수도 있다.

---
<br>

## 📌 장단점

|장점|단점|
|---|---|
|각각의 비즈니스를 도메인별로 독립적인 서비스로 운영 가능|네트워크 기반의 API 호출로 서비스가 구성되어 프로세스간 통신에 비해 느리고 복잡함 |
|빠른 구현과 배포 가능 | 일관된 트랜잭션과 데이터 정합성 유지가 힘듬|
|팀의 책임과 자율성이 극대화| 테스트와 장애추적, 모니터링이 힘듬|


### ⚡️ 우버가 MSA를 도입한 이유

1. 증가하는 트래픽 처리
2. 새로운 기능을 쉽게 추가
3. 조직의 성장에 쉽게 적응할 수 있는 아키텍처 적용
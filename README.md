# Querydsl 학습 프로젝트

## 프로젝트 소개
이 프로젝트는 Querydsl을 활용한 데이터 조회 최적화 및 복잡한 쿼리를 자바 코드로 표현하는 방법을 학습하고 구현한 프로젝트입니다. 스프링 데이터 JPA와 함께 Querydsl을 사용하여 타입 안전한 쿼리 작성과 동적 쿼리 처리 방법을 다룹니다.

## 기술 스택
- **Language**: Java 17
- **Framework**: Spring Boot 3.4
- **ORM**: JPA (Hibernate)
- **Query DSL**: Querydsl 5.0.0
- **Database**: H2 Database
- **Build Tool**: Gradle
- **Lombok**: 코드 간소화를 위한 어노테이션 기반 라이브러리

## 주요 기능
- **기본 문법**: Querydsl의 기본적인 쿼리 작성 방법 구현
- **중급 문법**: 동적 쿼리, 성능 최적화를 위한 벌크 연산 등 고급 기능 구현
- **순수 JPA와 Querydsl 연동**: JPA Repository와 Querydsl 결합 예제
- **스프링 데이터 JPA와 Querydsl 통합**: 스프링 데이터 JPA와 Querydsl 조합으로 강력한 쿼리 기능 구현
- **실무 활용 사례**: 페이징, 정렬, 검색 조건 처리 등 실무에서 자주 사용되는 기능 구현

## 프로젝트 구조
```
src
├── main
│   ├── java
│   │   └── study
│   │       └── querydsl
│   │           ├── controller
│   │           ├── dto
│   │           ├── entity
│   │           │   ├── Member.java
│   │           │   ├── Team.java
│   │           │   └── Hello.java
│   │           ├── repository
│   │           └── QuerydslApplication.java
│   └── resources
└── test
    └── java
        └── study
            └── querydsl
```

## 엔티티 모델
- **Member**: 회원 정보를 담당하는 엔티티 (이름, 나이, 소속 팀)
- **Team**: 팀 정보를 담당하는 엔티티 (팀명, 소속 회원 목록)

## 학습 내용
1. **Querydsl 설정 방법**
   - Gradle 설정
   - Q타입 생성 및 활용

2. **기본 문법**
   - JPQL vs Querydsl 비교
   - 검색조건 설정
   - 결과 조회 방법
   - 정렬과 페이징

3. **중급 문법**
   - 조인 (innerJoin, leftJoin, fetchJoin)
   - 서브쿼리 처리
   - Case 문과 상수/문자 처리
   - 동적 쿼리 구현

4. **실무 활용**
   - 순수 JPA Repository와 Querydsl 통합
   - 스프링 데이터 JPA와 Querydsl 통합
   - QuerydslRepositorySupport 활용
   - 페이징, 정렬, 검색 필터링 구현

## 기대 효과
- 타입 안전한 쿼리 작성으로 컴파일 시점에 오류 감지
- 동적 쿼리 처리의 용이성 향상
- 직관적인 자바 코드 기반 복잡한 쿼리 작성 능력 습득
- 스프링 데이터 JPA와 Querydsl 조합으로 생산성 향상

## 향후 계획
- 실무 프로젝트에 적용할 수 있는 보일러플레이트 코드 개발
- 복잡한 동적 쿼리 최적화 방안 연구
- 대용량 데이터 처리를 위한 성능 최적화 기법 연구

## 참고 자료
- [Querydsl 공식 문서](http://querydsl.com/static/querydsl/latest/reference/html/)
- [스프링 데이터 JPA 공식 문서](https://docs.spring.io/spring-data/jpa/docs/current/reference/html/)

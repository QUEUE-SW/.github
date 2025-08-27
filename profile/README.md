# 🎓 QUEUE-SW: 수강신청 대기열 시스템

> 대학교 수강신청은 수천 명이 동시에 접속해 서버가 과부하되는 경우가 많습니다. **QUEUE-SW**는 이를 해결하고, 대규모 트래픽 환경에서의 안정적인 수강신청 처리를 위해 설계된 **대기열 기반 수강신청 시스템**입니다.
> 스프링 기반 서버 구조와 병렬 분산 처리 기술을 활용하여 높은 동시성을 지원합니다.

---

## 🧭 프로젝트 개요

- **목표**: 대학교 수강신청 시 과부하를 방지하고, **안정적이고 사용하기 편한 대기열 기반 수강 시스템** 제공
- **특징**
  - 대기열 기반 사용자 처리
  - 고가용성 / 확장성 고려 설계
  - Redis, Spring Boot 등 최신 스택 사용
  - SSE 기반 실시간 피드백 제공
  - 사용자가 사용하긴 편한 UI/UX 제공

---

## 🛠️ 기술 스택

| 구성 요소        | 기술 명세                          |
|------------------|-----------------------------------|
| **Backend**      | Java 17, Spring Boot, Spring Web |
| **Queue 시스템** | Redis                      |
| **DB/Cache**     | Redis, MySQL                      |
| **API 통신**     | REST API, SSE                    |
| **배포환경**     | Docker, AWS EC2                   |

---

## 📌 레포지토리 구조
- `AllClear-web` : React+Vite 기반 프론트엔드
- `AllClear-was` : Spring Boot 기반 백엔드
- `QUEUE-was` : Redis 기반 대기열 처리 전용

---

## 💡 주요 기능
- 대기열 기반 수강신청
  - 유저가 로그인 시 대기열 등록
  - 순번에 따라 순차적으로 수강신청 페이지 입장하여 신청 가능
- 실시간 피드백
  - Polling 기반 대기열 순번 정보 제공
  - Polling 기반 과목 여석 정보 제공
- 안정성 및 확장성 고려
  - Redis 기반 분산 처리
  - 과부하 시에도 서비스 유지 가능

---

## 👽 팀원 소개 및 역할 분담
|👑 BE 👑|BE|FE|FE|
|:-:|:-:|:-:|:-:|
|<img height="150" src="https://avatars.githubusercontent.com/mingking2"/>|<img height="150" src="https://avatars.githubusercontent.com/MinjiSeo16"/>|<img height="150" src="https://avatars.githubusercontent.com/cryingdryice"/>|<img height="150" src="https://avatars.githubusercontent.com/jihyun132"/>|
|[주민기](https://github.com/mingking2)|[서민지](https://github.com/MinjiSeo16)|[박지원](https://github.com/cryingdryice)|[김지현](https://github.com/jihyun132)|

---

## 🎞 시연 영상

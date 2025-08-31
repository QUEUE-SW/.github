# 🎓 QUEUE-SW: 수강신청 대기열 시스템

대학교 수강신청은 수천 명이 동시에 접속해 서버가 과부하되는 경우가 많습니다. **QUEUE-SW**는 이를 해결하고, 대규모 트래픽 환경에서의 안정적인 수강신청 처리를 위해 설계된 **대기열 기반 수강신청 시스템**입니다.

> 본 프로젝트는 **과학기술정보통신부 주최 한이음 드림업 공모전**에 출품된 작품으로, **기업 전문가 멘토와 협업하여 기획·개발**하였습니다.

<br>

## 🧭 프로젝트 개요

- **목표**: 대학교 수강신청 시 과부하를 방지하고, **안정적이고 사용하기 편리한 대기열 기반 수강 시스템** 제공
- **특징**
  - 대기열 기반 사용자 분산 처리
  - JMeter 기반 성능 검증을 통한 단계별 아키텍처 고도화
  - Redis·SSE 기반 실시간 피드백 제공
  - 직관적이고 사용자 친화적인 UI/UX 제공
 
<br>

## 🛠️ 기술 스택

| 구성 요소        | 기술 명세                                    |
|------------------|----------------------------------------------|
| **Frontend**     | JavaScript, React + VITE, Zustand            |
| **Backend**      | Java 17, Spring Boot 3.2.3                   |
| **DB/Cache**     | Redis 7.1, MySQL 8.0.41                      |
| **API 통신**     | REST API, SSE, Polling                       |
| **배포환경**     | AWS EC2, Docker, RDS, ElastiCache, Nginx, AWS S3, CloudFront, Route53 |
|**협업 도구**   |Jira, Confluence, Slack|

<br> 

## 📐 아키텍처
<img width="500" height="800" alt="image (2)" src="https://github.com/user-attachments/assets/1fab7959-5950-480e-a270-3e92c6178ca3" />

<br>
<br>

## 📌 레포지토리 구조
- [AllClear-web](https://github.com/QUEUE-SW/AllClear-web) : 사용자 화면 및 인터페이스
- [AllClear-was](https://github.com/QUEUE-SW/AllClear-was) : 핵심 비즈니스 로직
- [QUEUE-was](https://github.com/QUEUE-SW/QUEUE-was) : 대기열 관리

<br>

## 💡 주요 기능
- 대기열 기반 수강신청
  - 유저가 로그인 시 대기열 등록
  - 순번에 따라 순차적으로 수강신청 페이지 입장하여 신청 가능
- 실시간 피드백
  - Polling 기반 대기열 순번 정보 제공
  - SSE 기반 과목 여석 정보 제공
 
<br>

## 👽 팀원 소개 및 역할 분담
|👑 BE 👑|BE|FE|FE|
|:-:|:-:|:-:|:-:|
|<img height="150" src="https://avatars.githubusercontent.com/mingking2"/>|<img height="150" src="https://avatars.githubusercontent.com/MinjiSeo16"/>|<img height="150" src="https://avatars.githubusercontent.com/cryingdryice"/>|<img height="150" src="https://avatars.githubusercontent.com/jihyun132"/>|
|[주민기](https://github.com/mingking2)|[서민지](https://github.com/MinjiSeo16)|[박지원](https://github.com/cryingdryice)|[김지현](https://github.com/jihyun132)|

<br>

## 🎞 시연 영상
[오픈소스 기반 수강신청 대기열 시스템 개발](https://www.youtube.com/watch?v=T_8bqxawZQY)

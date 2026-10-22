# findex
금융위원회 OpenAPI 기반 금융 지수 분석 서비스

## 프로젝트 구성

- **프로젝트명:** Findex
- **진행 방식:** 개인 프로젝트
- **개발자:** 진하윤

---

## 프로젝트 소개

Findex는 금융위원회에서 제공하는 주가지수 OpenAPI를 활용하여 금융 지수 정보를 관리하고, 시계열 차트 및 성과 분석 정보를 제공하는 금융 분석 서비스입니다.

Spring Boot를 기반으로 외부 API 연동, 금융 데이터 관리, 자동 동기화 기능을 구현하는 것을 목표로 합니다.

- **프로젝트 유형:** 금융 데이터 관리 및 분석 서비스
- **프로젝트 진행 상태:** 기획 및 준비 단계

---

## 기술 스택

- **Backend:** Java, Spring Boot, Spring Data JPA
- **Database:** PostgreSQL
- **API Documentation:** springdoc-openapi (Swagger)
- **Scheduling:** Spring Scheduler
- **Utility:** MapStruct
- **Deployment:** Railway
- **Version Control:** Git & GitHub

---

## 개인 프로젝트 기능 계획

### 1. OpenAPI 연동 준비
- 금융위원회 주가지수 OpenAPI 활용 신청
- API 인증키 발급 및 데이터 조회 테스트
- JSON 형식의 응답 데이터 확인

### 2. 지수 정보 관리
- 지수 정보 등록, 조회, 수정, 삭제(CRUD)
- 지수 분류 및 기본 정보 관리

### 3. 지수 데이터 관리
- 날짜별 지수 시세 데이터 관리
- 시가, 종가, 고가, 저가 및 거래량 조회
- CSV 파일 내보내기

### 4. 연동 작업 관리
- 외부 API 데이터 동기화
- 동기화 작업 이력 및 성공·실패 상태 관리

### 5. 자동 연동 설정 관리
- Spring Scheduler를 활용한 자동 데이터 수집
- 자동 동기화 설정 및 실행 이력 관리

### 6. 대시보드 관리
- 금융 지수 시계열 차트
- 이동평균선 및 등락률 등 금융 지표 분석

※ 위 기능은 프로젝트 요구사항을 바탕으로 정리한 구현 계획입니다.

---

## 프로젝트 파일 구조

향후 Spring Boot 프로젝트 구성 시 다음과 같은 구조를 사용할 계획입니다.

```plaintext
findex/
 ┣ src/
 ┃ ┣ main/
 ┃ ┃ ┣ java/
 ┃ ┃ ┃ ┗ com/findex/
 ┃ ┃ ┃   ┣ controller/
 ┃ ┃ ┃   ┣ service/
 ┃ ┃ ┃   ┣ repository/
 ┃ ┃ ┃   ┣ entity/
 ┃ ┃ ┃   ┣ dto/
 ┃ ┃ ┃   ┣ config/
 ┃ ┃ ┃   ┗ scheduler/
 ┃ ┃ ┗ resources/
 ┃ ┃   ┗ application.yml
 ┃ ┗ test/
 ┣ build.gradle
 ┣ settings.gradle
 ┣ .gitignore
 ┗ README.md
```

※ 실제 구현된 파일 구조가 아닌 예정 구조입니다.

---

## 구현 홈페이지

현재 서비스 구현 전 단계로, 배포된 홈페이지는 없습니다.

---

## 프로젝트 회고록

Findex 프로젝트를 준비하면서 금융위원회 OpenAPI 활용 신청과 인증키 발급을 진행하였습니다.

직접 API를 호출하여 JSON 형식의 주가지수 데이터를 확인하면서 외부 데이터를 가져오는 과정을 경험할 수 있었습니다.

이번 준비 과정을 통해 외부 API 연동의 기본적인 흐름을 이해할 수 있었고, 향후 Spring Boot와 데이터베이스를 활용하여 금융 데이터를 관리하는 방법을 학습하고자 합니다.

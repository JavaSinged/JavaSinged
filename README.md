# 신지웅 — Full-Stack Developer

React 화면에서 시작된 사용자의 요청이 Spring Boot API를 거쳐 DB에 저장되고, 다시 화면에 반영되는 흐름을 중요하게 생각합니다.

정상 흐름뿐 아니라 실패 흐름을 먼저 생각하며, 데이터가 어긋날 수 있는 지점을 찾고 이를 막는 구조를 설계하려고 합니다.

<br/>

## Tech Stack

**Frontend**
React · Vite · JavaScript · Zustand · React Query · Axios · CSS Modules · MUI

**Backend**
Java · Spring Boot · Spring MVC · Spring Security · MyBatis · JWT

**Database**
MySQL · Oracle DB

**Infra / DevOps**
AWS S3 · CloudFront · Docker · GitHub Actions · Vercel · Render

**External / Integration**
Toss Payments · Cloudinary · OneSignal · Naver Maps · Daum Postcode

<br/>

## Projects

### 🌱 GreenCarry

> 다회용기 사용과 친환경 배달 방식을 중심으로 설계한 음식 주문 플랫폼

**GitHub** | https://github.com/JavaSinged/green_carry

**Live Demo** | https://greencarry.vercel.app

**Stack**

**Frontend**
React · Vite · Zustand · Axios · CSS Modules · MUI

**Backend**
Java · Spring Boot · Spring Security · JWT · MyBatis

**Database**
Oracle DB

**External / Integration**
Toss Payments · Cloudinary · Naver Maps · Daum Postcode · JavaMailSender

**Deploy**
Vercel · Render

**내가 한 것**

* 팀장으로 기획, DB 설계, 역할 분배, 발표 및 배포 과정 참여
* 주문 생성 시 포인트 차감, 주문 기본 정보 저장, 주문 상세 저장, 주문 이력 저장 흐름 구현
* 주문 생성 로직에 `@Transactional` 적용 — 일부 작업만 성공하는 상황을 방지하고 전체 롤백 구조 구성
* 포인트 차감 쿼리에 DB 단계 조건 추가 — 보유 포인트 초과 사용 요청을 서버에서도 차단
* 주문 완료 시 포인트 적립과 탄소 절감량 누적이 함께 처리되도록 서비스 흐름 구성
* 매장 영업시간·휴무일 데이터 생성, 수정, 삭제 흐름 정리 및 저장 로직 개선
* 회원·점주·관리자 역할별 기능 흐름 이해 및 구현 참여

<br/>

### 📅 WithDay

> 여행, 식사, 문화생활 등 다양한 일정을 만들고 함께할 사람을 모집하는 일정 동행 플랫폼

**GitHub** | https://github.com/JavaSinged/WithDay

**Live Demo** | https://withday-mib.vercel.app

**Notion** | https://app.notion.com/p/0a2c51dc8c4683e8bb5b8170c24be3cc

**Stack**

**Frontend**
React · Vite · TanStack Query · Zustand · Axios · CSS Modules · MUI

**Backend**
Java · Spring Boot · Spring Security · JWT · MyBatis

**Database**
MySQL

**Notification / External**
OneSignal · Cloudinary

**Deploy / CI/CD**
AWS S3 · CloudFront · Docker · Kubernetes · GitHub Actions

**내가 한 것**

* 팀장으로 API 명세서를 선행 작성해 프론트엔드와 백엔드의 요청·응답 기준 정리
* 참여 신청 흐름 설계 — 모집 마감, 정원 초과, 중복 신청, 호스트 본인 신청 등 실패 케이스를 서버에서 검증
* `ParticipationController`는 요청 수신과 DTO 전달에 집중하고, 검증과 상태 저장은 `ParticipationService`로 분리
* `ParticipationService`에서 신청 완료 후 `NotificationService`를 호출하도록 구성해 도메인 책임 분리
* 참여중 / 신청중 / 호스팅 탭별 일정 데이터를 TanStack Query로 조회하고 캐시 키를 분리해 데이터 혼입 문제 개선
* 홈 화면 UI, 일정 탐색, 참여 신청·취소, 내 일정 탭 구조 구현
* GitHub Actions 기반 프론트엔드 배포 흐름 구성 및 모바일 반응형 개선

<br/>

## Portfolio

📝 **Notion Portfolio**
https://jiwoong-shin.notion.site/Backend-Developer-e2751061ca3a8348a44a01912c8a8c45?pvs=143

<br/>

## Contact

📧 **Email**
[shinjiwoong1656@gmail.com](mailto:shinjiwoong1656@gmail.com)

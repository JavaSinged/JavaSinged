# 신지웅 — Backend Developer

정상 흐름보다 실패 흐름을 먼저 그립니다.  
데이터가 어긋날 수 있는 지점을 찾고, 그걸 막는 구조를 먼저 잡습니다.

<br/>

## Tech Stack

**Backend**  
Java · Spring Boot · Spring Security · Spring MVC · MyBatis · JWT

**Frontend**  
React · Vite · Zustand · React Query · Axios · CSS Modules

**Database**  
MySQL · Oracle DB

**Infra / DevOps**  
AWS EC2 · AWS S3 · CloudFront · AWS RDS · Docker · GitHub Actions · Kubernetes / k3s

**External**  
Toss Payments · Cloudinary · OneSignal

<br/>

## Projects

### 🌱 GreenCarry
> 다회용기 사용과 친환경 배달 방식을 중심으로 설계한 음식 주문 플랫폼

**GitHub** | https://github.com/JavaSinged/green_carry  
**Live Demo** | https://greencarry.vercel.app

**Stack**  
Java · Spring Boot · Spring Security · MyBatis · Oracle DB · React · Vite · Zustand · Toss Payments · SSE · Vercel · Render

**내가 한 것**
- 팀장 | 기획, DB 설계, 역할 분배, 배포까지 전 과정 주도
- 주문 생성 로직에 `@Transactional` 적용 — 포인트 차감, 주문 저장, 이력 저장 중 하나라도 실패하면 전체 롤백되도록 구성
- 포인트 차감 쿼리에 DB 단계 조건 추가 — 프론트 검증만으론 부족하다고 판단, 보유 포인트 초과 요청을 서버에서도 차단
- 주문 취소 시 포인트 복구, 완료 시 포인트 적립·탄소 절감량 누적을 하나의 서비스 흐름으로 묶어 데이터 정합성 확보
- 매장 영업시간·휴무일 데이터 처리 로직 구현
- 회원·점주·관리자 역할 기반 권한 구조 설계

<br/>

### 📅 WithDay
> 여행, 식사, 문화생활 등 다양한 일정을 만들고 함께할 사람을 모집하는 일정 동행 플랫폼

**GitHub** | https://github.com/JavaSinged/WithDay  
**Live Demo** | https://withday-mib.vercel.app  
**Notion** | https://app.notion.com/p/0a2c51dc8c4683e8bb5b8170c24be3cc

**Stack**  
Java · Spring Boot · Spring Security · MyBatis · MySQL · React · Vite · TanStack Query · Zustand · CSS Modules · AWS S3 · CloudFront · Docker · Kubernetes · GitHub Actions

**내가 한 것**
- 팀장 | API 명세서 선행 작성으로 프론트·백엔드 요청·응답 기준 통일
- 참여 신청 흐름 설계 — 모집 마감·정원 초과·중복 신청·호스트 본인 신청 등 실패 케이스를 먼저 정의하고 서버에서 검증
- `ParticipationController`는 요청 수신·DTO 전달에 집중, 검증·상태 저장은 `ParticipationService`로 분리
- `ParticipationService`에서 신청 완료 후 `NotificationService` 호출 — 컨트롤러 간 직접 호출 없이 도메인 책임 분리
- 홈 화면 UI, 일정 탐색, 참여 신청·취소, 내 일정 탭 구조 구현
- GitHub Actions 기반 프론트엔드 CI/CD 구성 · 모바일 반응형 개선

<br/>

## Contact

📧 shinjiwoong1656@gmail.com  
💻 https://github.com/JavaSinged

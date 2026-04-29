<p align="center">
  <img src="images/miruni_word_ic.png" alt="Miruni" width="360">
</p>

<p align="center">
  <strong>미루는 습관을 추적하고, 친구와 함께 관리하는 소셜 리마인더</strong>
</p>

<p align="center">
  <a href="https://miruni.net">홈페이지</a> &nbsp;·&nbsp;
  <a href="https://app.miruni.net">웹 앱</a> &nbsp;·&nbsp;
  <a href="https://github.com/MiruniApp/miruni-app/issues">이슈</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Flutter-02569B?style=flat&logo=flutter&logoColor=white" alt="Flutter">
  <img src="https://img.shields.io/badge/Riverpod-2C5BB4?style=flat" alt="Riverpod">
  <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat&logo=springboot&logoColor=white" alt="Spring Boot">
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white" alt="PostgreSQL">
</p>

---

## 미루니가 다른 점

대부분의 할 일 앱은 “완료” 만 추적합니다. 미루니는 **미루는 행위 자체** 를 데이터로 봅니다.
횟수를 기록하고, 색으로 단계를 구분하고, 친구와 패턴을 비교합니다. 부끄럽지 않은 정도의
사회적 압박 — 그게 작은 행동을 바꾸는 가장 빠른 방식이라고 믿어요.

## 주요 기능

- 🐢 **미루기 카운트** — 할 일을 미룰 때마다 횟수 + 단계별 경고 색상
- 📅 **캘린더 + 일정 / 할일 통합** — 마감일 기준 grid 뷰, 일정 색 ribbon
- 👥 **친구 함께 관리** — 친구 일정 엿보기, 주간 통계 비교, 그룹 단위 한 눈에 보기
- 🔁 **반복 할일** — 일/주/월 단위 반복 + 시리즈 일괄 관리
- 📊 **주간 보고서 / 스트릭** — 매주 자동 정리 + 잔디 그래프
- 🔓 **잠금 화면 미루기 알림 (Android)** — 잠금화면에서 바로 task 확인

## 설계 원칙

- **Stale-While-Revalidate** — 캐시 즉시 표시 + 백그라운드 갱신, 깜박임 없음
- **단방향 인증** — Auth → 그 외, 역참조 금지로 circular dependency 차단
- **Optimistic Update + Rollback** — 모든 mutation 즉시 반영, 실패 시 자동 롤백
- **3단계 반응형** — 모바일 / 데스크톱 / 와이드 (폴더블 / 태블릿 대응)

## 저장소

| 저장소 | 설명 |
|---|---|
| [miruni-app](https://github.com/MiruniApp/miruni-app) | Flutter 클라이언트 (Android / iOS / Web / Desktop) |
| [miruni-backend](https://github.com/MiruniApp/miruni-backend) | Spring Boot 서버 (Kotlin / PostgreSQL) |
| [miruni-landing](https://github.com/MiruniApp/miruni-landing) | 공식 홈페이지 |

## 기술 스택

**프론트엔드** Flutter · Riverpod · GoRouter · Drift (SQLite) · Dio · Freezed
**백엔드** Spring Boot · Kotlin · PostgreSQL · Flyway · JWT
**인프라** Docker · Cloudflare · Firebase Cloud Messaging

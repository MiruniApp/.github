<p align="center">
  <img src="images/miruni_word_ic.png" alt="Miruni" width="360">
</p>

<p align="center">
  <strong>미루는 습관을 추적하고, 친구와 함께 관리하는 소셜 리마인더</strong>
</p>

<p align="center">
  <a href="https://miruni.net">miruni.net</a> &nbsp;|&nbsp;
  <a href="https://app.miruni.net">app.miruni.net</a> &nbsp;|&nbsp;
  <a href="https://miruni.net/status">API Status</a>
</p>

---

## About

미루니는 할 일과 일정을 관리하면서, 미루는 습관을 시각화하고 친구와 함께 관리하는 소셜 리마인더 앱입니다.

- 할 일을 미룰 때마다 횟수가 기록되고, 단계별 경고 색상으로 시각화
- 친구의 일정/할일을 엿보고, 주간 통계를 비교
- 반복 할일, 주간 보고서, 스트릭 시스템

## Repositories

| Repository | Description |
|------------|-------------|
| [miruni-app](https://github.com/MiruniApp/miruni-app) | Flutter 클라이언트 (Web + Mobile + Desktop) |
| [miruni-backend](https://github.com/MiruniApp/miruni-backend) | Spring Boot 백엔드 (Kotlin, PostgreSQL, Redis) |
| [miruni-admin-page](https://github.com/MiruniApp/miruni-admin-page) | React 관리자 대시보드 |
| [miruni-landing](https://github.com/MiruniApp/miruni-landing) | 랜딩 페이지 (miruni.net) |

## Tech Stack

<table>
  <tr>
    <td><b>Frontend</b></td>
    <td>Flutter (Dart), Riverpod, GoRouter, Drift (SQLite), Freezed, Sentry</td>
  </tr>
  <tr>
    <td><b>Backend</b></td>
    <td>Spring Boot (Kotlin), Spring Security, JPA, PostgreSQL, Redis, Flyway, Sentry</td>
  </tr>
  <tr>
    <td><b>Admin</b></td>
    <td>React, Vite</td>
  </tr>
  <tr>
    <td><b>Auth</b></td>
    <td>Google / Kakao / Naver OAuth (Web redirect + Mobile SDK), JWT</td>
  </tr>
  <tr>
    <td><b>Infra</b></td>
    <td>Mac Mini + Docker Compose, Cloudflare (Tunnel, Pages, DNS), UptimeRobot</td>
  </tr>
  <tr>
    <td><b>CI/CD</b></td>
    <td>GitHub Actions → Cloudflare Pages (프론트), Docker 빌드 (백엔드)</td>
  </tr>
</table>

## Features

- 할 일 / 일정 관리 (추가, 수정, 삭제, 완료, 미루기)
- 미룬 횟수 시각화 (단계별 색상 경고)
- 반복 할일 (매일/매주/매월)
- 월간 캘린더 뷰 (일정 바 + 할일 점)
- 친구 시스템 (친구 코드, 그룹, 일정 모아보기)
- 동향 잔디 (GitHub 스타일 완료 히트맵)
- 주간 통계 + 친구 비교 차트 + 주간 보고서
- 오프라인 지원 (Drift 로컬 DB + 동기화)
- 소셜 로그인 (Google, Kakao, Naver)
- 공지사항 시스템 + 관리자 대시보드
- 에러/서버 모니터링 (Sentry + UptimeRobot)
- 회원탈퇴 (soft delete + 재가입 복원)
- 반응형 UI (Mobile / Desktop / Web)

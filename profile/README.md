# MiruniApp

**미루니 (Miruni)** — 잠금 해제 시 할 일을 알려주는 나만의 비서

## About

미루니는 스마트폰 잠금 해제 시 오늘의 할 일과 일정을 바로 보여주는 개인 일정 관리 서비스입니다.
미루는 습관을 줄이고, 해야 할 일에 자연스럽게 집중할 수 있도록 도와줍니다.

## Repositories

| Repository | Description |
|------------|-------------|
| [miruni-app](https://github.com/MiruniApp/miruni-app) | Flutter 클라이언트 (Web + Mobile) |
| [miruni-backend](https://github.com/MiruniApp/miruni-backend) | Spring Boot 백엔드 서버 (Kotlin, PostgreSQL) |

## Tech Stack

- **Frontend**: Flutter (Dart), Riverpod, GoRouter, Material 3
- **Backend**: Spring Boot (Kotlin), PostgreSQL
- **Infra**: Mac Mini 자체 서버

## Features

- 할 일 / 일정 관리 (추가, 수정, 삭제, 완료, 미루기)
- 미룬 횟수 시각화 (단계별 색상 경고)
- 월간 캘린더 뷰
- 친구 일정 모아보기
- 잠금 해제 시 할 일 표시 (Android)
- 반응형 UI (Mobile / Desktop)

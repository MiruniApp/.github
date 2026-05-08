<p align="center">
  <img src="images/miruni_word_ic.png" alt="Miruni" width="360">
</p>

<p align="center">
  <strong>미루는 행동을 기록하고 관리하는 소셜 리마인더</strong>
</p>

<p align="center">
  <a href="https://miruni.net">홈페이지</a> ·
  <a href="https://app.miruni.net">웹 앱</a> ·
  <a href="https://github.com/MiruniApp/miruni-app/issues">이슈</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Flutter-02569B?style=flat&logo=flutter&logoColor=white" alt="Flutter">
  <img src="https://img.shields.io/badge/Riverpod-2C5BB4?style=flat" alt="Riverpod">
  <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat&logo=springboot&logoColor=white" alt="Spring Boot">
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white" alt="PostgreSQL">
</p>

---

## Overview

대부분의 할 일 앱은 완료 여부를 중심으로 관리합니다.  
미루니는 완료 이전의 행동, 즉 **‘미루는 과정’ 자체를 데이터로 기록**합니다.

사용자는 미루기 횟수와 패턴을 확인할 수 있고,
친구와 일정 및 통계를 공유하며 지속적인 행동 변화를 유도할 수 있습니다.

## Features

- **미루기 카운트**
  - 할 일을 미룰 때마다 횟수 기록
  - 단계별 경고 색상 표시

- **캘린더 통합**
  - 일정 / 할 일을 하나의 캘린더에서 관리
  - 마감일 기반 grid view 및 일정 ribbon 제공

- **소셜 기능**
  - 친구 일정 및 진행 상태 확인
  - 주간 통계 비교 및 그룹 단위 관리

- **반복 할 일**
  - 일 / 주 / 월 단위 반복 지원
  - 시리즈 전체 수정 및 관리

- **주간 리포트**
  - 스트릭 및 활동 통계 자동 집계
  - 잔디 그래프 기반 활동 시각화

- **잠금 화면 리마인더 (Android)**
  - 잠금 화면에서 바로 task 확인 가능

## Architecture Principles

- **Stale-While-Revalidate**
  - 캐시 데이터를 즉시 표시하고 백그라운드에서 동기화
  - UI 깜빡임 최소화 및 체감 속도 개선

- **Optimistic Update + Rollback**
  - 모든 mutation 결과를 즉시 반영
  - 실패 시 자동 rollback 처리

- **Unidirectional Auth Flow**
  - Auth 상태를 루트로 관리
  - feature 간 circular dependency 방지

- **Responsive Layout System**
  - Mobile / Desktop / Wide 3단계 반응형 대응
  - 태블릿 및 폴더블 환경 지원

## Repositories

| Repository | Description |
|---|---|
| [miruni-app](https://github.com/MiruniApp/miruni-app) | Flutter client (Android / iOS / Web / Desktop) |
| [miruni-backend](https://github.com/MiruniApp/miruni-backend) | Spring Boot backend (Kotlin / PostgreSQL) |
| [miruni-landing](https://github.com/MiruniApp/miruni-landing) | Official landing page |

## Tech Stack

### Frontend
- Flutter
- Riverpod
- GoRouter
- Drift (SQLite)
- Dio
- Freezed

### Backend
- Spring Boot
- Kotlin
- PostgreSQL
- Flyway
- JWT

### Infrastructure
- Docker
- Cloudflare
- Firebase Cloud Messaging

## Platform Support

| Platform | Supported |
|---|---|
| Android | ✅ |
| iOS | ✅ |
| Web | ✅ |
| Windows | ✅ |

## Philosophy

미루니는 단순한 task manager 가 아니라,
사용자의 행동 패턴을 관찰하고 지속적으로 관리할 수 있는 시스템을 목표로 합니다.

작은 사회적 상호작용과 반복적인 피드백이
지속적인 행동 변화에 영향을 준다고 믿습니다.

# 🛡️ SafePic: AI 기반 안심 중고거래 솔루션

> **"AI 기술로 이미지의 진위 여부를 판별하여 사기 없는 투명한 중고 거래 생태계를 구축합니다."**

SafePic은 중고 거래 시장의 고질적인 문제인 **이미지 도용** 및 **AI 생성 이미지 사기**를 해결하기 위해 탄생한 차세대 안심 거래 플랫폼입니다. 판매자의 실물 인증 사진을 AI가 실시간으로 분석하여 구매자에게 신뢰할 수 있는 거래 환경을 제공합니다.

---

## 🚀 프로젝트 비전 (Project Vision)

* **Trust First:** 고가의 전자기기, 명품 등 사진 조작 사기가 빈번한 품목의 거래 안정성 확보.
* **AI Integration:** 단순한 커머스 기능을 넘어, AI 판별 기술을 실제 비즈니스 로직(채팅/검증)에 성공적으로 통합.
* **Scalability:** 대규모 트래픽을 고려한 컨테이너 기반 인프라(AWS ECS)와 효율적인 데이터 설계.

---

## 🏗️ 시스템 아키텍처 (System Architecture)

SafePic은 유연한 확장성과 유지보수성을 위해 **Front-Back 분리 구조** 및 **컨테이너 오케스트레이션**을 채택했습니다.

- **Frontend:** React Native를 이용한 크로스 플랫폼(iOS/Android) 대응 및 React 관리자 웹.
- **Backend:** Java Spring Boot 기반의 고성능 RESTful API 및 WebSocket 채팅 서버.
- **Infrastructure:** AWS ECS, ECR, S3를 활용한 클라우드 네이티브 환경 및 GitHub Actions를 통한 CI/CD 구현.
- **AI Engine:** 외부 AI Detection API 연동을 통한 이미지 메타데이터 및 픽셀 정밀 분석.

---

## 📦 레포지토리 구성 (Repositories)

| Repository | Description | Tech Stack |
| :--- | :--- | :--- |
| **[📂 SafePic-Backend](https://github.com/safe-pic/safe=pic-be)** | 핵심 비즈니스 로직, AI 연동 모듈, 실시간 채팅 서버 및 관리자 API | Java 17, Spring Boot, JPA, PostgreSQL, Redis, Docker |
| **[📂 SafePic-Frontend](https://github.com/safe-pic/safe-pic-fe)** | 사용자 앱(RN) 및 서비스 운영을 위한 관리자 대시보드(React) | React Native, React, Redux, Styled Components |

---

## ✨ 핵심 차별화 기능 (Key Features)

### 1. Safe-Verify 실시간 채팅 시스템
구매자가 '실물 인증'을 요청하면 판매자가 즉석에서 촬영한 사진을 전송합니다. 시스템은 해당 이미지를 가로채 AI 판별 엔진으로 즉시 전달합니다.

### 2. AI 이미지 신뢰도 분석
AI가 분석한 결과를 기반으로 이미지의 **진위 여부(Real/Fake)**와 **신뢰도 점수(Confidence Score)**를 산출합니다. 이 결과는 구매자에게만 '안심 알림'으로 전달되어 안전한 의사결정을 돕습니다.

### 3. 데이터 기반 운영 관리자 모드
모든 AI 판별 기록은 데이터베이스에 로깅되며, 관리자는 대시보드를 통해 오탐 여부를 확인하고 수동 보정 및 사기 의심 유저를 즉각 제재할 수 있습니다.

---

## 🛠 Tech Stack Overview

- **Languages:** Java, JavaScript/TypeScript
- **Frameworks:** Spring Boot 3.x, React Native, React
- **Database:** PostgreSQL, Redis
- **Infra:** AWS (ECS, EC2, S3, ECR), Docker, GitHub Actions
- **Communication:** WebSocket (STOMP), REST API

---

## 👨‍💻 Contributors

- **[김나연 | Nayeon Kim]** ([@GitHub_ID](https://github.com/nayeon-io)) - Backend & Infrastructure Architect
- **[최준영 | Junyeong Choi]** ([@GitHub_ID](https://github.com/Qnokka)) - Frontend & UI/UX Design

---

## 📄 License

---

Copyright © 2024 Potato Team. All rights reserved.

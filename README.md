<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/header-dark.svg">
  <img alt="HHHv-v — 디자인 의도를 이해하는 프론트엔드 개발자" src="./assets/header-light.svg" width="100%">
</picture>

<br>

웹 디자인에서 출발해 컴퓨터과핑으로 넘어온 프론트엔드 개발자입니다. 디자이너가 **왜** 그렇게 설계했는지를 먼저 이해하고, 그 의도를 화면 위에서 어긋나지 않게 구현하는 데 관신이 있습니다. 경북대학교 컴퓨터학부와 디지털아트를 복수전공하고 있으며 2027년 8월 졸업 예정입니다.

<br>

## Projects

### TONES — AI 리뷰 관제 대시보드 · Google AI Agent Challenge 대상

국내 뷰티 브랜드의 리뷰가 여러 스토어에 흩어져 있어 브랜드가 반응을 한눈에 파악하기 어렵다는 문제에서 시작했습니다. 흩어진 리뷰를 하나의 대시보드로 모으는 것이 1차 목표였습니다.

핵심 결정은 **"별점을 신뢰 지표로 쓰지 않는다"** 였습니다. 별점 5점인데 본문은 부정적이거나, 1점인데 본문은 긍정적인 경우가 흔해서 정량 점수만으로는 실제 반응이 왜곡된다고 봤습니다. 그래서 별점을 그대로 집계하는 대신, `Gemini`로 리뷰 본문을 다시 읽어 긍정·부정·중립으로 재분류하고 **내용 기반**으로 지표를 보여주도록 설계했습니다.

프론트엔드에서는 Next.js App Router의 **Server Actions로 AI·백엔드 호출을 서버 측에만 두는 구조**를 택했습니다. `Gemini` API 키 같은 크리덴셜이 클라이언트로 노출되는 것을 막기 위해서였고, 브라우저에는 결과만 내려주도록 경계를 그었습니다. 지표 시각화는 `Recharts`로 구성했습니다.

`Next.js (App Router)` · `React` · `TypeScript` · `Tailwind CSS` · `Recharts` · `Gemini`

### Hearo — 청각장애인용 가정 환경음 알림 IoT

청각장애인이 집에서 놓치기 쉬운 소리 — 화재경보 같은 긴급 상황, 노크와 도어락, 생활 소음 — 을 대신 감지해 알려주는 시스템입니다. 라즈베리파이 기기가 소리를 수집·판별하고, 앱이 그 정보를 실시간으로 전달합니다.

설계의 출발점은 **"사용자에게는 청각 채널이 닫혀 있다"** 는 제약이었습니다. 그래서 소리를 소리로 알리는 대신 **지동과 시각 알림으로 번역**해, 지금 무슨 소리가 났는지를 눈과 촉각으로 확인할 수 있게 만드는 데 초점을 뒀습니다.

현재 프론트엔드를 `JavaScript`에서 `TypeScript`로 마이그레이션하는 중입니다.

`React` · `Vite` · `JavaScript → TypeScript`

<br>

## Experience

### DataHouse Vietnam · Frontend Intern

5인 팀에서 LMS를 개발했습니다. `React`·`TypeScript` 기반에서 **클라이언트 상태와 서버 상태를 분리**해, 클라이언트 상태는 `Redux Toolkit`으로, 서버에서 받아오는 데이터는 `TanStack Query`로 나눠 관리했습니다. `spec-kit` 워크플로우를 따라 Epic 1의 기획부터 개발까지 한 사이클 전체를 경험했습니다.

<br>

## Skills

뱃지 대신 실제로 손에 익은 것들만 적었습니다.

**프론트엔드** — `React` · `TypeScript` · `Next.js`
**상태 · 데이터** — `Redux Toolkit` · `TanStack Query`
**스타일 · 시각화** — `Tailwind CSS` · `Recharts`
**워크플로우** — `spec-kit`
**디자인** — 웹 디자인 실무 · 디지털아트 복수전공 배경, 손으로 그리는 `SVG`

<br>

## Awards & Activity

- **Google AI Agent Challenge — 대상** · TONES 프론트엔드
- **2026-ITEC0401 (Hearo)** — 청각장애인용 환경음 알림 IoT 프론트엔드

<div align="center">

# 박태정 | Taejung Park
### AI Agent / LLM Application Developer

<br>

> **"AI의 작업을 통제하고 검증해, 생성물을 이해하고 설명하며 책임질 수 있는 결과로 만드는 AI-native 개발자."**

<br>

[![Interactive Portfolio](https://img.shields.io/badge/Interactive_Portfolio-taejung3852.github.io-0f172a?style=for-the-badge&logo=googlechrome&logoColor=white)](https://taejung3852.github.io)
[![GitHub](https://img.shields.io/badge/GitHub-taejung3852-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/taejung3852)
[![Email](https://img.shields.io/badge/Gmail-taejung3852%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:taejung3852@gmail.com)

</div>

---

## 🔭 Featured Projects

### 1. [FOWOCO](https://github.com/fowoco/ai) — 외국인 근로자 HR 업무 지원 서비스
> 고용허가제(EPS) 행정 대응 표현 검색 누락을 해결하기 위한 3중 RAG(Dense+Sparse Hybrid, RRF, Re-ranking) 파이프라인 및 서브그래프 구현
* **역할:** Language Assistant 서브그래프 / HWPX MCP 책임 분리 / 8인 온라인 협업 조율 (8인 팀 · 완료)
* **스택:** `Python` · `LangGraph` · `Qdrant` · `BGE-M3` · `MCP` · `FastAPI`
* **핵심:** 정량 벤치마크 평가를 통해 단일 Dense(99%) 대비 3중 분기 파이프라인의 지연 시간(60ms → 390ms) 트레이드오프를 측정하고 파이프라인 단순화 방향 도출

---

### 2. [HWPX Document Plugin](https://github.com/taejung3852/hwpx-document-plugin) — 에이전트 기반 한글 문서 편집 지원 플러그인
> XML 구조와 렌더링 이미지 듀얼 분석 매핑 및 4단계 [분석 → 사용자 확인(HITL) → 실행 → 검증] Agent Skills 워크플로우
* **역할:** MCP 서버 전반 설계 및 구현 / Agent Skills 설계 및 개발 (2인 팀 · 개발 중)
* **스택:** `Python` · `FastMCP` · `PyO3` · `Rust (rhwp)` · `Agent Skills` · `Vision`
* **핵심:** 표·빈칸 시각 배치 오차 제어를 위한 듀얼 매핑, 25종 MCP 도구 생태계 구축, 비추측 원칙 기반 불확실 필드 사전 질의 격리

---

### 3. [OwnHands](https://github.com/taejung3852/OwnHands) — 근거 기반 검증과 인간 승인 중심의 AI-native SDLC 하네스
> 에이전트의 거짓 성공(가짜 테스트 통과 등)을 차단하고 실행 증거(Fresh Evidence)와 Human Gate로 결과 품질을 통제하는 개발 하네스
* **역할:** 제품 문제의식 정립 / Thin Harness 아키텍처 설계 / 독립 검증 체계 및 피드백 루프 구축 (1인 개발 · 실무 적용 중)
* **스택:** `Codex CLI` · `Thin Harness` · `Agent Skills` · `Fresh Evidence` · `Human Gate` · `Continuous Evals`
* **핵심:** 데몬 과잉 설계를 걷어낸 파일 기반 Thin Harness, 사전 사양(Spec)과 실제 터미널 실행 로그·Diff를 1:1 대조 검증하는 독립 Verifier 운영

---

### 4. [LLM Gateway Service](https://github.com/taejung3852/llm-gateway) — 다중 LLM 선택 및 호출 통합 게이트웨이
> 비용·속도·성능·Context Length 4대 기준 Min-Max 정규화 가중합 기반 다기준 상대 평가 라우팅 및 통신 프로토콜 최적화
* **역할:** LLM Provider 연동 / 다기준 모델 우선순위 계산 로직 / 모델 호스팅 환경 구성 (2인 팀 · 완료)
* **스택:** `Java` · `Spring Boot` · `LangChain4j` · `WebSocket / SSE` · `MySQL` · `Ollama`
* **핵심:** SageMaker POC 후 자체 GPU 환경에 오픈소스 LLM(Ollama) 호스팅 및 LangChain4j 연동으로 상용 API 비용 절감, REST + SSE 단방향 스트리밍 프로토콜 분석

---

## 🛠 Tech Stack

| 분류 | 기술 및 도구 |
|---|---|
| **AI / Agent** | LangGraph · LangChain4j · MCP (Model Context Protocol) · Agent Skills · Claude Code · Codex |
| **Search & Data** | Qdrant · Hybrid Search (Dense + Sparse) · Embedding · MySQL · SQLite |
| **Backend & API** | Python · FastAPI · Java · Spring Boot · HTTP · WebSocket · Server-Sent Events (SSE) |
| **LLM Runtime** | Ollama (Local & On-Premise) · AWS SageMaker JumpStart |
| **Languages & Tools** | Python · Java · SQL · Git · GitHub |

---

## 🎓 Education & Training

* **상명대학교 소프트웨어학과** 학사 졸업 (2020.03 ~ 2026.02)
  * 학점 **3.95 / 4.5** (4학년 1학기 학과 수석)
* **KT그룹 AX전략 기획 및 멀티에이전트 서비스 개발 과정** (2026.09.07 ~ 현재, 10주 과정)
* **KT AIVLE School 9기 AI Developer** 수료 (2026.04 ~ 2026.09.03)

---

## 📜 Certifications

* **AICE Associate** (2026.04 · KT / 한국경제신문)
* **ISTQB CTFL** (2026.02 · KSTQB / ISTQB)
* **정보처리기사** (2025.09 · 한국산업인력공단)
* **SQLD (SQL 개발자)** (2025.06 · 한국데이터산업진흥원)
* **ADsP (데이터분석 준전문가)** (2025.06 · 한국데이터산업진흥원)

---

<div align="center">

[![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=taejung3852&theme=github-compact&hide_border=true&area=true)](https://github.com/taejung3852)

![Snake animation](https://raw.githubusercontent.com/taejung3852/taejung3852/output/github-contribution-grid-snake-dark.svg?sanitize=true)

<br>

[![Email](https://img.shields.io/badge/Gmail-taejung3852%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:taejung3852@gmail.com)

</div>

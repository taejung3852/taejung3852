<div align="center">

# 박태정
### AI Agent / LLM Application Developer

> **"AI의 작업을 통제하고 검증해, 생성물을 이해하고 설명하며 책임질 수 있는 결과로 만드는 AI-native 개발자."**

<br>

[![Interactive Portfolio](https://img.shields.io/badge/Interactive_Portfolio-taejung3852.github.io-2563eb?style=flat-square&logo=googlechrome&logoColor=white)](https://taejung3852.github.io)
&nbsp;
[![GitHub](https://img.shields.io/badge/GitHub-taejung3852-24292f?style=flat-square&logo=github&logoColor=white)](https://github.com/taejung3852)
&nbsp;
[![Email](https://img.shields.io/badge/Gmail-taejung3852%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:taejung3852@gmail.com)

</div>

---

## 🔭 Featured Projects

### 1. [FOWOCO](https://github.com/fowoco/ai) `2026.06 - 2026.08`
**외국인 근로자 HR 업무 지원 서비스 (8인 팀 · 완료)**
* **기술 스택:** `Python` · `LangGraph` · `Qdrant` · `BGE-M3` · `MCP` · `FastAPI`
* 고용허가제(EPS) 행정 대응 표현 검색 누락을 해결하기 위해 **Dense(BGE-M3)+Sparse Hybrid Search, RRF, Re-ranking** 3중 RAG 파이프라인 구축 (상위 5개 문서 선별)
* 정량 벤치마크 평가를 통해 **단일 Dense(99%)** 대비 3중 분기 파이프라인의 **지연 시간(60ms → 390ms)** 트레이드오프를 측정하고 구조 단순화 개선 방향 도출
* LangGraph 워크플로우 내 결합되어 있던 HWPX 파싱 로직을 **독립 MCP 서버로 분리**하여 메인 워크플로우와의 책임 경계를 명확히 하고 재사용성 확보
* 8인 온라인 협업의 논점 분산을 방지하기 위해 **[2개 조 분할 논의 → 조장 정리 → 전체 합의]** 3단계 의사결정 체계를 정립해 마감 지연 없이 완주

---

### 2. [HWPX Document Plugin](https://github.com/taejung3852/hwpx-document-plugin) `2026.07 - 현재`
**에이전트 기반 한글 문서 편집 지원 플러그인 (2인 팀 · 개발 중)**
* **기술 스택:** `Python` · `FastMCP` · `PyO3` · `Rust (rhwp)` · `Agent Skills` · `Vision`
* XML 노드 구조와 렌더링 이미지를 상호 대조하는 **듀얼 분석 매핑**을 도입하여 표·빈칸 시각 배치 오차로 인한 필드 오입력 위험 제어
* AI의 임의 추측을 방지하기 위해 **[분석 → 사용자 확인(HITL) → 실행 → 검증]** 4단계 Agent Skills 워크플로우 및 25종 MCP 도구 생태계 구축
* PyO3 기반 Rust(rhwp) 인프로세스 렌더링 브리지를 설계하여 외부 프로세스 의존성 없이 고속 렌더링 및 레이아웃 검증 수행

---

### 3. [OwnHands](https://github.com/taejung3852/OwnHands) `2026.09 - 현재`
**근거 기반 검증과 인간 승인 중심의 AI-native SDLC 하네스 (1인 개발 · 실무 적용 중)**
* **기술 스택:** `Codex CLI` · `Thin Harness` · `Agent Skills` · `Fresh Evidence` · `Human Gate` · `Continuous Evals`
* 에이전트의 거짓 성공(가짜 테스트 통과 등)으로 인한 통제력 상실을 방지하기 위해, 데몬 과잉 설계를 걷어내고 마크다운 파일 기반 **Thin Harness**로 전면 단순화
* AI의 완료 주장을 배제하고, 구현체와 분리된 독립 Verifier가 **사전 사양(Spec)과 실제 터미널 실행 로그·Diff를 1:1 대조**하며 사람이 최종 배포를 결정하는 **Human Gate** 구축
* Codex CLI 환경과 연동해 실무 개발에 매일 활용하며, 작업 중 발견한 실패 패턴과 피드백을 규칙(Rules)과 **Continuous Evals**로 축적하는 피드백 환류 체계 운영

---

### 4. [LLM Gateway Service](https://github.com/taejung3852/llm-gateway) `2025.04 - 2025.10`
**다중 LLM 선택 및 호출 통합 게이트웨이 (2인 팀 · 완료)**
* **기술 스택:** `Java` · `Spring Boot` · `LangChain4j` · `WebSocket / SSE` · `MySQL` · `Ollama`
* 모델별 특성 차이와 후보 고갈 문제를 해결하기 위해 **비용·속도·성능·Context Length 4대 기준 Min-Max 정규화** 및 가중치 기반 다기준 상대 평가 라우팅 알고리즘 구현
* SageMaker JumpStart POC 검증 후 자체 GPU 환경에 **오픈소스 LLM(Ollama) 호스팅 및 LangChain4j 연동**으로 상용 API 비용 절감
* 초기 WebSocket 도입 후 실제 요구가 단방향 토큰 스트리밍임을 확인하여 **차기 구조로 REST + SSE를 도출**하는 통신 프로토콜 트레이드오프 분석

---

## 🛠 Tech Stack

| 구분 | 기술 및 도구 |
|---|---|
| **AI / Agent** | LangGraph · LangChain4j · MCP (Model Context Protocol) · Agent Skills · Claude Code · Codex |
| **Search & Data** | Qdrant · Hybrid Search (Dense + Sparse) · Embedding · MySQL · SQLite |
| **Backend & API** | Python · FastAPI · Java · Spring Boot · HTTP · WebSocket · Server-Sent Events (SSE) |
| **LLM Runtime** | Ollama (Local & On-Premise) · AWS SageMaker JumpStart |
| **Languages & Tools** | Python · Java · SQL · Git · GitHub |

---

## 🎓 Education & Training

* **상명대학교 소프트웨어학과** 학사 졸업 (2020.03 ~ 2026.02) · 학점 **3.95 / 4.5**
* **KT그룹 AX전략 기획 및 멀티에이전트 서비스 개발 과정** (2026.09 ~ 현재, 10주 과정)
* **KT AIVLE School 9기 AI Developer** 수료 (2026.04 ~ 2026.09)

---

## 📜 Certifications

* **AICE Associate** (2026.04 · KT / 한국경제신문)
* **ISTQB CTFL** (2026.02 · KSTQB / ISTQB)
* **정보처리기사** (2025.09 · 한국산업인력공단)
* **SQLD (SQL 개발자)** (2025.06 · 한국데이터산업진흥원)
* **ADsP (데이터분석 준전문가)** (2025.06 · 한국데이터산업진흥원)

---

<div align="center">

![Snake animation](https://raw.githubusercontent.com/taejung3852/taejung3852/output/github-contribution-grid-snake-dark.svg?sanitize=true)

</div>

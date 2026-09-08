<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/profile-header-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="./assets/profile-header-light.svg" />
  <img alt="박태정 — AI 에이전트 · LLM 애플리케이션 개발자" src="./assets/profile-header-light.svg" width="100%" />
</picture>

<div align="center">
  <a href="#프로젝트">프로젝트</a> ·
  <a href="#개발-원칙">개발 원칙</a> ·
  <a href="#기술과-도구">기술과 도구</a> ·
  <a href="mailto:taejung3852@gmail.com">이메일</a>
</div>

<br />

AI의 작업 범위를 정하고 결과를 검증해, 사람이 **이해하고 설명하며 책임질 수 있는 시스템**을 만듭니다.

---

## 프로젝트

AI 서비스, 에이전트가 사용하는 도구, AI 개발 작업을 검토하는 도구를 만듭니다. 네 프로젝트의 위치를 먼저 보고, 아래에서 역할과 기술을 확인할 수 있습니다.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/profile-map-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="./assets/profile-map-light.svg" />
  <img alt="프로젝트 인덱스: FOWOCO, LLM Gateway, HWPX Document Plugin, OwnHands" src="./assets/profile-map-light.svg" width="100%" />
</picture>

<div align="center">
  <a href="#fowoco">FOWOCO</a> ·
  <a href="#llm-gateway">LLM Gateway</a> ·
  <a href="#hwpx-document-plugin">HWPX Plugin</a> ·
  <a href="#ownhands">OwnHands</a>
</div>

### AI 서비스 — 모델과 업무를 연결합니다

#### FOWOCO

**팀 프로젝트** · [저장소 열기 ↗](https://github.com/fowoco/ai)

검색과 AI 작업 흐름을 실제 업무에 연결하는 서비스입니다. 생성된 번역·안내문을 검증하고, 사람의 검토가 필요한 결과를 구분하는 흐름을 다룹니다.

- **참여 영역:** Language·Document/HWPX 및 Language runtime 연동
- **관련 기술:** Hybrid Retrieval · Reranking · FastAPI

#### LLM Gateway

**팀 프로젝트** · [비공개 저장소 열기 ↗](https://github.com/taejung3852/llm-gateway)

여러 AI 모델을 하나의 서비스에서 사용할 수 있도록 연결하는 백엔드입니다. 모델 선택과 응답을 조금씩 전달하는 스트리밍 구조를 다룹니다.

- **담당 영역:** 백엔드·AI 아키텍처, 모델 제공자 통합과 부분 응답 전달
- **역할 구분:** 프론트엔드는 팀원이 담당
- **관련 기술:** Spring Boot · LangChain4j · Ollama

### 에이전트 도구 — 문서를 안전하게 다룹니다

#### HWPX Document Plugin

**팀 프로젝트** · [비공개 저장소 열기 ↗](https://github.com/taejung3852/hwpx-document-plugin)

AI가 HWPX 문서를 다룰 때 **분석 → 변경 계획 → 사람의 승인 → 수정 → 검증**을 거치도록 돕는 도구입니다.

- **참여 영역:** 외부 rhwp 엔진과 Python을 연결하는 인프로세스 브리지 및 렌더링 연동
- **역할 구분:** 원천 렌더링 엔진 자체를 개발한 것은 아님
- **관련 기술:** MCP · Python · Rust / PyO3

### AI 개발 도구 — 개발 과정 자체를 검토합니다

#### OwnHands

**개인 프로젝트** · [비공개 저장소 열기 ↗](https://github.com/taejung3852/OwnHands)

AI의 개발 작업을 통제하고 검토하는 도구입니다. 무엇을 했는지 보여주는 **근거와 검증을 사람의 판단에 연결**합니다.

- **개발 방향:** 작업 범위, 수행 근거, 검증 결과를 함께 확인할 수 있는 구조
- **목표:** AI가 만든 변경을 사람이 다시 읽고 이해하는 부담을 줄이는 것

---

## 개발 원칙

1. **범위를 정합니다.** AI에게 맡길 일과 사람이 결정할 일을 구분합니다.
2. **근거를 확인합니다.** 생성된 결과를 그대로 믿지 않고 검증합니다.
3. **이해하고 수정합니다.** 필요한 부분을 직접 고쳐 내 것으로 만듭니다.
4. **판단할 수 있게 설명합니다.** 다른 사람이 맥락과 근거를 따라갈 수 있게 합니다.
5. **최종 결정은 사람이 합니다.** 판단과 책임을 도구에 넘기지 않습니다.

## 기술과 도구

아이콘만 보고 추측하지 않도록 실제 이름을 표시했습니다.

<div align="center">
  <img src="https://img.shields.io/badge/Python-20232A?style=flat-square&amp;logo=python&amp;logoColor=4B8BBE" alt="Python" />
  <img src="https://img.shields.io/badge/FastAPI-20232A?style=flat-square&amp;logo=fastapi&amp;logoColor=009688" alt="FastAPI" />
  <img src="https://img.shields.io/badge/Spring_Boot-20232A?style=flat-square&amp;logo=springboot&amp;logoColor=6DB33F" alt="Spring Boot" />
  <img src="https://img.shields.io/badge/Rust-20232A?style=flat-square&amp;logo=rust&amp;logoColor=F5F5F5" alt="Rust" />
  <img src="https://img.shields.io/badge/Docker-20232A?style=flat-square&amp;logo=docker&amp;logoColor=2496ED" alt="Docker" />
  <img src="https://img.shields.io/badge/GitHub-20232A?style=flat-square&amp;logo=github&amp;logoColor=F5F5F5" alt="GitHub" />
  <br />
  <img src="https://img.shields.io/badge/Codex-1D4ED8?style=flat-square&amp;logo=openai&amp;logoColor=white" alt="Codex" />
  <img src="https://img.shields.io/badge/Claude_Code-1D4ED8?style=flat-square&amp;logo=anthropic&amp;logoColor=white" alt="Claude Code" />
  <img src="https://img.shields.io/badge/MCP-1D4ED8?style=flat-square" alt="MCP" />
  <img src="https://img.shields.io/badge/Plugin-1D4ED8?style=flat-square" alt="Plugin" />
</div>

## GitHub 활동

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/contribution-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="./assets/contribution-snake-light.svg" />
  <img alt="GitHub 기여 잔디 뱀 애니메이션" src="./assets/contribution-snake-light.svg" width="100%" />
</picture>

## 교육과 자격

**KT AIVLE School** 9기 AI 개발자 트랙 (2026.03 ~ 2026.09)  
AICE Associate · ISTQB CTFL · 정보처리기사 · SQLD · ADsP

## 연락

**[taejung3852@gmail.com ↗](mailto:taejung3852@gmail.com)**

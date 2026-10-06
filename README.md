# Boyeon Kim (Yeonb0)

> Per Aspera Ad Astra

서강대학교 컴퓨터공학 · 철학 · 종교학을 함께 공부하는 학부생입니다.
모바일 · 웹 프론트엔드를 중심으로 만들고, 만든 것과 배운 것을 글과 위키로 쌓아 둡니다.

- Blog : [Bora.log](https://yeonb0.github.io/)
- GitHub : [@Yeonb0](https://github.com/Yeonb0)
- Email : kby7576@sogang.ac.kr

<br>

## Tech Stack

| 분야 | 사용 기술 |
| --- | --- |
| Mobile | React Native, Expo, TypeScript, TanStack Query, Zustand |
| Web | Next.js (App Router), React, Astro, HTML / CSS |
| Backend | Spring Boot, Java, Gradle, JPA, Flyway, PostgreSQL / MySQL |
| Systems | C / C++, Pintos, x86-64 Assembly |
| AI · Tooling | Python, Dify, llama.cpp, Jupyter |
| Knowledge | Obsidian, Quartz, Notion, Jekyll, GitHub Actions |

<br>

## Projects

### SkinTeller — 피부 반응 기반 스킨케어 분석 앱
`멋쟁이 사자처럼 중앙 해커톤` · `팀 일당백 (서강대 1조)` · **프론트엔드 단독 담당**

> 화장품에 피부를 맞추는 대신, 내 피부에 맞춘 화장품을 찾아줍니다.

- 루틴 · 피부 사진 기록 → AI 피부 분석 (트러블 · 홍조 · 색소침착 · 모공, 0 ~ 100점)
- 제품 사용 시점과 피부 변화의 시차 상관 분석, 자외선 · 습도 등 외부 변수 반영
- 성분 궁합을 적합 / 관찰 / 주의 3단계로 표시, 바코드 스캔 등록
- Phase 단위 화면 구현 → Figma 시안 비교 검수, `tsc --noEmit` + `eslint` 통과 후 커밋

**Stack** : Expo SDK 57 · React Native · TypeScript · TanStack Query · Zustand / Spring Boot 4.1 · MySQL / FastAPI · MediaPipe · OpenCV
**Repo** : [hackerthon-team-ildangbaek](https://github.com/Yeonb0/hackerthon-team-ildangbaek)

### 뿌기사주 — 수능 응원 사주 + 합격 부적 웹서비스
`멋쟁이 사자처럼 창업경진대회` · **프론트엔드**

- 수험생 대상 모바일 웹서비스, 실제 출시 · 수익화를 목표로 진행 (출시 목표 2026-10-31)
- main 보호 + feature 브랜치 + PR, CI에서 lint · typecheck · test · build 검증
- 서비스명 확정, 팀 문서 · FE 문서 체계 정리

**Stack** : Next.js (App Router) · TypeScript / Spring Boot
**Repo** : [saju-project](https://github.com/Yeonb0/saju-project)

### 라멘티드 (Ramented) — 라멘 한 그릇 단위 기록 지도 앱
**풀스택**

- 평점이 가게가 아니라 메뉴 하나에 붙는 구조 → 같은 라멘을 가게별로 비교
- `Ramen` · `RamenShop` · `ShopRamen` N:M 모델, 라멘 6축 분류 (육수 · 맑기 · 온도 · 타레 · 형태 · 스타일)
- Kakao Map Web SDK를 WebView로 연동, Flyway 마이그레이션
- Phase 기반 vertical slice 개발, 화면 개발 전 디자인 시스템 (색상 토큰 · 타이포) 먼저 구축

**Stack** : React Native · Expo · TypeScript / Spring Boot 4.1 · Java 25 · PostgreSQL · JPA
**Repo** : [ramented](https://github.com/Yeonb0/ramented)

### Layered Wiki Harness — 계층형 위키 에이전트 평가 하네스

- 개인 · 팀 · 전사 3계층 문서 집합에서 새 개념의 계층 배정과 조건부 하향 링크를 수행하는 에이전트 시스템 평가
- 규칙 기반 · 단일 프롬프트 · 기존 위키 빌더 · 제안 방법 4종 비교
- 로컬 LLM (Qwen3 8B) + bge-m3 임베딩 + Dify 워크플로우, 테스트 27개 통과

**Stack** : Python · Dify · llama.cpp · JSONL
**Repo** : [layered-wiki-harness](https://github.com/Yeonb0/layered-wiki-harness)

### Pintos — 운영체제 수업 프로젝트

- Project #1 `make grade` 100.0%
- 단계별 분할 구현 → 단계마다 검증, WSL2 로컬 개발 + 학과 서버 최종 검증

**Stack** : C · WSL2 (Ubuntu 22.04)
**Repo** : [2026-Operating-System](https://github.com/Yeonb0/2026-Operating-System)

<br>

## Writing & Knowledge Base

### Bora.log — 기술 블로그 · [yeonb0.github.io](https://yeonb0.github.io/)
Jekyll (Minimal Mistakes) 기반, 2026-01부터 **432편** 작성

| 분류 | 글 수 | 내용 |
| --- | ---: | --- |
| BOJ 풀이 | 335 | Bronze 132 · Silver 127 · Gold 70 · Platinum 6 |
| Computer System | 31 | Network 18 · Computer System 8 · Operating System 5 |
| Basic Coding | 29 | Data Structure 22 · Algorithm 6 · Discrete Math 1 |
| Language | 26 | C / C++ 13 · Programming Language 11 · Java 2 |
| Architecture · Graphics | 11 | Computer Architecture 10 · Graphics 1 |

### 기술 위키 — Obsidian → Quartz → Cloudflare Pages
- 컴퓨터공학 개념을 원자 단위 노트로 쌓고 `[[ ]]` 링크로 연결 (노트 538개 · 링크 3,071개)
- Python 파이프라인 : Notion export 정규화 → LLM 기반 원자 노트 분해 → 자동 위키링크 · 중복 / 고아 노트 리포트
- **Repo** : [Main](https://github.com/Yeonb0/Main)

### TIL
- "과거의 나에게 설명하듯" 쓰는 Today I Learned, 고정 템플릿 + GitHub Actions 자동화
- **Repo** : [TIL](https://github.com/Yeonb0/TIL)

<br>

## Activities

| 시기 | 활동 | 구분 |
| --- | --- | --- |
| 4학년 | 멋쟁이 사자처럼 14기 프론트엔드 ([Like-Lion-14](https://github.com/Yeonb0/Like-Lion-14)) | 동아리 |
| 4학년 | 멋사 중앙 해커톤 · 복커톤 · 아이디어톤 · 창업경진대회 | 대회 |
| 4학년 | AI/ML 스터디 (MNIST 중심 3단계 커리큘럼 기획) · Spring 스터디 | 스터디 |
| 4학년 | 서버 엔지니어 스터디 · 정보처리기사 스터디 (개설) | 스터디 |
| 2 ~ 3학년 | SGAEM | 학회 / 동아리 |
| 1 ~ 2학년 | 난섹션 학생회 | 학생회 |
| 1학년 | 서만창 | 학회 / 동아리 |
| 1학년 | 철학 개론 · 분석 철학 · 니체 강독 + 독일어 · 맹자 강독 한문 · 모종삼 강독 스터디 | 인문학 스터디 |
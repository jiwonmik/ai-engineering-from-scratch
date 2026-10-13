# My AI Engineering Path
<!-- Managed by the ai-engineering-from-scratch learning skills.
     Repo: https://github.com/rohitg00/ai-engineering-from-scratch -->

## Mission
커리어 전환이 목표이고, 그걸 위해 포트폴리오를 만든다 (그래서 실제로 동작하는 AI 제품을 출시하는 것도 해당).
최종 산출물: 도구, 상태, 메모리, 실패 동작, 릴리스 증거를 들여다볼 수 있는 "Observable Agent System".

## Placement
- Date: 2026-10-12
- Score: self-selected
- Route: Agent Systems Engineering (`learning-paths/agentic-ai-engineer.json`), 매니페스트 순서대로 진행
- Entry point: Phase 13: Tools and Protocols, Lesson 01 (The Tool Interface)
- Pace: as fast as possible
- Note: 이 경로는 기초(소프트웨어 엔지니어링, LLM API 호출) 위에 얹는 전문 과정이다. 막히는 전제 지식이 나오면 해당 기초 레슨으로 잠깐 돌아간다.

## Path
다음 레슨은 아래 표에서 Status가 `Do`인 첫 번째 행이다 (Phase 번호 순서가 아님).

| # | Stage | Lesson | Est. | Status |
|---|-------|--------|------|--------|
| 1 | Common Core | phases/13-tools-and-protocols/01-the-tool-interface | 45 min | Done |
| 2 | Common Core | phases/13-tools-and-protocols/05-tool-schema-design | 45 min | Do |
| 3 | Common Core | phases/13-tools-and-protocols/06-mcp-fundamentals | 55 min | Do |
| 4 | Common Core | phases/14-agent-engineering/01-the-agent-loop | 60 min | Do |
| 5 | Common Core | phases/14-agent-engineering/06-tool-use-and-function-calling | 60 min | Do |
| 6 | Role Practice | phases/11-llm-engineering/05-context-engineering | 90 min | Do |
| 7 | Role Practice | phases/14-agent-engineering/07-memory-virtual-context-memgpt | 75 min | Do |
| 8 | Role Practice | phases/14-agent-engineering/13-langgraph-stateful-graphs | 75 min | Do |
| 9 | Role Practice | phases/14-agent-engineering/28-orchestration-patterns | 60 min | Do |
| 10 | Proof Project | phases/14-agent-engineering/26-failure-modes-agentic | 60 min | Do |
| 11 | Proof Project | phases/14-agent-engineering/27-prompt-injection-defense | 75 min | Do |
| 12 | Proof Project | phases/14-agent-engineering/30-eval-driven-agent-development | 60 min | Do |
| 13 | Readiness Evidence | phases/14-agent-engineering/29-production-runtimes | 60 min | Do |
| 14 | Readiness Evidence | phases/14-agent-engineering/24-agent-observability-platforms | 45 min | Do |

Total: 865 min (약 14.5시간, 레슨 시간만. 포트폴리오 작업은 별도).

### Stage artifacts
- Common Core: 타입이 있는 도구, 검증, 종료 조건, 트랜스크립트를 갖춘 결정적 에이전트 루프
- Role Practice: 컨텍스트 예산, 메모리 정책, 체크포인트, 복구 경로를 갖춘 상태 기반 워크플로
- Proof Project: 적대적 테스트, 궤적 평가, 명시적 릴리스 게이트를 갖춘 관측 가능한 에이전트 시스템
- Readiness Evidence: 아키텍처, 실패 증거, 런타임 제어, 트레이스, 트레이드오프를 담은 케이스 스터디

### Portfolio project (learning-paths/CAREER-PRACTICE.md)
일회용 워크스페이스에서 범위가 제한된 변경을 제안하는 repository-maintenance agent.
보여줘야 할 증거: 도구 권한, 컨텍스트/상태 트레이스, 범위 밖 행동 거부, 종료, 복구, 독립적인 패치 리뷰.

## Progress log
| Date | Lesson | Quiz | Note |
|------|--------|------|------|
| 2026-10-13 | 13-tools-and-protocols/01-the-tool-interface | 1/2 | 연습문제 1~3 완료(검증기의 bool/여분 필드 구멍 수정, delete_file 추가, consequential 게이트). 형식 검증과 "해도 되는 행동인가" 게이트를 혼동함. 스키마 옵션을 Tool 필드에 두거나 일부 도구에 빠뜨리는 실수, 복사한 `.title()`로 경로가 바뀐 것을 트레이스에서 발견. |

## Review queue
- 13-tools-and-protocols/01-the-tool-interface: 형식 검증(스키마)과 권한/의미 게이트(consequential, 신뢰할 수 없는 입력)의 구분. 스키마를 통과한 호출이라도 실행을 막아야 하는 경우.

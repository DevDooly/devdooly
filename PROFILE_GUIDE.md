# GitHub 프로필 관리 가이드

[github.com/DevDooly](https://github.com/DevDooly)에서는 이 저장소 기본 브랜치의 `README.md`를 표시합니다. 이번 개편 대상은 GitHub 프로필입니다.

## 현재 구성

1. 기존 `assets/profile-banner.svg`와 개발 역량·AI 프로젝트·기술 위키·연락처로 가는 링크
2. **개발 역량** — 공개 프로필의 실무·개인 기술 범위, 업무의 AI 활용 경험, 개인 Lab의 문제 해결 사례
3. **AI와 함께 진행한 프로젝트** — Slivue·모임포켓·Platform Lab을 먼저 소개하고 추가 도구·실험·기획을 연결

대표 프로젝트는 목적, 실제 기능, 기술과 현재 상태를 읽고 소스·문서로 이동할 수 있도록 구성합니다. 기존 Lab의 세부 관측·복원 기록은 접어서 확인할 수 있습니다. 후속 운영 검증 목록은 각 프로젝트의 진행 문서에서 관리합니다.

## 2026-11-23 확인한 소개 근거

| 프로젝트 | 기능·상태 근거 | AI 활용 설명의 근거 |
| --- | --- | --- |
| Slivue | [README](https://github.com/DevDooly/Slivue/blob/main/README.md), [개발 문서](https://github.com/DevDooly/Slivue/blob/main/docs/DEVELOPMENT_REFERENCE.md) — Android 알림·답장, GitHub APK, Play 출시 준비 | [AI 작업 지침과 스킬](https://github.com/DevDooly/Slivue/blob/main/AGENTS.md) |
| 모임포켓 | [README](https://github.com/DevDooly/moim-pocket/blob/main/README.md) — 회비·장부·일정·투표·사진, Docker Compose 실행 | 사용자가 AI와 진행한 계모임 페이지로 지정. 도구별 작업량·기여 비율은 공개 기록에 없음 |
| Platform Lab | [공개 문서](https://devdooly.github.io/devdooly-platform-lab/handbook/), [소스](https://github.com/DevDooly/devdooly-platform-lab)와 [VM CI/CD](https://github.com/DevDooly/devdooly-platform-lab-vm-cicd) | 이 대화의 구현·검증·문서화 기록, [Java 예제의 AI 활용 범위](https://github.com/DevDooly/devdooly-platform-lab/blob/main/examples/java-window-analysis/PROVENANCE.md) |
| Thumbbridge | [README](https://github.com/DevDooly/Thumbbridge/blob/main/README.md), [구현·검증](https://github.com/DevDooly/Thumbbridge/blob/main/docs/DEVELOPMENT.md) — Kotlin·Android View, 개발용 debug APK | 이전 공개 프로필의 Android 개발 프로젝트를 계승. 문서에 없는 모델명·기여 비율은 추가하지 않음 |
| llm-dev-cli | [README](https://github.com/DevDooly/llm-dev-cli/blob/main/README.md) — 초기 문서·룰셋·정적 점검·로컬 대시보드 | AI 프로젝트를 위한 개발 도구라는 공개 설명 |
| AI Playground | [README](https://github.com/DevDooly/ai-playground/blob/main/README.md) — Gemini CLI, LLM 개발 환경과 AI 게시판 | 도구와 실험별 공개 안내 |
| Nasdaq is God | [README](https://github.com/DevDooly/nasdaq-is-god/blob/main/README.md), [구현 상태](https://github.com/DevDooly/nasdaq-is-god/blob/main/PROJECT_STATUS.md) — 백테스트·감성 분석 실험 | [AI 작업 지침](https://github.com/DevDooly/nasdaq-is-god/blob/main/PROJECT_RULE.md). 실제 매매 성과를 소개하는 근거는 없음 |
| PyBridge | [README](https://github.com/DevDooly/PyBridge/blob/main/README.md) — FastAPI CSV 검증·실행 스크립트 | [Gemini 개발 지침](https://github.com/DevDooly/PyBridge/blob/main/GEMINI.md) |
| Java UTC 구간 계산 | [예제](https://github.com/DevDooly/devdooly-platform-lab/tree/main/examples/java-window-analysis)와 JMH·독립 oracle | [AI 활용 범위](https://github.com/DevDooly/devdooly-platform-lab/blob/main/examples/java-window-analysis/PROVENANCE.md). [소유자 검토](https://github.com/DevDooly/devdooly-platform-lab/blob/main/docs/reviews/ai-window-owner-review.md)는 PENDING |
| RoadWitness | [README](https://github.com/DevDooly/road-witness/blob/main/README.md) — 기획·구조·합성 예시 | 기기 내 AI 기능의 설계 단계. 실행 앱·학습 모델의 완료로 표시하지 않음 |

Color Rest와 노비의 삶은 공개 개인 앱 후보로 확인했으나 README에서 AI 개발 범위를 확인하지 못해 이번 AI 모음에 넣지 않았습니다. geek-news-checker는 README에 상세 소개 근거가 부족했습니다. 이후 사용자 설명이나 공개 기록이 보완되면 추가할 수 있습니다.

## 새 VM 설치 작업의 재개 상태

2026-11-17 마지막 관측에서 별도 PR309 VM의 Ubuntu·SSH·cloud-init이 응답했습니다. 설치기는 `--check`의 systemd 빈 패턴 조회가 종료 코드 1을 반환해 멈췄습니다. 수정 커밋 `b9edd51`과 로컬 스킬 등록 `46d0969`가 준비돼 있습니다.

2026-11-23 확인한 [PR #309](https://github.com/DevDooly/devdooly-platform-lab/pull/309)는 OPEN/DRAFT이며 원격 head는 `7b6cb0d`입니다. 관리자 재시도 등록, 전체 설치, Grafana 서비스 상태·실제 로그 검증과 그 뒤 스킬 게시가 남아 있습니다. 프로필에서는 이 새 설치를 진행 중으로 표시합니다. 이 문서 정리 과정에서 VM 상태를 재조회하거나 설치를 실행하지 않았습니다.

개인 재개 명령과 상세 이력은 로컬 `RESUME-20261123.md`와 `platform-lab-setup-guide-20261116/EXECUTION-LOG.md`에 보관합니다. 공개 문서에는 접속 주소·키·비밀·원본 서비스 로그를 넣지 않습니다.

## 수정과 확인

- 공개 프로필에 있던 업무 경험과 개인 Lab의 합성 시험을 나눠 설명합니다. 성능 수치는 조건과 원본 근거를 연결할 수 있을 때 추가합니다.
- 프로젝트의 구현·APK·실행 가이드·공개 서비스·설계 단계를 각각 실제 상태로 적습니다.
- 소스에 AI 지침이 있다는 사실을 도구별 개발 기여 비율이나 사람의 채택 완료로 바꾸지 않습니다.
- 직무 소개와 기술 범위의 원문은 이전 README의 Git 이력에서 확인할 수 있습니다. 학습·자격증 상태는 새로 확인한 내용으로 갱신합니다.
- 프로필의 본문 앵커는 GitHub가 생성한 실제 ID를 사용합니다. 상단 링크는 `#user-content-개발-역량`과 `#user-content-ai와-함께-진행한-프로젝트`입니다. 파일 미리보기와 실제 사용자 프로필에서 이동을 각각 확인합니다. 링크, 접이식 기록, 기존 배너와 모바일 줄바꿈을 확인합니다.
- GitHub 프로필 소개문과 고정 저장소는 README와 별도 설정입니다. 이번 변경은 README와 이 관리 문서에 적용합니다.

대표 저장소 고정 후보는 `devdooly-platform-lab`, `Slivue`, `moim-pocket`, `llm-dev-cli`, `Thumbbridge`, `TIL`입니다. 실제 고정 여부와 순서는 프로필의 고정 저장소 편집 화면에서 확인합니다.

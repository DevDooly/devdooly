# GitHub 프로필 관리 가이드

프로필 주소는 [github.com/DevDooly](https://github.com/DevDooly)이며, 이 저장소의 기본 브랜치에 있는 `README.md`가 프로필에 표시됩니다.

## 현재 구성

1. `assets/profile-banner.svg`: 저장소에서 직접 제공하는 네이비·민트 배너
2. 상단 Platform Lab 바로가기와 백엔드·데이터 플랫폼 소개
3. `assets/platform-lab-card.svg`: 공개 Lab·소스·계획을 연결하는 대표 프로젝트 카드
4. 사용자에게 확인한 LLM 활용 사례
5. 개발 도구와 공개 프로젝트 네 가지
6. 최근 Android 앱 Slivue와 ThumbBridge
7. 실무·개인 프로젝트·학습을 구분한 기술 목록
8. TIL의 대표 기술 기록과 연락처

## 내용을 추가할 때

- 실제로 수행한 일과 공개 저장소에서 확인할 수 있는 기능을 소개합니다.
- 업무 경험, 개인 프로젝트, 학습 중인 내용을 구분합니다. CKA는 취득 전까지 준비 중으로 표기합니다.
- 시간복잡도나 처리 속도의 전후 수치는 측정 근거가 확인됐을 때 추가합니다.
- 프로젝트를 추가할 때는 목적, 대표 기능, 저장소 링크를 짧게 적습니다.
- 버전 번호를 본문에 고정하기보다 릴리스 목록이나 최신 릴리스로 연결합니다. 개발용 APK는 개발 버전임을 드러냅니다.
- 회사의 소스 코드, 내부 URL, 고객 정보, 개인 전화번호는 프로필에 넣지 않습니다.

## 배너와 링크

배너는 외부 이미지 생성 서비스 없이 GitHub 저장소의 SVG를 사용합니다. 변경할 때 라이트·다크 배경에서 가독성과 글자 잘림을 확인합니다. 이미지가 표시되지 않아도 핵심 내용은 본문에서 읽을 수 있게 유지합니다.

README를 수정한 뒤에는 GitHub Markdown 렌더링, 주요 링크, 작은 화면에서의 표 줄바꿈을 확인합니다. 프로필 소개문과 웹사이트 주소는 저장소의 README와 별도로 GitHub 사용자 프로필에서 관리됩니다. 웹사이트는 [Platform Lab](https://devdooly.github.io/devdooly-platform-lab/)으로 연결하고 기존 TIL은 상단 링크로 제공합니다. 개발 계획의 원본은 [Lab 다음 개발 계획](https://github.com/DevDooly/devdooly-platform-lab/blob/main/docs/NEXT_STEPS.md)입니다.

## 대표 저장소 후보

대표 저장소 고정은 GitHub 프로필의 고정 저장소 편집 화면에서 관리합니다. 현재 구성과 연결되는 후보는 다음과 같습니다.

- `devdooly-platform-lab`: 현재 대표 포트폴리오와 배포·운영 검증
- `llm-dev-cli`: AI 개발 도구
- `TIL`: 기술 기록
- `spring-skeleton`: 백엔드 구조
- `ai-playground`: AI 개발 실험
- `Slivue`: Android 알림 앱
- `Thumbbridge`: Android 터치 보조 앱

실제 고정 여부와 순서는 프로필 화면에서 확인합니다.
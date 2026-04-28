# 🚀 GitHub 프로필 관리 가이드

이 문서는 GitHub Stats 수치가 비어 보이는 원인 분석과 더불어, 효과적인 GitHub 프로필(가꾸기)을 위한 가이드라인을 제공합니다.

---

## 📊 1. GitHub Stats 수치 분석

현재 Stats 카드에서 'Commits' 외의 항목(Stars, PRs, Issues 등)이 비어 있거나 낮은 이유는 다음과 같을 수 있습니다.

### 1.1 Private Repository 기여도 미반영 (가장 흔한 원인)
기본적으로 GitHub Stats는 **Public 저장소**의 데이터만 집계합니다. 많은 작업을 Private 저장소에서 진행하신다면 아래 설정을 확인해야 합니다.
- **해결 방법**: GitHub 프로필 페이지의 기여도 그래프(Grass) 우측 상단 `Contribution settings` 클릭 -> `Private contributions` 체크. (Stats 카드 자체 옵션에서도 `&count_private=true` 파라미터가 필요할 수 있습니다.)

### 1.2 활동 유형의 불균형
GitHub Stats는 단순히 코드를 올리는 것(Commit) 외에, 협업 지표(PR, Issue, Code Review)를 중요하게 평가합니다.
- 개인 프로젝트 위주로 작업할 경우 PR(Pull Request)을 생성하지 않고 직접 Push하는 경우가 많아 PR 수치가 낮게 나타날 수 있습니다.

---

## ✨ 2. GitHub 프로필 가꾸기 가이드라인

단순히 '잔디(기여도)'를 채우는 것을 넘어, 방문자에게 전문성을 보여줄 수 있는 방법입니다.

### 2.1 Pinned Repositories (대표 프로젝트 설정)
프로필 상단에 최대 6개의 저장소를 고정할 수 있습니다.
- **선정 기준**: 가장 코드가 깔끔한 프로젝트, 현재 주력하고 있는 기술 스택이 포함된 프로젝트.
- **팁**: 각 저장소에 **Social Preview 이미지**를 등록하고, **Description**과 **Topics(태그)**를 상세히 입력하세요.

### 2.2 Repository README의 품질
메인 README만큼이나 개별 프로젝트의 README가 중요합니다.
- 프로젝트 목적, 기술 스택, 실행 방법(Quick Start), 아키텍처 다이어그램을 포함하세요.
- 시각적인 자료(스크린샷, GIF 애니메이션)는 글보다 훨씬 강력한 인상을 줍니다.

### 2.3 일관된 기여 기록 (잔디 관리)
- 매일 대단한 기능을 만드는 것보다, **꾸준함**이 중요합니다.
- `TIL(Today I Learned)` 저장소를 활용하여 매일 학습한 내용을 1개의 커밋이라도 남기는 습관을 들이세요.

### 2.4 오픈소스 기여 및 협업
- 타인의 저장소에 Issue를 제기하거나 PR을 보내는 활동은 `PRs`, `Issues` 지표를 높여줄 뿐만 아니라 '함께 일하고 싶은 개발자'라는 인상을 줍니다.

### 2.5 기술 스택의 구체화
- 메인 README의 Tech Stack 섹션을 단순히 나열하기보다, **[상급/중급/관심있음]** 등으로 숙련도를 구분하여 신뢰도를 높이세요.

---

## 🎨 4. GitHub 프로필 고도화 전략 (Advanced)

프로필을 더욱 "살아있게" 만들기 위한 고급 꾸미기 팁입니다.

### 4.1 동적 데이터 연동 (Dynamic Stats)
- **WakaTime**: 주간 코딩 시간과 사용 언어 통계를 실시간으로 보여줍니다.
- **Blog RSS Feed**: `GitHub Action`을 활용하여 개인 블로그의 최신 글 목록을 자동으로 업데이트합니다.

### 4.2 시각적 요소 강화
- **Profile Banner**: [Capsule Render](https://github.com/kyechan9/capsule-render)나 직접 만든 이미지를 상단에 배치하여 아이덴티티를 드러냅니다.
- **Visitor Counter**: [HITS](https://hits.seeyoufarm.com/) 등을 사용하여 방문자 수를 시각화합니다.
- **3D Grass**: [github-profile-3d-contrib](https://github.com/yoshi389111/github-profile-3d-contrib) 액션을 사용해 입체적인 기여도 그래프를 생성합니다.

### 4.3 오픈소스 활동 배지
- **GitHub Trophies**: [github-profile-trophy](https://github.com/ryo-ma/github-profile-trophy)를 통해 획득한 성과를 트로피 형태로 전시합니다.

---

## 🛠 5. 즉시 적용해볼 수 있는 Action Item (Update)
1. [ ] GitHub 설정에서 **Private Contributions** 공개 설정하기.
2. [ ] `nasdaq-is-god` 등 주요 프로젝트에 **Topics(태그)** 등록하기.
3. [ ] 상단에 나만의 **커스텀 배너** 추가하기.
4. [ ] 하단 혹은 상단에 **방문자 카운트 배지** 추가하기.

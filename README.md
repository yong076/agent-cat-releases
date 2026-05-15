# Agent Cat Downloads

[Agent Cat](https://agent-cat.vercel.app) 의 공개 빌드(macOS DMG · Windows .exe) 만 보관하는 저장소예요. 제품 소스는 비공개이고, 여기엔 릴리즈 파일과 README 만 있습니다.

Agent Cat 은 macOS 메뉴바 / Windows 트레이에서 Codex, Claude Code, Gemini CLI 의 활동을 로컬 메타데이터와 커넥터 스냅샷으로 보여주는 유틸리티입니다.

## 💬 질문 · 버그 · 기능 제안

**모두 [Issues](https://github.com/yong076/agent-cat-releases/issues) 탭에 올려주세요.**

이메일 대신 이슈에 올려주시면 다른 분들도 같은 문제 / 같은 제안을 같이 볼 수 있고, 진행 상황도 공개적으로 추적할 수 있어요. 한국어, 영어 모두 환영합니다.

- 새 이슈: <https://github.com/yong076/agent-cat-releases/issues/new>
- 전체 목록: <https://github.com/yong076/agent-cat-releases/issues>

## ⬇️ 다운로드

- **최신 릴리즈**: <https://github.com/yong076/agent-cat-releases/releases/latest>
  - macOS: `AgentCat-<버전>-<해시>.dmg`
  - Windows: `AgentCat-<버전>-win-x64-setup.exe`

## 🔧 설치

### macOS

1. Releases 페이지에서 DMG 를 받아주세요.
2. DMG 를 열고 `Agent Cat.app` 을 `응용 프로그램` 폴더로 드래그합니다.
3. 응용 프로그램에서 Agent Cat 을 실행합니다.
4. 서명되지 않은 테스터 빌드가 차단되면, 앱을 우클릭 → `열기` 또는 `시스템 설정 → 개인정보 보호 및 보안 → 열기 허용` 으로 진행합니다.
5. 첫 실행 시 안내되는 로컬 커넥터 설치 마법사를 따라가면 됩니다.

### Windows

1. Releases 페이지에서 `.exe` 인스톨러를 받아주세요.
2. 더블클릭해서 설치 마법사를 따라갑니다.
3. `Windows 에서 PC 를 보호했습니다` 창이 뜨면 **자세한 정보 → 실행** 을 눌러주세요. 코드 서명은 곧 붙일 예정입니다.
4. 설치가 끝나면 시스템 트레이에서 Agent Cat 아이콘이 나타납니다.

## 🔒 개인정보

Agent Cat 은 로컬 활동 메타데이터와 사용량 스냅샷만 읽도록 설계되어 있어요. 프롬프트 본문, 응답, 대화 기록, 코드 내용은 의도적으로 저장하지 않습니다.

- 데이터 정책 (친근 설명): <https://agent-cat.vercel.app/privacy>
- 개인정보 처리방침 (정식 문서): <https://agent-cat.vercel.app/legal/privacy>

## 🔗 더 보기

- 홈페이지: <https://agent-cat.vercel.app>
- 트렌드 페이지: <https://agent-cat.vercel.app/trends>
- 커넥터 (오픈소스): <https://github.com/yong076/agentcat-connectors>

---

## English

This repository hosts the public Agent Cat builds (macOS DMG · Windows .exe). The product source code lives in a private repository; only release artifacts and this README are public here.

Agent Cat is a menu bar (macOS) / system tray (Windows) utility that watches local Codex, Claude Code, and Gemini CLI activity through local metadata and connector snapshots.

### 💬 Questions, bugs, feature requests

**Please open them all on the [Issues](https://github.com/yong076/agent-cat-releases/issues) tab.** Filing on the tracker keeps everything public so others can see the same problem or upvote the same request. Korean and English both welcome.

### Download

- Latest release: <https://github.com/yong076/agent-cat-releases/releases/latest>

### Install

- **macOS**: Open the DMG, drag `Agent Cat.app` into `Applications`, launch it. If the unsigned build is blocked, right-click → `Open` or use `System Settings → Privacy & Security → Open Anyway`.
- **Windows**: Run the `.exe` installer. If SmartScreen flags it, click `More info → Run anyway`. Code signing is on the roadmap.

### Privacy

Prompts, responses, transcripts, and code contents are never stored. Only metadata (CPU, process names, opt-in usage events) is read.

- Data policy: <https://agent-cat.vercel.app/privacy>
- Privacy policy: <https://agent-cat.vercel.app/legal/privacy>

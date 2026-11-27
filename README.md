# Agent Cat — Claude Code & Codex usage, quota and reset monitor

**Free macOS menu bar and Windows tray app** that shows how much of your AI coding agents'
quota is left — Claude Code, OpenAI Codex, Gemini CLI and OpenCode — with iPhone and Android
companions.

- Remaining **5-hour and 7-day quota** and the next **reset time**, when the provider exposes it
- **Codex reset credits**: how many you have and when they expire; reset notifications on Mac
- Tokens and estimated cost **by model and by project folder**; history by period
- Several signed-in accounts per CLI side by side
- **Local metadata only** — prompts, replies and code are never stored or uploaded
- Free. No subscription, no paid unlocks

**Get it:** [Mac App Store](https://apps.apple.com/app/agentcat/id6769434137?mt=12) ·
[Microsoft Store](https://apps.microsoft.com/detail/9pphrk2hkvr7) ·
[Latest DMG / EXE](https://github.com/yong076/agent-cat-releases/releases/latest) ·
[iPhone](https://apps.apple.com/app/id6804198497) ·
[Android](https://play.google.com/store/apps/details?id=com.trappist.agentcat.mobile)

More: [agentcat.app](https://agentcat.app/en) ·
[Claude Code usage tracker](https://agentcat.app/claude-code-usage-tracker) ·
[Codex quota monitor](https://agentcat.app/codex-quota-monitor) ·
[Data policy](https://agentcat.app/privacy) ·
[Connector source](https://github.com/yong076/agentcat-connectors) (source-available)

Questions, bugs and feature requests: [Issues](https://github.com/yong076/agent-cat-releases/issues).

---

# Agent Cat Downloads

[Agent Cat](https://agentcat.app) 의 공개 빌드(macOS DMG · Windows .exe) 만 보관하는 저장소예요. 제품 소스는 비공개이고, 여기엔 릴리즈 파일과 README 만 있습니다.

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
4. 앱은 Apple Developer ID로 서명되고 공증(notarized)되어 있어 바로 열립니다. 그래도 경고가 뜨면 앱을 우클릭 → `열기` 로 진행합니다.
5. 첫 실행 시 안내되는 로컬 커넥터 설치 마법사를 따라가면 됩니다.

### Windows

1. Releases 페이지에서 `.exe` 인스톨러를 받아주세요.
2. 더블클릭해서 설치 마법사를 따라갑니다.
3. `Windows 에서 PC 를 보호했습니다` 창이 뜨면 **자세한 정보 → 실행** 을 눌러주세요. 코드 서명은 곧 붙일 예정입니다.
4. 설치가 끝나면 시스템 트레이에서 Agent Cat 아이콘이 나타납니다.

## 🔒 개인정보

Agent Cat 은 로컬 활동 메타데이터와 사용량 스냅샷만 읽도록 설계되어 있어요. 프롬프트 본문, 응답, 대화 기록, 코드 내용은 의도적으로 저장하지 않습니다.

- 데이터 정책 (친근 설명): <https://agentcat.app/privacy>
- 개인정보 처리방침 (정식 문서): <https://agentcat.app/legal/privacy>

## 🔗 더 보기

- 홈페이지: <https://agentcat.app>
- 트렌드 페이지: <https://agentcat.app/trends>
- 커넥터 (오픈소스): <https://github.com/yong076/agentcat-connectors>

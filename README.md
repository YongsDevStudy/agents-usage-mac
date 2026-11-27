# Agents Usage Mac

macOS 네이티브 메뉴 막대(`MenuBarExtra`)·`WidgetKit` 위젯·대시보드로 로컬 코딩 에이전트 CLI 사용량, 질문당 토큰 효율, 요금제 ROI를 분석하는 **실제 애플리케이션 구현 저장소**.

> **현재 상태**: 기획서(PRD) 고도화 및 기술 설계(ADR/TDD) 진행 중. 기획 확정 후 구현 이슈 수립 및 개발 착수 예정.

---

## 1. 관련 저장소 및 프로젝트 보드

| 구분 | 설명 | 링크 |
| :--- | :--- | :--- |
| **기획·지식 위키** | 시장/단가 리서치, PRD, ADR/TDD, 로컬 로그 픽스처 검증 | [YongsDevStudy/agents-usage-mac-wiki](https://github.com/YongsDevStudy/agents-usage-mac-wiki) |
| **구현 저장소 (현재)** | Swift / SwiftUI / WidgetKit 네이티브 앱 구현 | [YongsDevStudy/agents-usage-mac](https://github.com/YongsDevStudy/agents-usage-mac) |
| **Organization Project** | 전체 로드맵 및 마일스톤 관리 보드 | [Agents Usage Mac Roadmap (#3)](https://github.com/orgs/YongsDevStudy/projects/3) |

---

## 2. GitHub Branch Strategy & 협업 규약

- **`main` 브랜치 보호 (GitHub Ruleset `active`)**:
  - `main` 직접 푸시·강제 푸시(`non_fast_forward`)·브랜치 삭제 차단
  - 모든 변경은 이슈 기반 작업 브랜치(`feat/<issue>-<desc>`, `fix/<issue>-<desc>`, `refactor/<issue>-<desc>`, `chore/<issue>-<desc>`)에서 PR로만 머지
  - 미해결 리뷰 스레드 해결(`required_review_thread_resolution`) 필수
- **커밋 컨벤션**: `[#<issue>] <type>(<scope>): <Imperative description>`
- **프라이버시 원칙**: 프롬프트·코드 원문, 로컬 DB, 토큰/시크릿 파일 커밋 절대 금지

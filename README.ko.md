# Notion Skills for Claude

Notion에서 직접 제작한 공식 Claude Skills입니다. Claude가 Notion에서 실제 워크플로우를 수행하는 방법을 가르칩니다.

> [English README](README.md) | [Original Notion Page](NOTION.md)

## 개요

Notion Skills는 Claude가 Notion에서 전체 워크플로우를 완수할 수 있도록 돕는 단계별 가이드입니다. 페이지 구조화, 데이터베이스 업데이트, 패턴 따르기, 실제 프로세스 수행 등을 지원합니다.

## 사용 가능한 Skills

| Skill | 설명 |
|-------|------|
| [notion-meeting-intelligence](skills/notion-meeting-intelligence/) | Notion에서 컨텍스트를 수집하여 회의 자료, 사전 읽기 자료, 안건 작성 |
| [notion-research-documentation](skills/notion-research-documentation/) | 여러 페이지의 내용을 종합하여 구조화된 리서치 보고서 작성 |
| [notion-knowledge-capture](skills/notion-knowledge-capture/) | 대화 내용을 Notion의 구조화된 문서로 변환 |
| [notion-spec-to-implementation](skills/notion-spec-to-implementation/) | 제품/기술 스펙을 구현을 위한 구체적인 Notion 태스크로 변환 |

## 설치 방법

### Claude.ai

1. 원하는 skill의 `.zip` 파일 다운로드
2. **Settings** > **Capabilities** > **Skills** 열기
3. `.zip` 파일 업로드
4. `...` > **Try in chat** 클릭하여 시작

### Claude Code

skill 폴더를 프로젝트 또는 개인 skills 디렉토리에 복사:

```bash
# 개인 skills (모든 프로젝트에서 사용 가능)
cp -r skills/notion-meeting-intelligence ~/.claude/skills/

# 프로젝트 skills (팀과 공유)
cp -r skills/notion-meeting-intelligence .claude/skills/
```

## Skill 구조

각 skill은 표준 Claude Skills 형식을 따릅니다:

```
skill-name/
├── SKILL.md           # 핵심 지침 (YAML frontmatter + markdown)
├── evaluations/       # 테스트 시나리오
├── examples/          # 사용 예시
└── reference/         # 템플릿 및 가이드
```

## 참고 자료

- [Skills란 무엇인가?](https://support.claude.com/en/articles/12512176-what-are-skills)
- [Claude에서 Skills 사용하기](https://support.claude.com/en/articles/12512180-using-skills-in-claude)
- [Agent Skills 문서](https://docs.claude.com/en/docs/agents-and-tools/agent-skills/overview)
- [Anthropic Skills 저장소](https://github.com/anthropics/skills)

## 라이선스

이 skills는 Notion에서 제공합니다. 개별 skill 폴더에서 구체적인 조건을 확인하세요.

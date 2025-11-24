# Commit Message Rules

## Format

```
<type>: <subject>

<body>
```

## Rules

- **Use Korean** 한국어로 작성!
- **Be concise**: Shorter is easier to understand. Focus on the essence rather than implementation details.
- **body**: Optional. Write only when necessary. Explain implementation direction and reasoning. Provide context. Keep it brief. Don't write detailed implementation explanations.
- **NO template phrases**: Prohibit "Generated with Claude Code", "Co-Authored-By", etc.

## Examples

```
✅ Good example:
refactor: 배틀 모달 복수 모듈 선택 지원

- 객관식/주관식 복수 선택 가능
- 관심사 분리로 파일 분할

❌ Bad example:
refactor: 배틀 모달 복수 모듈 선택 지원

- PageLayout의 공통 레이아웃 시스템 적용
- Container에서 max-width, min-width, 가운데 정렬 제거
- ResultHeader에 height: 36px, margin-top: 60px 추가
(Too detailed!)

🤖 Generated with Claude Code
Co-Authored-By: Claude
(Template phrases prohibited!)
```

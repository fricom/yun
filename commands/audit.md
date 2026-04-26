---
name: audit
description: 코드베이스 또는 Figma 라이브러리의 컴포넌트 일관성을 감사합니다.
---

<instructions>
audit 에이전트를 사용하여 컴포넌트 감사를 실행합니다.

## 사용법
```
/audit [디렉토리 경로 | Figma 라이브러리 URL] [--scope tokens|components|patterns|all]
```

## 예시
```
/audit src/components/ --scope all
/audit https://figma.com/design/xxx --scope tokens
/audit src/styles/ --scope tokens
```

## 감사 항목
- **tokens**: 하드코딩 값, 미사용 토큰, 네이밍 비일관성
- **components**: 중복 컴포넌트, 상태 미정의, 반응형 누락
- **patterns**: 동일 문제의 다른 해결 패턴, 접근성 패턴 누락
- **all**: 전체 감사 실행

## 처리 흐름
1. 대상 스코프 파일/라이브러리 스캔
2. 인벤토리 생성
3. 불일치·중복·누락 탐지
4. 심각도별 정렬 및 개선 로드맵 제안
</instructions>

---
name: copy
description: UX 카피를 작성하거나 기존 텍스트를 사용자 중심으로 개선합니다. CTA, 에러 메시지, 빈 상태, 온보딩 텍스트 등을 지원합니다.
---

<instructions>
copy 에이전트를 사용하여 UX 카피를 작성하거나 개선합니다.

## 사용법
```
/copy [파일 경로 | 텍스트] [--type cta|error|empty|onboarding|tooltip|all]
```

## 예시
```
/copy "확인" --type cta
/copy "오류가 발생했습니다." --type error
/copy src/components/EmptyState.tsx --type empty
/copy src/pages/ --type all
```

## 카피 유형
- **cta**: 버튼, 링크 텍스트 개선
- **error**: 에러·경고·검증 메시지 개선
- **empty**: 빈 상태 텍스트 작성
- **onboarding**: 온보딩·튜토리얼 텍스트 개선
- **tooltip**: 툴팁·헬프 텍스트 개선
- **all**: 파일 내 모든 텍스트 검토

## 처리 흐름
1. 대상 텍스트 수집
2. UX 라이팅 원칙 기반 평가
3. 원본/개선안 대조 형식으로 제안
4. 변경 이유 설명 포함
</instructions>

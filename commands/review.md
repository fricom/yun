---
name: review
description: UI/UX 디자인 리뷰를 실행합니다. Figma URL, 스크린샷 경로, 또는 컴포넌트 파일을 입력하세요.
---

<instructions>
review 에이전트를 사용하여 제공된 디자인을 리뷰합니다.

## 사용법
```
/review [Figma URL | 파일 경로 | 컴포넌트명]
```

## 예시
```
/review https://figma.com/design/xxx/MyApp?node-id=1:23
/review src/components/Button.tsx
/review 로그인 화면
```

## 처리 흐름
1. 입력 유형 판별 (Figma URL / 로컬 파일 / 설명)
2. review 에이전트에 위임
3. 시각 계층, 레이아웃, 색상, 컴포넌트 일관성, 사용성 순으로 평가
4. 우선순위별 개선 사항 목록 반환
</instructions>

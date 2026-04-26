---
name: specs
description: Figma 디자인 또는 컴포넌트 파일에서 개발 핸드오프용 스펙 문서를 자동 생성합니다.
---

<instructions>
specs 에이전트를 사용하여 디자인 스펙을 추출하고 문서화합니다.

## 사용법
```
/specs [Figma URL | 컴포넌트 경로] [--format markdown|json]
```

## 예시
```
/specs https://figma.com/design/xxx?node-id=2:45
/specs src/components/Card.tsx --format json
```

## 출력 내용
- 컴포넌트 크기 및 간격 (px / rem)
- 색상값 (HEX + 디자인 토큰명)
- 타이포그래피 스케일
- 상태별(default, hover, focus, disabled, error) 스펙
- 반응형 중단점별 레이아웃
- 에셋 목록 (아이콘, 이미지)
- 애니메이션/트랜지션 값
</instructions>

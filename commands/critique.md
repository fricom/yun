---
name: critique
description: 닐슨의 10가지 휴리스틱을 기반으로 UX 크리틱을 수행합니다.
---

<instructions>
critique 에이전트를 사용하여 휴리스틱 평가 기반의 UX 크리틱을 수행합니다.

## 사용법
```
/critique [Figma URL | 화면 설명] [--heuristic 번호]
```

## Nielsen의 10가지 휴리스틱
1. 시스템 상태 가시성
2. 실제 세계와의 일치
3. 사용자 통제 및 자유
4. 일관성과 표준
5. 오류 방지
6. 재인식 vs. 회상
7. 사용의 유연성과 효율성
8. 심미적이고 미니멀한 디자인
9. 오류 인식, 진단, 복구 지원
10. 도움말과 문서

## 예시
```
/critique https://figma.com/design/xxx?node-id=3:10
/critique 결제 플로우 --heuristic 5,9
```

## 처리 흐름
1. 대상 화면/플로우 분석
2. 10가지 휴리스틱 각각에 대해 평가 (Pass / Warning / Fail)
3. 실제 스크린샷/코드의 구체적 위치 참조
4. 심각도 점수 (1-4) 및 개선 방향 제시
</instructions>

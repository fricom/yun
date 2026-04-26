# UX Designer Plugin for Claude Code

UI/UX 시니어 디자이너 워크플로우를 위한 Claude Code 플러그인.

## 커맨드 → 에이전트 매핑

| 커맨드 | 에이전트 | 기능 |
|---|---|---|
| `/review` | `agents/review.md` | 시각 계층·레이아웃·사용성 디자인 리뷰 |
| `/a11y` | `agents/a11y.md` | WCAG 2.1 AA/AAA 접근성 검사 |
| `/specs` | `agents/specs.md` | Figma → 개발 핸드오프 스펙 생성 |
| `/critique` | `agents/critique.md` | 닐슨 10 휴리스틱 UX 평가 |
| `/audit` | `agents/audit.md` | 토큰·컴포넌트·패턴 일관성 감사 |
| `/copy` | `agents/copy.md` | UX 카피 작성 및 개선 |

## 빠른 사용 예시

```bash
/review https://figma.com/design/xxx?node-id=1:23
/a11y src/pages/Login.tsx --level AA
/specs https://figma.com/design/xxx?node-id=2:45
/critique 결제 플로우 --heuristic 5,9
/audit src/components/ --scope all
/copy "확인" --type cta
```

## 설치

```bash
cp -r ux-designer-plugin/.claude-plugin <your-project>/.claude-plugin
cp -r ux-designer-plugin/agents <your-project>/agents
cp -r ux-designer-plugin/commands <your-project>/commands
```

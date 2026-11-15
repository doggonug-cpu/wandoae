# Copilot Instructions — `doggonug-cpu/wandoae`

> 전체 규칙은 저장소 루트의 [`AGENTS.md`](../AGENTS.md) 를 따른다. 이 파일은 Copilot 이
> 짧게 참조하는 요약이며, 충돌하면 `AGENTS.md` 가 우선한다.

## 프로젝트 한 줄 요약
완도애협동조합(Wandoae Cooperative) 공식 원페이지 웹사이트. **정적 사이트**, 빌드 없음,
GitHub Pages + 커스텀 도메인 `wandoae.me`.

## 반드시 지킬 것
- **파일**: `index.html`(사이트 전체), `assets/`(WebP 이미지 5종), `CNAME`(`wandoae.me` 고정), `README.md`, `AGENTS.md`.
  `CNAME` 은 읽기만 한다. 삭제·수정 금지. 사진은 모두 AI 생성 이미지이므로 “AI 생성 이미지” 표기를 유지한다.
- **기술**: HTML5 + 순수 CSS(CSS 변수) + Vanilla JS. 프레임워크·번들러·npm·CSS CDN(Tailwind 포함) 금지.
  외부 스크립트 금지. 웹폰트만 허용.
- **한/영 전환**: 번역 대상 리프 엘리먼트에 `data-en="..."` 를 붙이고 JS가 `textContent` 를 교체한다.
  `data-en` 엘리먼트 안에 자식 태그를 넣지 않는다. 문구를 추가하면 한국어·영어를 반드시 함께 넣는다.
- **접근성**: 섹션별 `h2`, 페이지에 `h1` 하나. `alt`, `aria-*`, `:focus-visible`,
  `prefers-reduced-motion` 대응. 색 대비 AA.
- **반응형**: 360 / 640 / 900 / 1200px. 가로 스크롤 금지. `clamp()` 로 유동 타이포.

## 절대 금지 (신뢰 규칙)
- 없는 인증·수상·특허·파트너사·고객사·후기·이용자 수치를 만들지 않는다.
- 확인되지 않은 설립연도·사업자등록번호·매출·직원 수를 쓰지 않는다.
- 가격·무료 기간·할인 등 상업 조건을 임의로 만들지 않는다 → `문의` 로 연결.
- `[사업자번호]`, `TODO`, `Lorem ipsum` 같은 빈 placeholder 를 커밋하지 않는다.
- 이메일 도메인은 `contact@wandoae.me` (`.com` 아님).
- `doggonug-cpu.github.io` 저장소에 이 도메인의 `CNAME` 을 만들지 않는다(HTTPS 충돌 이력).
- DNS·도메인·Pages 설정 변경, `main` force push, 무단 배포 금지 — 사람 확인 후.

## 사업 사실 (카피 작성 시 이 범위만)
1. **마인드 쉴드(Mind Shield)** — 시니어 기억 복원·인지 방어, B2G. 구술 인터뷰 → AI 원고 →
   모바일 자서전(생애 화보집) → AI 수채화 삽화·육성 오디오 → A4 1장 월간 리포트(SGDS 노인우울척도 추이 + 전문가 소견 3줄).
   현재 **개발 중 / 기관 파일럿 준비**. 대상: 노인복지관·주간보호센터·치매안심센터·지자체 돌봄 사업단.
2. **완도 특산물 온라인·B2B 유통** — 동결건조 매생이, 전복 만능볶음장 등. 온라인 직판 + 기업·기관 답례품.
3. **초등 에듀테크·AI 교육 콘텐츠** — 엔트리·마이크로비트·캔바 수업 지도안, 활동지, 웹 교구.

## 톤
담백한 존댓말. 과장 형용사 금지. 한국어 `word-break: keep-all`. 영어 표기는 `Wandoae Cooperative` 고정.

## 커밋
Conventional Commits (`feat:`, `fix:`, `style:`, `docs:`). 한 커밋 한 변경.
커밋 전 3크기(360/768/1280) 확인, 한/영 전환 확인, `cat CNAME` 확인.

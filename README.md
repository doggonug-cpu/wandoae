# 🌊 완도애협동조합 공식 웹사이트 (Wandoae Cooperative)

완도에서 나고 자란 것들을 조용한 기술로 잇는 지역 협동조합, 완도애협동조합의 공식 원페이지 사이트입니다.

- **운영 주소**: <https://wandoae.me>
- **공식 연락처**: contact@wandoae.me
- **기술 스택**: HTML5 · CSS(순수) · Vanilla JS · GitHub Pages (빌드 없음)
- **언어**: 한국어 기본 / 영어 전환 (우상단 KO·EN, `?lang=en`)

## 사업 영역

| # | 사업 | 대상 | 단계 |
|---|---|---|---|
| ① | 마인드 쉴드(Mind Shield) — 시니어 기억 복원·인지 방어, B2G | 노인복지관·주간보호센터·치매안심센터·지자체 돌봄 사업단 | 개발 중 / 기관 파일럿 준비 |
| ② | 완도 특산물 온라인·B2B 유통 | 온라인 소비자, 기업·기관 답례품 | 운영 준비 |
| ③ | 초등 AI·에듀테크 교육 콘텐츠 | 초등 교사, 방과후 강사, 디지털튜터 | 콘텐츠 제작·판매 준비 |

## 파일 구조

```
index.html   사이트 전체 (HTML + CSS + JS)
CNAME        wandoae.me  ← 삭제·수정 금지
AGENTS.md    AI 코딩 에이전트·기여자 작업 규칙
.github/copilot-instructions.md
README.md
```

## 로컬에서 보기

```bash
python3 -m http.server 8080
# → http://localhost:8080
```

## 배포

`main` 브랜치 루트가 그대로 GitHub Pages로 배포됩니다. push 후 1~2분 내 반영.

> ⚠️ `doggonug-cpu.github.io` 저장소에는 `wandoae.me` CNAME을 만들지 마세요.
> 두 저장소가 같은 도메인을 주장하면 HTTPS 인증서 발급이 중단됩니다. (2026-11-09 발생 이력)

## 편집 규칙 요약

- 확인되지 않은 수치·인증·후기·고객사는 쓰지 않습니다.
- 개발 중인 기능은 "개발 중"으로 표기합니다.
- 문구를 추가하면 한국어와 영어를 함께 넣습니다(`data-en` 속성).

자세한 규칙은 [AGENTS.md](AGENTS.md)를 참고하세요.

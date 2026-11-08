# STRUCTURE · choseokroasters-sample

```
choseokroasters-sample/
├─ index.html              단일 파일 (CSS·JS 인라인)
├─ wrangler.toml           name = choseokroasters-sample → choseokroasters-sample.lgt3232.workers.dev (Worker 이름도 같게)
├─ .assetsignore           img/ · 문서 · index_*.html · _deploy 배포 제외
├─ cs-notoserif.woff2      한자 · 제목 (Noto Serif KR 500–900, 쓰는 글자만)
├─ cs-pretendard.woff2     본문 (Pretendard 400–700, 한자 없음)
├─ cs-logo.webp / cs-logo-w.webp   검정 · 흰색 배지 로고 · favicon.png
├─ cs-hero.webp            히어로 팀 사진 (v0.2 · img/hero.jpg)
├─ cs-hero-logo.webp       히어로 礎石 로고 (흰색 · v0.3 · 사장님 누끼)
├─ cs-bean-eumyeong / chaegwang / jeongjeok .webp   원두 카드 그래픽 (img/1_jpg · multiply)
├─ cs-green / cs-roast / cs-brew .webp   Roasting 3단계 (brew = img/brewing.jpg)
├─ cs-bakery / cs-bakery-team .webp      베이커리팀 섹션 (#cups)
├─ cs-space-1~3.webp       Space (img/cpn1~3)
├─ og-choseok.jpg
├─ img/                    다올 제공 원본 55장 (배포 제외 · 직원 얼굴 · 타 브랜드 포함, 레포에 올리지 말 것)
└─ CHANGELOG.md / STRUCTURE.md
```

## 섹션 순서
헤더(종이) → 히어로(어두움) → `#beans`(종이) → `#roast`(어두움) → `#cups`(종이) → `#space`(어두움) → `#stores`(종이) → 푸터(어두움) + 모바일 `.quick`.

## 원두 카드 수정
`.bean` 하나 = 원두 1종. 점 계량 `<i class="f">`=채움 · `<i class="h">`=반 · `<i>`=빈 칸(5개). aria-label 점수도 같이 수정.

## 지점 정보 수정
`#stores .store` 3개 + head JSON-LD `@graph` 3개. 지점명: 초석로스터스 삼산 · 국가정원 · 한남(v0.2). 메타 설명 · 푸터에도 지점명 있음.

## 폰트 재생성
문구 · 한자를 바꾸면 빠진 글자 검사(LESSONS §26). 한자는 Noto Serif 요소에만(Pretendard엔 한자 없음).

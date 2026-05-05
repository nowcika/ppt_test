---
version: alpha
name: Keynote Dark
description: Apple Keynote에서 영감받은 드라마틱한 다크 프레젠테이션 시스템. 풀블리드 타일이 라이트/다크/그라디언트를 교차하며 리듬을 만들고, 단일 액센트 블루가 모든 인터랙티브 요소를 담당한다. 장식적 그라디언트나 복잡한 그림자 없이, 제품·데이터·메시지가 스스로 말하게 한다.

colors:
  accent: "#0066cc"
  accent-bright: "#2997ff"
  black: "#000000"
  near-black: "#1d1d1f"
  dark-tile: "#272729"
  white: "#ffffff"
  parchment: "#f5f5f7"
  muted: "rgba(255,255,255,0.55)"
  overline: "#2997ff"
  text-gradient-start: "#2997ff"
  text-gradient-end: "#0066cc"
  text-gradient-mid: "#5ac8fa"
  slide-gradient-start: "#0a0a0f"
  slide-gradient-mid: "#0d1b40"
  slide-gradient-end: "#071428"
  card-bg: "rgba(255,255,255,0.05)"
  card-border: "rgba(255,255,255,0.08)"
  do-bg: "rgba(0,102,204,0.08)"
  do-border: "rgba(0,102,204,0.3)"
  dont-bg: "rgba(255,59,48,0.06)"
  dont-border: "rgba(255,59,48,0.2)"
  danger: "#ff3b30"

typography:
  font-display: "Pretendard Variable, -apple-system, BlinkMacSystemFont, sans-serif"
  font-mono: "JetBrains Mono, monospace"
  xl:
    fontSize: 72px
    fontWeight: 800
    lineHeight: 1.05
    letterSpacing: -1.5px
  lg:
    fontSize: 52px
    fontWeight: 700
    lineHeight: 1.08
    letterSpacing: -0.8px
  md:
    fontSize: 36px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.3px
  sm:
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.6
  xs:
    fontSize: 15px
    lineHeight: 1.6
  overline:
    fontSize: 11px
    fontWeight: 500
    letterSpacing: 3px
    textTransform: uppercase
    color: "{colors.overline}"
  section-label:
    fontSize: 11px
    letterSpacing: 3px
    textTransform: uppercase
    color: "{colors.overline}"

rounded:
  none: 0px
  sm: 6px
  md: 10px
  lg: 14px
  xl: 16px
  pill: 9999px

spacing:
  xs: 8px
  sm: 16px
  md: 24px
  lg: 32px
  xl: 48px
  xxl: 64px
  section: 80px

slide-variants:
  slide-dark:
    background: "{colors.black}"
    color: "{colors.white}"
  slide-tile:
    background: "{colors.dark-tile}"
    color: "{colors.white}"
  slide-gradient:
    background: "linear-gradient(145deg, {colors.slide-gradient-start} 0%, {colors.slide-gradient-mid} 50%, {colors.slide-gradient-end} 100%)"
    color: "{colors.white}"
  slide-light:
    background: "{colors.parchment}"
    color: "{colors.near-black}"

components:
  progress-bar:
    height: 2px
    backgroundColor: "{colors.accent}"
    position: fixed top-0 left-0
  counter:
    fontSize: 11px
    letterSpacing: 1px
    color: "rgba(255,255,255,0.35)"
    fontFamily: "{typography.font-mono}"
    position: fixed bottom-22 right-32
  hint:
    fontSize: 11px
    color: "rgba(255,255,255,0.25)"
    position: fixed bottom-22 left-32
  fullscreen-btn:
    background: "rgba(255,255,255,0.08)"
    border: "1px solid rgba(255,255,255,0.12)"
    color: "rgba(255,255,255,0.5)"
    borderRadius: "{rounded.sm}"
    padding: 6px 14px
    position: fixed top-20 right-32
  slide-base:
    position: absolute
    inset: 0
    display: flex flex-col center center
    textAlign: center
    padding: 64px 96px
    transition: opacity 0.4s ease
  overline:
    marginBottom: 20px
    color: "{colors.overline}"
  text-gradient:
    background: "linear-gradient(135deg, {colors.text-gradient-start} 0%, {colors.text-gradient-end} 60%, {colors.text-gradient-mid} 100%)"
    backgroundClip: text
    WebkitTextFillColor: transparent
  agenda-item:
    display: flex align-center
    gap: 20px
    padding: 14px 20px
    borderRadius: "{rounded.md}"
    background: "rgba(255,255,255,0.04)"
    border: "1px solid rgba(255,255,255,0.07)"
  agenda-num:
    fontSize: 11px
    fontFamily: "{typography.font-mono}"
    color: "{colors.overline}"
    letterSpacing: 1px
  swatch:
    width: 120px
    borderRadius: "{rounded.lg}"
    border: "1px solid rgba(255,255,255,0.1)"
  swatch-color:
    height: 70px
  swatch-info:
    padding: 10px 12px
    background: "rgba(255,255,255,0.05)"
  comp-card:
    padding: 24px
    borderRadius: "{rounded.xl}"
    background: "{colors.card-bg}"
    border: "1px solid {colors.card-border}"
    backdropFilter: blur(10px)
  btn-primary:
    background: "{colors.accent}"
    color: "{colors.white}"
    borderRadius: "{rounded.pill}"
    padding: 12px 24px
    fontSize: 16px
    fontWeight: 400
  btn-ghost:
    background: transparent
    color: "{colors.accent-bright}"
    border: "1px solid {colors.accent-bright}"
    borderRadius: "{rounded.pill}"
    padding: 12px 24px
  btn-dark:
    background: "{colors.near-black}"
    color: "{colors.white}"
    borderRadius: "{rounded.sm}"
    padding: 8px 16px
    fontSize: 13px
  btn-active:
    transform: scale(0.95)
  pill-tag:
    padding: 10px 20px
    borderRadius: "{rounded.pill}"
    fontSize: 14px
    fontWeight: 500
    border: "1px solid rgba(255,255,255,0.15)"
    background: "rgba(255,255,255,0.05)"
  flow-icon:
    width: 64px
    height: 64px
    borderRadius: "{rounded.pill}"
    background: "rgba(41,151,255,0.12)"
    border: "1px solid rgba(41,151,255,0.3)"
    fontSize: 26px
  shadow-product:
    boxShadow: "rgba(0,0,0,0.22) 3px 5px 30px 0"
  closing-line:
    width: 48px
    height: 2px
    background: "{colors.accent-bright}"
    margin: 24px auto

animations:
  fade-up:
    keyframes: "from opacity:0 translateY(18px) → to opacity:1 translateY(0)"
    duration: 0.45s
    easing: ease
    stagger:
      child-1: 0.05s
      child-2: 0.12s
      child-3: 0.19s
      child-4: 0.26s
      child-5: 0.33s
      child-6: 0.40s
      child-7: 0.47s
      child-8: 0.54s
  slide-transition:
    property: opacity
    duration: 0.4s
    easing: ease

interaction:
  press-state: "transform: scale(0.95)"
  keyboard:
    next: "ArrowRight, Space"
    prev: "ArrowLeft"
    fullscreen: "F"
    notes: "S"
    first: "Home"
    last: "End"
  touch:
    threshold: 50px
    direction: horizontal
  click-nav:
    right-half: next
    left-half: prev

elevation:
  flat: none
  card: "none — border only"
  product-image: "rgba(0,0,0,0.22) 3px 5px 30px 0"
  philosophy: "그림자는 제품 이미지에만. 카드·버튼·텍스트에 그림자 없음."

slide-types:
  title:
    variant: slide-dark
    elements: [overline, xl-headline(text-gradient), subtitle(sm muted), meta(xs)]
    layout: centered-stack
  agenda:
    variant: slide-dark
    elements: [overline, lg-headline, agenda-list(6-items)]
    layout: centered-stack
  key-message:
    variant: slide-gradient
    elements: [section-label, large-quote(42px 700w), sub-text(sm muted)]
    layout: centered-stack
  section-divider:
    variant: slide-gradient
    elements: [section-label, lg-headline(partial text-gradient), description(sm muted)]
    layout: centered-stack
  color-swatch:
    variant: slide-dark
    elements: [overline, md-headline, swatch-row(5 swatches)]
    layout: centered-stack
  data-metrics:
    variant: slide-dark
    elements: [overline, md-headline, metrics-grid(3-4 large numbers)]
    layout: centered-stack
  content-list:
    variant: slide-dark
    elements: [overline, md-headline, bullet-list, footnote(xs muted)]
    layout: centered-stack
  comparison:
    variant: slide-light
    elements: [overline, md-headline, two-column-grid(do/dont or option-a/option-b)]
    layout: split-two-col
  card-grid:
    variant: slide-tile
    elements: [overline, md-headline, 3x2-card-grid(icon+title+desc)]
    layout: centered-grid
  flow-steps:
    variant: slide-gradient
    elements: [section-label, lg-headline, horizontal-flow(icons+arrows)]
    layout: centered-stack
  breakpoints:
    variant: slide-dark
    elements: [overline, md-headline, bar-chart(ascending bars), pill-tags]
    layout: centered-stack
  quote:
    variant: slide-dark
    elements: [emoji(large), blockquote(text-gradient), attribution(sm muted)]
    layout: centered-stack
  closing:
    variant: slide-dark
    elements: [overline, xl-headline(text-gradient), line-divider, tagline(sm muted), links]
    layout: centered-stack

do:
  - 모든 인터랙티브 요소에 accent(#0066cc) 단 하나만 사용
  - slide-dark ↔ slide-gradient ↔ slide-light 교차로 섹션 리듬 생성
  - pill radius는 CTA·검색·칩 등 액션 요소에만
  - 그림자는 제품/히어로 이미지에만 (shadow-product)
  - 애니메이션은 .a 클래스 stagger fade-up 하나로 통일
  - 버튼 프레스 상태는 scale(0.95) 하나로 통일

dont:
  - 두 번째 액센트 컬러 추가 금지
  - 카드·버튼·텍스트에 box-shadow 금지
  - 장식 목적의 CSS 그라디언트 배경 금지
  - body-weight 500 사용 금지 (300/400/600/700만)
  - 풀블리드 슬라이드에 border-radius 금지
  - 스피커 노트를 인라인 패널로 구현 금지 (popup window 필수)
---

## Overview

Apple Keynote에서 영감받은 **드라마틱하고 미니멀한 발표 디자인 시스템**. 슬라이드는 세 가지 배경 변형(순수 블랙 · 딥 네이비 그라디언트 · 파치먼트 화이트)을 교차하며 자연스러운 섹션 리듬을 만든다. 경계선, 장식 그라디언트, 복잡한 그림자 없이 — 타이포그래피·컬러 전환·스페이싱만으로 위계를 구성한다.

## 핵심 특성

- **단일 액센트**: `{colors.accent}` (#0066cc) 하나가 모든 인터랙티브 신호 담당
- **3종 슬라이드 변형**: slide-dark(블랙) · slide-gradient(네이비) · slide-light(파치먼트) 교차
- **텍스트 그라디언트**: 주요 헤드라인에만 `{components.text-gradient}` 적용, 남용 금지
- **Glass-morphism 카드**: 카드 그리드 슬라이드에만 backdrop-blur + 반투명 배경
- **Stagger 애니메이션**: `.a` 클래스 자녀에 0.05~0.54s 딜레이 자동 적용
- **그림자 철학**: `{elevation.product-image}` 는 히어로/제품 이미지에만, UI 요소는 flat

## 슬라이드 리듬 패턴

```
Title (dark) → Agenda (dark) → Key Message (gradient)
→ [Section: Data] (gradient) → Content (dark) → Data (dark)
→ [Section: Analysis] (gradient) → Cards (tile) → Comparison (light)
→ Quote (dark) → Closing (dark)
```

## 타이포그래피 철학

- **XL (72px/800w/-1.5px)**: 표지 타이틀 한 곳에만
- **LG (52px/700w/-0.8px)**: 섹션 분기점 헤드라인
- **MD (36px/600w/-0.3px)**: 일반 슬라이드 헤드라인
- **SM (20px/400w)**: 부제목, 리드 카피
- **XS (15px)**: 주석, 캡션
- 오버라인: 11px / 500w / 대문자 / 3px 자간 / `{colors.overline}` 색상

## 컴포넌트 사용 규칙

1. **카드 그리드**: 3×2 배치 기준, glass-morphism, 아이콘+제목+설명
2. **플로우**: 아이콘 원형(64px) + 화살표(→) 수평 배열
3. **비교**: slide-light 위에 do/dont 2열 배치
4. **메트릭**: 대형 숫자(50px+) + 단위 + 설명 3~4개 수평 배치
5. **어젠다**: 6항목 이하, 번호+텍스트 카드형 리스트

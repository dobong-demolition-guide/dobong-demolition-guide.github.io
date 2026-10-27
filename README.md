# 도봉구 철거업체 — 업데이트한 정적 홈페이지

공식 사이트명은 **도봉구 철거업체**입니다. 제공하는 서비스는 폐업철거, 상가 내부철거, 원상복구 및 관련 견적 상담입니다.
실제 상담 서비스 제공 업체명은 점포리턴으로 **푸터에 1회 명시**하고, `Organization` 구조화 데이터에는 실제 제공 업체명으로 유지했습니다. 검색 키워드를 별도 법인 상호로 표현하지 않습니다.

## 파일 구성

- `index.html`: 페이지 본문, 단일 H1, 검색 메타정보와 JSON-LD
- `style.css`와 `script.js`: 모바일/데스크톱 레이아웃, 메뉴
- `assets/*.webp`: 히어로, 안내용 사진, 시공 전후 원본을 최적화한 사진 4장, OG 이미지
- `assets/logo.svg` 및 `assets/logo-mark.svg`: 사이트명과 아이콘
- `favicon.ico`, `favicon.png`, `assets/apple-touch-icon.png`: 파비콘
- `robots.txt`, `sitemap.xml`, `.nojekyll`: 사이트 수집·설정 파일

## SEO 정보

- 사이트 이름: **도봉구 철거업체** (화면 헤더, `application-name`, `og:site_name`, `WebSite.name`)
- SEO Title: **도봉구 철거업체 | 폐업철거·상가철거·원상복구 견적 상담**
- Meta Description: 도봉구 철거업체를 찾으시나요? 창동·방학동·쌍문동·도봉동 상가의 폐업철거, 내부철거, 원상복구 비용과 폐기물 처리, 공사 일정까지 확인하고 견적을 상담하세요.
- H1: **도봉구 철거업체 | 폐업철거부터 상가 원상복구까지**
- Canonical 및 구조화 데이터의 대표 주소: **https://dobong-demolition-guide.github.io/**
- JSON-LD: `WebSite`, `WebPage`, `Organization`, `Service` (확인되지 않은 사업장 주소나 연락처는 입력하지 않음)
- 메인 키워드를 부자연스럽게 반복하지 않았으며, 도봉구 4개 동별 현장 조건, 견적서 확인사항, 사진, FAQ를 포함했습니다.

**주의:** 공식 사이트명은 검색엔진이 자체적으로 결정합니다. 일반적인 지역 키워드만으로 구성한 사이트명은 검색결과에 채택되지 않을 수 있으며, 수집·색인·통합검색 1위는 보장할 수 없습니다.

## 이미지 및 문구 변경

- 실제 시공 사진: `before_01.webp`↔`after_01.webp`, `before_02.webp`↔`after_02.webp`로 같은 현장끼리 나란히 배치했습니다. 지역/업종을 임의로 기재하지 않았습니다.
- `hero-commercial-demolition.webp`: AI 생성한 일반 작업 설명 이미지입니다. 실제 지역/업체의 수행 공사를 증명하지 않습니다.
- 과거에 첨부된 **세로형 홍보 이미지에는 다른 상호와 과거 지원금 문구**가 있어 이번 수정본에서는 **사용하지 않고 파일도 제외했습니다.** 지원사업 영역은 일반적인 설명과 견적 CTA로 대체했습니다.
- `service-store-interior.webp`, `service-partition-interior.webp`, `restoration-cleared-space.webp`는 제공된 실제 사진을 재활용한 설명용 이미지입니다.
- `service-waste-removal.webp`는 일반 설명 이미지입니다.

## 상담 및 상세 안내 링크

- 모든 상담 버튼/지원 안내 이미지 CTA:
  https://docs.google.com/forms/d/e/1FAIpQLSfdzNitwdwclnvlcy6wj8D73z8kBuRSHsiyCp-L3XB9agx9bQ/viewform?usp=header
- 추가 안내 링크 (본문 1회):
  https://store-return.netlify.app/dobong-gu-demolition-company/

## GitHub 업로드

1. `dobong-demolition-guide` Organization의 `dobong-demolition-guide.github.io` 저장소를 사용합니다.
2. **ZIP 자체가 아니라 압축 해제 후 파일 전체**를 저장소 루트에 업로드합니다. `index.html`, `style.css`, `assets` 폴더가 같은 레벨이어야 합니다.
3. 기존 파일을 덮어쓰거나 삭제된 이미지 `assets/demolition-support-guide.webp`를 저장소에서도 제거하세요. 캐시가 남으면 강력 새로고침(`Ctrl+Shift+R`) 하세요.
4. GitHub 저장소는 소스 보관용으로 사용하고, 상업적 영업 유도를 목적으로 한 웹사이트 공개는 Netlify 또는 Cloudflare Pages 등 플랫폼 정책에 맞는 정적 호스팅을 우선 검토하세요. GitHub Pages는 영업 목적의 무료 호스팅에 제약이 있습니다.
5. 새 실제 공개 주소가 `https://dobong-demolition-guide.github.io/`와 **다르면 반드시** `index.html`의 canonical, OG URL, OG 이미지/파비콘 절대경로, JSON-LD `@id`, `url`, `robots.txt`와 `sitemap.xml` URL을 새 주소로 통일하세요.
6. 공개 후 네이버 서치어드바이저에서 소유 확인, `https://실제주소/sitemap.xml` 제출, URL 검사 및 수집 상태를 확인하고, Google Search Console에서도 사이트맵과 색인 상태를 확인하세요.

## 공개 전 사실관계 점검

- 사이트를 통해 접수되는 Google Forms의 접수 주체 및 제공 업체 관계
- 실제 시공 사진의 현장별 전후 대응 관계(원자료 기준 최종 확인)
- 전체 누적 실적 5,540+, 2,190, 1,850, 4,860+의 집계 기준일과 정의 (도봉구 한정 수치 아님, 지원금 **상담** 건수는 **지급** 건수가 아님)
- 공사 가능 지역·일정, 견적의 포함/제외 범위, 최신 지원사업 공고/신청 자격
- 공개 URL 동작 및 실제 메타/사이트맵 검색엔진 수집 확인

# ChamCel (참셀) — 던파 **캐릭터 일괄 조회 / 다캐릭 조회** 배포 레포

> 이 저장소는 **정적 배포물(dist)** 만 담는 **GitHub Pages 배포용** 레포입니다.  
> 실제 개발 소스는 별도 저장소에서 빌드된 후 이곳으로 동기화됩니다.

- 라이브 사이트: **https://chamcel.github.io/**
- 결과 페이지(사용자용 딥링크): **https://chamcel.github.io/#/results**
- 결과 페이지(SEO 엔트리): **https://chamcel.github.io/results**
- 소스 저장소: https://github.com/Chamcel/Chamcel

---

## 프로젝트 소개 (SEO 키워드: *참셀*, *ChamCel*, *던파 캐릭터 일괄 조회*, *던파 다캐릭 조회*, *던전앤파이터 조회*)
**ChamCel(참셀)** 은 던전앤파이터(던파) 유저가 **여러 캐릭터 닉네임을 한 번에 입력**하면  
**장착 장비/세트포인트/명성/튜닝/인챈트/버프 강화** 정보를 **하나의 화면에서 비교**할 수 있게 해주는 웹앱입니다.  
React + Vite 기반이며, **네오플(던파) Open API**를 사용합니다.

- 다캐릭 일괄 조회(줄바꿈/쉼표 입력)
- 서버 선택: 안톤/바칼/카인/카시야스/디레지에/힐더/프레이/시로코
- 결과 섹션: 전체 요약, **무기/장착장비**, **태초(Primordial) 현황**, **버프 강화**, **융합석/내실/마부**, ...
- **라이트/다크 모드** 지원
- **검색 노출 최적화(SEO)**: OG/Twitter 메타, JSON-LD(Organization/WebSite), `sitemap.xml`·`robots.txt`
- GitHub Pages에서도 색인 안정화를 위한 **정적 엔트리 `/results`** 제공

> 검색 팁: 네이버/구글에서 **“참셀 ChamCel”**, **“던파 캐릭터 일괄 조회”** 로 검색하세요.

---

## 주요 기능 상세

- **여러 캐릭터 동시 검색**: 닉네임을 줄바꿈/쉼표로 입력 → 중복/공백 자동 정리 → 한 번에 조회
- **장착 장비 뷰**: 희귀도, 세트/세트포인트, 업그레이드, 튜닝, 인챈트(마부) 요약
- **전체 요약 테이블**: 직업/명성/세트포인트/튜닝/해방 등 핵심 지표를 비교
- **태초(Primordial) 타임라인**: 태초 아이템 획득/상태 흐름 가시화
- **버프 강화 현황**: 버프 장비/아바타/크리쳐 O/X 및 옵션/플래티넘 정리
- **검색 기록 쿠키**: 최근 닉네임 자동 저장(최대 30개)
- **반응형 UI + 테마**: 모바일/데스크톱 대응, 라이트/다크 자동 전환

---

## 기술 스택 & 배포

- **Frontend**: React, TypeScript, Vite  
- **API**: 네오플 Dungeon&Fighter Open API  
- **배포**: GitHub Pages(사용자 페이지)  
- **정적 색인 강화**: `/results/index.html`을 **MPA 엔트리**로 빌드하여 크롤러 접근성 향상

---

## SEO(검색 노출) 설정 요약

- **sitemap.xml**: 최소 `https://chamcel.github.io/`, `https://chamcel.github.io/results` 포함
- **robots.txt**
User-agent: *
Allow: /
Sitemap: https://chamcel.github.io/sitemap.xml

- **메타/OG/Twitter**: 페이지별 `<title>`, `<meta name="description">`, `og:site_name`, `og:image:width/height`
- **JSON-LD**: `Organization` + `WebSite`(+ `SearchAction`), `alternateName`: `["참셀","Chamcel"]`
- **내/외부 링크**: 푸터/README/블로그에 사이트/결과 페이지 고정 링크 제공

---

## 고지(Attribution)
본 서비스는 **네오플 Open API**를 사용하며, 게임 데이터의 모든 권리는 ⓒ **NEOPLE Inc.** 에 있습니다.

# Hiionn 소개 웹페이지

해외 환자 유치 온·오프라인 통합 파트너 **Hiionn**((주)아크로모빌리티) 브랜드 소개 원페이지 사이트입니다.

## 구성

```
hiionn-web/
├── index.html      단일 파일 랜딩 페이지 (HTML + CSS + JS 인라인)
├── images/         로고 및 콘텐츠 이미지 (상대경로 ./images/ 참조)
└── README.md
```

| 파일 | 용도 |
|---|---|
| `images/logo-horizontal.png` | 가로 로고 (헤더·푸터) |
| `images/logo-symbol.png` | 심볼 로고 (히어로·파비콘·OG 이미지) |
| `images/online-content.jpg` | 온라인 파트 섹션 |
| `images/offline-content.jpg` | 오프라인 파트 섹션 |
| `images/content-vlog.jpg` | 콘텐츠 전략 — VLOG |
| `images/content-interview.jpg` | 콘텐츠 전략 — 인터뷰 |
| `images/content-review.jpg` | 콘텐츠 전략 — 후기 |

## 로컬에서 보기

`index.html`을 브라우저로 바로 열면 됩니다. 또는 로컬 서버 실행:

```bash
python -m http.server 8000
# http://localhost:8000
```

## 배포

GitHub Pages (`main` 브랜치 `/` 루트)로 배포됩니다.
`index.html`을 수정해 커밋·푸시하면 1~2분 내 자동 반영됩니다.

## 기술 사항

- 외부 의존성 없음 (Google Fonts만 CDN 로드)
- 모든 이미지는 상대경로 `./images/` 참조 — 외부망·오프라인 환경에서도 동작
- 반응형: 980px / 768px / 430px 브레이크포인트
- SEO: meta description, Open Graph 태그, 파비콘
- 성능: 사진 `loading="lazy"`, 이미지 압축 적용 (약 775KB → 457KB)

## 이미지 교체 안내

`images/content-*.jpg`, `online-content.jpg`, `offline-content.jpg`는 **예시 목적**의
외부 인물·플랫폼 화면 및 서드파티 제안서 슬라이드가 포함되어 있습니다.
실제 대외 공개 시에는 자체 촬영 또는 저작권이 확보된 이미지로 교체하세요.
**같은 파일명으로 `images/` 안의 파일만 바꿔치기하면 코드 수정은 필요 없습니다.**

## 문의

(주)아크로모빌리티 · hiionn@acromobility.com · TEL. +82-2-6952-1617

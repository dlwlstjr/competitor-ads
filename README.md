# competitor-ads

엑셈 BX팀 경쟁사 광고 이미지 아카이브.

노션 `(온라인) 경쟁사 동향` DB에서 embed 용도로 사용. raw.githubusercontent.com 링크를 노션 image 블록에 연결하면 노션 페이지 안에서 바로 렌더링됨.

## 폴더 구조

```
competitor/
├── meta/        — Meta (Facebook/Instagram) 광고
├── google/      — Google Ads (검색·디스플레이)
└── linkedin/    — LinkedIn 광고
```

각 플랫폼 하위 경로: `{경쟁사}/{yyyy-mm}/ad-{hash}.png`

예: `competitor/meta/whatap/2026-04/ad-a3f21c.png`

## 네이밍 규칙

- **경쟁사 폴더명**: 소문자 영문 (whatap, datadog, newrelic, dynatrace, splunk, elastic, grafana-labs, honeycomb, cisco, instana, jennifersoft, sherpasoft, brains-company, nkia, watchtek, openmaru, elevisor)
- **연월**: `yyyy-mm` (예: 2026-04)
- **파일명**: `ad-{해시 6자}.png` — 동일 크리에이티브 중복 업로드 방지

## 수집 원칙

1. 원본 광고 URL과 이미지를 동시 수집
2. 이미지는 이 레포에, 원본 URL + 카피는 노션에 저장
3. 광고가 내려가도 이미지 스냅샷으로 카피·크리에이티브 파악 가능
4. 월 단위 폴더로 시계열 추적

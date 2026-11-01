# vibe 실습 모음

제주대학교 AI콘텐츠 부트캠프 1기(2026.10.26 – 11.4) 실습 파일을 날짜별로 모은 저장소예요.
배포 주소의 첫 화면(`index.html`)이 전체 목차예요 → https://vibe-nine-eta.vercel.app

## 폴더 구조

```
vibe/
├─ index.html              전체 목차 (Vercel 첫 화면)
├─ README.md               이 문서
├─ day1/                   DAY 1 · 첫 웹페이지 '제주 귤 뽑기'
├─ day2/                   DAY 2 · 특산물 홍보관 · 채팅 화면 · JavaScript 연습   (자체 저장소 day2와 같은 내용)
├─ day3/                   DAY 3 · JavaScript · JSON · 지도 · 과제
│   ├─ 과제_제출/          과제 '제주 멍때리기 좋은 명소'
│   ├─ 교안/               수업 교안
│   ├─ 실습/               연습 파일 (2 · 4 · 5.html)
│   ├─ 실습_제주대본/      제주대 수업 때 받은 연습 파일 (1 ~ 3.html)
│   ├─ 제주지도/           Leaflet + OpenStreetMap 관광지 지도
│   └─ jeju-base-data.html 제주 데이터 주제별 예제 (JSON · Key · Value)
├─ json꺼내기/             JSON 꺼내기 실습 데이 교안 · 연습장 · 과제
├─ day4/  (git 제외)       자체 저장소 day4 → 아래 '따로 관리하는 저장소'
├─ day5/  (git 제외)       자체 저장소 day5 → 아래 '따로 관리하는 저장소'
└─ _archive/ (git 제외)    받은 zip 원본 · 예전 git 백업 (이 PC에만 보관)
```

## 배포 주소 한눈에 보기

| DAY | 결과물 | 배포 주소 | 저장소 |
|---|---|---|---|
| 1 | 제주 귤 뽑기 | https://study-nine-delta.vercel.app | jeongeunlee0/study |
| 2 | 제주 특산물 홍보관 · 특산물 길잡이 | https://day2-psi-seven.vercel.app | jeongeunlee0/day2 |
| 3 | 제주 멍때리기 좋은 명소 (과제) | https://jeju-spots-project.vercel.app | jeongeunlee0/jeju_spots_project |
| 1–3 | vibe 실습 모음 (이 저장소) | https://vibe-nine-eta.vercel.app | jeongeunlee0/vibe |
| 4 | 돌하르방의 제주 텃밭 | https://day4-ten-theta.vercel.app | jeongeunlee0/day4 |
| 5 | 제주상점 · 서귀포 길잡이 | https://day5-flax.vercel.app | jeongeunlee0/day5 |
| 5 | 답사 스탬프 투어 (과제 2단계) | https://leejeongeun-step2.vercel.app | jeongeunlee0/leejeongeun-step2 |

## 따로 관리하는 저장소

`day4/`, `day5/`는 폴더 안에 각자 `.git`이 있는 별도 저장소예요. 이 저장소(vibe)에는 올리지 않고, 각 폴더에서 따로 커밋 · 푸시하면 Vercel이 자동으로 배포해요.
`day5/과제제출_26.10.30/이정은_2단계/`도 별도 저장소(leejeongeun-step2)예요.

## 파일 이름 규칙

배포된 주소가 바뀌지 않도록 **이미 있는 파일 이름은 그대로** 두고, 새로 만드는 파일부터 아래 규칙을 따라요.

| 종류 | 위치 · 이름 | 예 |
|---|---|---|
| 결과물 (배포 대상) | `dayN/주제/index.html` | `day3/제주지도/index.html` |
| 연습 파일 | `dayN/실습/번호_주제.html` (번호는 두 자리) | `day3/실습/06_반복문.html` |
| 교안 | `dayN/교안/DAYxx_대상_교안.html` | `day3/교안/DAY05_학생용_교안.html` |
| 데이터 | 쓰는 페이지 옆에 `.json` | `day3/제주지도/jeju_spots.json` |
| 문서 | 폴더마다 `README.md` 한 개 | `day1/README.md` |

- 폴더 · 파일 이름에 띄어쓰기 대신 `_`(밑줄)을 써요.
- 비밀 값(API 키)은 `.env.local`에만 두고 올리지 않아요 (`.gitignore`에 들어 있음).

## 로컬에서 보기

`fetch`로 JSON을 읽는 페이지가 있어서, 파일을 더블클릭하지 말고 서버로 열어야 해요.

```bash
python -m http.server 8000
```

`http://localhost:8000`에 접속해 목차에서 고르세요.

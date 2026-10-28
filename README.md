# vibe 실습 모음

AI 부트캠프 실습 파일을 한 곳에 모은 저장소입니다. 배포 주소의 첫 화면(`index.html`)이 전체 목차예요.

```
vibe/
├─ index.html            전체 목차 (Vercel 첫 화면)
├─ day1/                 1일차: 첫 페이지 만들기
├─ day2/                 2일차: 레이아웃·채팅·사진 검색 (자체 GitHub/Vercel 연결 유지)
├─ day3/                 3일차: JavaScript · JSON
│   ├─ 교안/             수업 교안
│   ├─ 실습/             연습 파일 (2~5.html)
│   ├─ 실습_제주대본/    제주대 수업 때 받은 연습 파일 (1~3.html)
│   └─ 제주지도/         Leaflet + OpenStreetMap 제주 관광지 지도 (index.html + jeju_spots.json)
├─ json꺼내기/           JSON 꺼내기 교안·연습장·과제
├─ _archive/             받은 zip 원본 (git/배포 제외)
└─ AI 부트캠프  Vault/   개인 노트 (git/배포 제외)
```

## 로컬에서 보기

`fetch`로 JSON을 읽기 때문에 파일을 더블클릭하지 말고 서버로 열어야 합니다.

```bash
python -m http.server 8000
```

`http://localhost:8000` 접속 후 목차에서 고르세요.

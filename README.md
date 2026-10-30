# 칼로리 사전

식품 이름만 입력하면 칼로리와 탄단지가 바로 나오는 개인용 식단 사전입니다.
단일 HTML 파일로 동작하고, 데이터는 브라우저 `localStorage`에만 저장됩니다.

- 라이브: https://calorie-dict.web.app
- Firebase 프로젝트: `calorie-dict`

## 기능

- 식품 이름 검색 (초성 검색 지원)
- 100g 기준 칼로리·탄수화물·단백질·지방 표시
- 1인분/1개 등 제공량 전환
- 오늘 먹은 음식 기록 및 합계
- 내 음식 직접 추가

## 구조

```
calorie-app/
├── index.html      앱 전체 (HTML/CSS/JS + 음식 데이터)
├── firebase.json   Firebase Hosting 설정
├── .firebaserc     프로젝트 ID
└── README.md
```

## 로컬 실행

`index.html`을 브라우저에서 열면 끝입니다. 별도 빌드나 서버가 필요 없습니다.

## Firebase 배포

```powershell
firebase.cmd deploy --only hosting
```

## 참고

- 음식 데이터는 앱 안에 내장되어 있고, 기록만 `localStorage`에 저장됩니다.
- 서버나 계정 로그인은 없습니다.

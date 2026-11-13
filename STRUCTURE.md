# STRUCTURE · mugyeolwaxing-sample (v0.2 · 사장님 공지 카드 톤)

```
mugyeolwaxing-sample/
├─ index.html                 단일 파일 (CSS · JS 인라인)
├─ wrangler.toml              name = mugyeolwaxing-sample → mugyeolwaxing-sample.lgt3232.workers.dev
├─ .assetsignore              img/ · _old/ · 문서 · index_*.html · _deploy 배포 제외
├─ mg-fraunces.woff2          영문 제목 (Fraunces 400–500 · opsz 72 · SOFT 50 · WONK 0, 대문자 포함)
├─ mg-notoserif.woff2         한글 명조 부제 · 인용 · 항목 이름 (Noto Serif KR 400–500, 페이지 글자 전부)
├─ mg-pretendard.woff2        본문 · 버튼 · 로고 글자 (Pretendard 300–600, 페이지 글자 전부)
├─ mg-leaf.webp               잎 그림자 (새로 그림, 투명 배경 · 히어로 · 마무리 프레임)
├─ mg-room.webp               히어로 아래 · 시술실
├─ mg-door.webp               05 Visit · B2층 복도 유리문
├─ mg-b1~b3-before/after.webp 04 눈썹 전후 3쌍 (버튼 data-b / data-a로 전환)
├─ favicon.png · og-mg.jpg
├─ img/                       다올 제공 원본 84장 (배포 제외 · 얼굴 · 체모 사진 · 다른 브랜드 포함, 레포에 올리지 말 것)
└─ CHANGELOG.md / STRUCTURE.md
```

## 섹션 순서
헤더(+ 900px 미만 가로 섹션 링크 `.snav`) → 히어로(프레임 카드 + 사진) → `#philosophy` → `#price` → `#care` → `#before-after` → `#visit` → 마무리(프레임 카드) → 푸터 + 모바일 `.quick`.

## 디자인 규칙 (사장님 공지 카드에서)
- 가운데 정렬 섹션 머리: 번호 라벨(브론즈, 자간 넓게) → 세로 가는 선 → 영어 제목(Fraunces) → 한글 명조 부제
- 프레임 = 1px #B9AEA2 테두리, 두 줄 라벨 = 위아래 1px 선
- 유채색은 브론즈 #7A6550 하나. 버건디 · 빨강 사용 안 함.

## 스크립트
- 가격표 여자/남자 탭: `role=tab` · 방향키 이동, JS 없으면 두 표 모두 보임(라벨 표시).
- 전후 비교: 투명 `input[type=range]`가 `--p` 값을 바꿈(키보드 · 터치 가능).
- 나타나기 효과: `.js .reveal`, 동작 줄이기에서도 재생(다올 방침).

## 링크 한곳 정리
- 네이버 플레이스 `m.place.naver.com/place/2022733941/home`: 헤더 · 히어로 · 가격 안내 · 마무리 · 하단 바
- 네이버 길찾기 `map.naver.com/p/entry/place/2022733941`: Visit
- 전화 `tel:050713602129`: 히어로 · Visit · 푸터 · 하단 바
- 인스타 `https://www.instagram.com/mugyeol_waxing/`: Visit · 푸터 · 하단 바

## 폰트 재생성
문구 바꾸면 빠진 글자 검사(LESSONS §26). 한글은 명조 · Pretendard 둘 다에 들어가야 함. 서브셋 옵션에 `--unicodes=U+0020,U+00A0`(R-6).

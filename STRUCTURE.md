# STRUCTURE · mugyeolwaxing-sample

```
mugyeolwaxing-sample/
├─ index.html                 단일 파일 (CSS · JS 인라인)
├─ wrangler.toml              name = mugyeolwaxing-sample → mugyeolwaxing-sample.lgt3232.workers.dev
├─ .assetsignore              img/ · _old/ · 문서 · index_*.html · _deploy 배포 제외
├─ mg-cormorant.woff2         영문 세리프 (Cormorant Garamond 500–600, 대문자 포함)
├─ mg-pretendard.woff2        한글 · 본문 (Pretendard 300–700, 페이지 글자 전부)
├─ mg-sign.webp               히어로 · 입구 버건디 간판
├─ mg-room.webp               01 Philosophy · 시술실
├─ mg-door.webp               05 Visit · B2층 복도 유리문
├─ mg-b1~b3-before/after.webp 04 눈썹 전후 3쌍 (버튼 data-b / data-a로 전환)
├─ favicon.png · og-mg.jpg
├─ img/                       다올 제공 원본 84장 (배포 제외 · 얼굴 · 체모 사진 · 다른 브랜드 포함, 레포에 올리지 말 것)
└─ CHANGELOG.md / STRUCTURE.md
```

## 섹션 순서
헤더(+ 900px 미만 가로 섹션 링크 `.snav`) → 히어로 → `#philosophy` → `#price` → `#care` → `#before-after` → `#visit` → 마무리 → 푸터 + 모바일 `.quick`.

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
문구 바꾸면 빠진 글자 검사(LESSONS §26). 서브셋 옵션에 `--unicodes=U+0020,U+00A0`(R-6).

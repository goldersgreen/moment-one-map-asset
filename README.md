# Moment One Map

이 리포지토리는 [Moment One](https://github.com/goldersgreen/moment_one) 모바일 앱의 카카오맵 WebView 페이지를 호스팅합니다.

## 용도

Flutter 앱에서 `InAppWebView` 가 이 페이지를 로드하여 카카오맵 JS SDK 를 실행합니다.
카카오 JS SDK 는 정식 HTTPS 도메인에서만 SDK 응답을 주므로, GitHub Pages 의 HTTPS 도메인이 필요합니다.

## 파일

- `map.html` — 카카오맵 WebView 페이지 (URL 쿼리로 키·좌표 받음)
- `.nojekyll` — GitHub Pages 의 jekyll 처리 비활성화

## URL 형식

```
https://goldersgreen.github.io/<리포명>/map.html
  ?key=<KAKAO_JS_KEY>
  &lat=<위도>
  &lng=<경도>
  &level=<줌레벨>
  &interactive=<true|false>
```

## 카카오 디벨로퍼스 등록

JavaScript 키의 JavaScript SDK 도메인에 다음을 등록해야 SDK 로드가 통과합니다:

```
https://goldersgreen.github.io
```

## 라이선스

내부 사용 전용

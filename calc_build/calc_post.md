## 정적 사이트 배포(Static Site Deployment)
 리액트 계산기 프로젝트 빌드

## package.json 수정

## package.json에 "homepage" 필드를 추가합니다.
```js
{
  "name": "your-app",
  "version": "0.1.0",
  "private": true,
  "homepage": "https://U-jinLee.github.io/mini-project/siyeon",
  "dependencies": { ... },
  "scripts": { ... }
}
```
- hwangsiyeon@hwangsiyeon-ui-MacBookPro react-calc % npm run build
- build 폴더 생성
- build 폴더 안에 index.html src 주소를 수정 된 거 확인 : src="/mini-project/siyeon/static/js/main.861eb5e9.js"
- 안에 있는 폴더&파일들을 mini-project에 추가 . 커밋

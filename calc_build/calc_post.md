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

## BrowserRouter 설정
<BrowserRouter basename="/mini-project/siyeon"> 추가


- hwangsiyeon@hwangsiyeon-ui-MacBookPro react-calc % npm run build
- build 폴더 생성
- build 폴더 안에 index.html src 주소를 수정 된 거 확인 : src="/mini-project/siyeon/static/js/main.861eb5e9.js"
- 안에 있는 폴더&파일들을 mini-project에 추가 . 커밋

## 1️⃣ GitHub Pages URL 규칙
**개인 페이지(User/Organization Pages)**

- 레포지토리 이름과 상관없이 https://<username>.github.io/ 가 기본 URL

- 예시: https://U-jinLee.github.io/
  
- 브랜치: main 브랜치 + /root 폴더

**프로젝트 페이지(Project Pages)**

- 레포지토리 이름을 포함한 URL

- 형식: https://<username>.github.io/<repository>/

- 예시: https://U-jinLee.github.io/mini-project/

- 브랜치: main 브랜치 + /root 또는 /docs 폴더

**서브폴더까지 지정**

- 프로젝트 페이지 내 특정 서브폴더를 URL로 지정 가능

- 예시: https://U-jinLee.github.io/mini-project/siyeon/ → siyeon 폴더 안의 빌드 파일이 페이지로 나옴

## 2️⃣ package.json의 "homepage" 역할

- React 앱에서 상대 경로로 만들어진 파일(bundle.js, index.html) 링크를 절대 경로로 변환

- 예: "homepage": "https://U-jinLee.github.io/mini-project/siyeon"
- → 빌드하면 index.html에서 <script src="/mini-project/siyeon/static/js/..."> 처럼 경로가 자동 적용됨

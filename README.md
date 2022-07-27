# webpack-learn

### Copyright 2020. Captain Pangyo. all rights reserved.
- https://www.inflearn.com/course%ED%94%84%EB%9F%B0%ED%8A%B8%EC%97%94%EB%93%9C-%EC%9B%B9%ED%8C%A9/dashboard


### node.js
- <code>node -v</code> : node.js 버전확인

### npm
- 명령어로 자바스크립트 라이브러리를 설치하고 관리할 수 있는 패키지 매니저
- <code>npm -v</code>
- <code>npm init</code>
- <code>npm init -y</code>
- <code>npm install ___</code>
  - NPM 지역 설치는 해당 프로젝트에서 사용할 자바스크립트 라이브러리를 설치할 때 사용
  - dependencies: 애플리케이션의 로직을 구현하는데 연관이 있는 라이브러리
- <code>npm uninstall ___</code>
- <code>npm install ___ --global</code> : 전역으로 설치된 라이브러리
  - NPM 전역 설치는 시스템 레벨에서 사용할 자바스크립트 라이브러리를 설치할 때 사용
- <code>npm i ___ -D(--save-dev)</code>
  - devDependencies: 개발보조 라이브러리

### 웹팩 webpack
- 최신 프론트엔드 프레임워크에서 가장 많이 사용되는 모듈 번들러
- 모듈 번들러: 웹 애플리케이션을 구성하는 자원을 모두 각각의 모듈로 보고 이를 조합해서 병합된 하나의 결과물을 만드는 도구
- 장점: 여러가지의 파일을 하나로 합치고 파일에 대한 요청을 한번만 보냄
- <code>npm i webpack webpack-cli -D</code>
- <code>npm i lodash</code>
- <code>"build": "webpack --mode=none"</code>
- <code>npm run build</code>

### 웹팩 주요속성
- entry
  - 웹팩에서 웹 자원을 변환하기 위해 필요한 최초 진입점이자 자바스크립트 파일 경로
  - 웹팩을 실행할 대상 파일. 진입점
- output
  - 웹팩의 결과물에 대한 정보를 입력하는 속성 -> 결과물의 파일 경로를 의미
  - 일반적으로 filename과 path를 정의
- loader
  - 웹팩이 웹 애플리케이션을 해석할 때 자바스크립트 파일이 아닌 웹 자원(HTML, CSS, Image, 폰트 등)
    들을 변환할 수 있도록 도와주는 속성
  - css, 이미지와 같은 비 자바스크립트 파일을 웹팩이 인식할 수 있게 추가하는 속성
  - 오른쪽에서 왼쪽 순으로 적용
- plugins
  - 웹팩의 기본적인 동작에 추가적인 기능을 제공하는 속성
  - 해당 결과물의 형태를 바꾸는 역할
  - 웹팩으로 변환한 파일에 추가적인 기능을 더하고 싶을 때 사용하는 속성 
  - 웹팩 변환과정 전반에 대한 제어권을 갖고 있음

### Webpack Dev Server
- 웹팩 데브 서버는 웹 애플리케이션을 개발하는 과정에서 유용하게 쓰이는 도구
- 웹팩의 빌드 대상 파일이 변경 되었을 때 매번 웹팩 명령어를 실행하지 않아도 코드만 변경하고 저장하면
  웹팩으로 빌드한 후 브라우저를 새로고침 해줌
- <code>"scripts": { "dev": "webpack serve", "build": "webpack" }</code>

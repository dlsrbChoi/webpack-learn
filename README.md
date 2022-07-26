# webpack-learn

### Copyright 2020. Captain Pangyo. all rights reserved.
- https://www.inflearn.com/course%ED%94%84%EB%9F%B0%ED%8A%B8%EC%97%94%EB%93%9C-%EC%9B%B9%ED%8C%A9/dashboard


### node.js
- node -v

### npm
- 명령어로 자바스크립트 라이브러리를 설치하고 관리할 수 있는 패키지 매니저
- npm -v
- npm init
- npm init -y
- npm install ___
  - NPM 지역 설치는 해당 프로젝트에서 사용할 자바스크립트 라이브러리를 설치할 때 사용
  - dependencies: 애플리케이션의 로직을 구현하는데 연관이 있는 라이브러리
- npm uninstall ___
- npm install ___ --global : 전역으로 설치된 라이브러리
  - NPM 전역 설치는 시스템 레벨에서 사용할 자바스크립트 라이브러리를 설치할 때 사용
- npm i ___ -D(--save-dev)
  - devDependencies: 개발보조 라이브러리

### 웹팩 webpack
- 최신 프론트엔드 프레임워크에서 가장 많이 사용되는 모듈 번들러
- 모듈 번들러: 웹 애플리케이션을 구성하는 자원을 모두 각각의 모듈로 보고 이를 조합해서 병합된 하나의 결과물을 만드는 도구
- 장점: 여러가지의 파일을 하나로 합치고 파일에 대한 요청을 한번만 보냄
- npm i webpack webpack-cli -D
- npm i lodash
- "build": "webpack --mode=none"
- npm run build

### 웹팩 주요속성
- entry
  - 웹팩에서 웹 자원을 변환하기 위해 필요한 최초 진입점이자 자바스크립트 파일 경로
- output
- loader
- plugins

 
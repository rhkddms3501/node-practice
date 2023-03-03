Node Practice

1. 패키지
    - 프로젝트 사용하는 module(라이브러리)
    - 완전한 애플리케이션(babel, webpack, nodemon)

2. 의존성
    - 개발하는 프로젝트(애플리케이션, 라이브러리)에서 설치하고 사용하는 패키지
    - 일반 의존성: 개발하고 있는 프로젝트에서 사용하는 패키지로 꼭 빌드와 배포에 포함되어야 한다.
    - 개발 의존성: 개발에 필요하거나 도움이 되는 패키지로 빌드와 배포에 포함하지 않는다.

3. 패키지 설치 (npm install or npm i)
    1) 전역설치 (global) 여러 프로젝트에서 공통으로 사용하는 도구
    2) 지역설치 (local) : 특정 프로젝트 종속적인 도구나 라이브러리
    3) 패키지 설치 실습
        $ npm i ejs             [local, general dependency]
        $ npm i -D nodemon      [local, dev, dependency]
        $ npm i -g gulp         [global, general dependency] / 실행방법: $npx gulp
        $ npx gulp --version
    4) 패키지 삭제
        $ npm un ejs            [local install uninstall]
        $ npm un nodemon        [local install uninstall]
        $ npm un -g gulp        [global install uninstall]
        $ npx gulp --version    

4. Node(javascript) project 생성
    1) 프로젝트 생성 (mkdir, 디렉토리 생성)
    2) 프로젝트 이동 (cd)
    3) 프로젝트 초기화: 프로젝트 매니페스트(Manifest) 파일인 package.json 생성
        $[project-ex01] npm init -y

5. Module
    1) 코어 모듈: node에서 제공하는 모듈(fs, os, process, http, ...)
    2) 파일 모듈: 파일 경로로 불러온 모듈안의 함수, 객체를 사용한다.
    3) npm 모듈: npm을 통해서 node_modules에 설치하고 사용하는 모듈
        - 원격 배포가 된 패키지로 
            npmjs.com의 npm registry에 패키지 배포

        - 로컬 설치
            $ npm i ../douzone-math

6. helloweb-ex01: 웹 애플리케이션 만들어 보기 (express 프레임워크 x)
7. helloweb-ex02: 웹 애플리케이션 만들어 보기 (express 프레임워크 o)
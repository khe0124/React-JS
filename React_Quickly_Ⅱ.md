# 리액트 교과서 (React Quickly)
개념정리를 전체 인데스를 파악하기 위한 요약 정리입니다.

<br>
<hr>
<br>

## 12. Webpack 빌드 도구
- 핫 모듈 대체를 작동시키려면 webpack-dev-server를 사용하고 설정에 react-hot-loader를 추가하거나 원하는 파일에 module.hot.accept()를 적용해야한다.
- style-loader와 css-loader를 사용하면 require()문으로 css를 불러올 수 있다.
- 명령줄로 --inline --hot 옵션을 추가해서 WDS를 실행하면 HMR이 적용된다.
- 설정에 devtool: '#sourcemap'을 추가하면 컴파일된 코드에서 원본 코드의 줄번호를 확인할 수 있다.
- WDS를 사용할 때는 publicPath 설정으로 번들 파일의 위치를 지정한다.

<br>

## 13. React 라우팅
- 단방향 데이터 흐름은 React앱에 예측가능성과 유지보수의 편의를 제공한다.
- Flux는 React와 단방향 데이터 흐름을 다룰 때 권장되는 아키텍쳐다.
- Redux는 Flux 아키텍처의 구현체 중 가장 인기가 좋다.
- Redux를 사용하면 액션을 스토어에 전달하거나 속성 객체에 추가할 수 있다.
- Redux의 connect()메서드는 스토어의 데이터에 접근할 수 있게 해주고 액션을 스토어에 전달할 수 있으며, 이는 컨테이너 컴포넌트에 필요한 기능이다.
- Redux의 Provider 컴포넌트가 자식 컴포넌트에서 스토어에 접근할 수 있게 해주므로 수동으로 스토어 속성을 전달하지 않아도 된다.
<br>

## 14. Redux를 이용한 데이터 다루기
- 단방향 데이터 흐름은 React앱에 예측가능성과 유지보수의 편의를 제공한다.
- Flux는 React와 단방향 데이터 흐름을 다룰 때 권장되는 아키텍처다.
- Redux는 Flux 아키텍처의 구현체 중 가장 인기가 좋다.

<br>

## 15. GraphQL을 이용한 데이터 다루기

<br>

## 16. Jest를 이용한 React 단위 테스트

<br>

## 17. React와 Node.js를 이용한 유니버셜 자바스크립트

<br>

## 18. 프로젝트: React Router를 이용한 서점 만들기

<br>

## 19. 프로젝트: Jest를 이용한 비밀번호 검사

<br>

## 20. 프로젝트: Jest,Express, MongoDB를 이용한 자동완성 컴포넌트 구현

<br>

# 리액트 교과서 (React Quickly)
개념정리를 전체 인데스를 파악하기 위한 요약 정리입니다.

<br>
<hr>
<br>

## 12. Webpack 빌드 도구
- 핫 모듈 대체를 작동시키려면 webpack-dev-server를 사용하고 설정에 react-hot-loader를 추가하거나 원하는 파일에 module.hot.accept()를 적용해야한다.
- style-loader와 css-loader를 사용하면 `require()`문으로 css를 불러올 수 있다.
- 명령줄로` --inline --hot `옵션을 추가해서 WDS를 실행하면 HMR이 적용된다.
- 설정에 devtool: '#sourcemap'을 추가하면 컴파일된 코드에서 원본 코드의 줄번호를 확인할 수 있다.
- WDS를 사용할 때는 publicPath 설정으로 번들 파일의 위치를 지정한다.

<br>

## 13. React 라우팅
- 단방향 데이터 흐름은 React앱에 예측가능성과 유지보수의 편의를 제공한다.
- Flux는 React와 단방향 데이터 흐름을 다룰 때 권장되는 아키텍쳐다.
- Redux는 Flux 아키텍처의 구현체 중 가장 인기가 좋다.
- Redux를 사용하면 액션을 스토어에 전달하거나 속성 객체에 추가할 수 있다.
- Redux의 `connect()`메서드는 스토어의 데이터에 접근할 수 있게 해주고 액션을 스토어에 전달할 수 있으며, 이는 컨테이너 컴포넌트에 필요한 기능이다.
- Redux의 Provider 컴포넌트가 자식 컴포넌트에서 스토어에 접근할 수 있게 해주므로 수동으로 스토어 속성을 전달하지 않아도 된다.
<br>

## 14. Redux를 이용한 데이터 다루기
- 단방향 데이터 흐름은 React앱에 예측가능성과 유지보수의 편의를 제공한다.
- Flux는 React와 단방향 데이터 흐름을 다룰 때 권장되는 아키텍처다.
- Redux는 Flux 아키텍처의 구현체 중 가장 인기가 좋다.

<br>

## 15. GraphQL을 이용한 데이터 다루기
- GraphQL은 프론트엔드에서 데이터를 제공하는 우수하고 믿을 수 있는 방법이다. 또한, 중복된 백엔드 코드도 많이 제거한다.
- React Router에서 브라우저 히스토리를 활성화하고 해시(#)가 없는 URL을 사용하려면 Express라우팅 경로의 * (별표)에서 `sendFile()`을 이용해 `index.html`을 전달하도록 해야한다.
- Express를 데이터 제공자 또는 API뿐만 아니라 정적 자원을 위한 웹서버로 사용하려면 `app.use()`에서 `express.static` 미들웨어를 추가한다.
- GraphQL의 URL구조는 `/q?query=...`이며, 여기서 query는 데이터 쿼리 값이다.

<br>

## 16. Jest를 이용한 React 단위 테스트
- Jest를 설치하려면 `npm i jest-cli --save-dev`를 실행한다.
- 모듈을 테스트할 때 자동 모의 기능을 사용하지 않도록 설정하려면 `jest.dontMock()`을 사용한다.
- `expect.toBe()`를 비롯한 Expect 메서드를 사용할 수 있다.
- TestUtils를 설치하려면 `npm i react-addons-test-utils --save-dev`를 실행한다.
- TestUtils.Simulate.eventName(node)에서 eventName으로 React 이벤트명(on접두사 제외)을 사용하면 DOM이벤트를 시뮬레이션할 수 있다.
- scry...로 시작하는 메서드는 엘리먼트를 여러 개 가져온다.
- find...로 시작하는 메서드는 단일 엘리먼트를 가져온다(엘리먼트가 두 개 이상 있는 경우에는 오류가 발생한다. 정확하게 엘리먼트가 한 개만 있어야한다.)
<br>

## 17. React와 Node.js를 이용한 유니버셜 자바스크립트
- 서버에서 React를 사용하고 렌더링하려면 `react-dom/server`와 `renderToString()`이 필요하다.
- 서버에서 생성한 React HTML과 브라우저 React를 동기화하려면 동일한 데이터를 사용해야한다. React는 체크섬을 사용하여 비교한다.
- `renderToString()`과 `renderToStaticMarkup()`의 차이점은 `renderToString()`에는 브라우저 React가 HTML을 재사용할 수 있도록 체크섬이 포함되어 있고, `renderToStaticMarkup()`에는 체크섬이 포함되어 있지 않다는 점이다.
- 유니버셜 자바스크립트를 구현하기 위해 서버에서 React를 렌더링한 후, 브라우저 React에 동일한 데이터를 제공하여 브라우저 쪽의 React컴포넌트를 렌더링한다.
- Handlebars에서 중괄호 세 개를 사용하여 {{html}}로 입력하면 이스케이프 처리하지 않은 HTML을 출력할 수 있다.
<br>

## 18. 프로젝트: React Router를 이용한 서점 만들기

<br>

## 19. 프로젝트: Jest를 이용한 비밀번호 검사

<br>

## 20. 프로젝트: Jest,Express, MongoDB를 이용한 자동완성 컴포넌트 구현

<br>

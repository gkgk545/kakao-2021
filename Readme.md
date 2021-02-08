# KakaoTalk_Clone

## 카카오톡 클론 만드는 과정에서 공부한 지식을 여기에 적습니다.

<br>

### 1. BEM

- BEM은 html, css 클래스 작명규칙입니다.
- \_\_: 언더바 두 번 / ~의 구조적 일부분
  - _ex. body**container, status-bar**column_
- --: 하이픈 두 번 / ~의 상태
  - _ex. btn--danger, btn--orange_
- -: 하이픈 한 번 / 일반적인 띄어쓰기
  - _ex. toggle-btn, statur-bar_
    <br>
    <br>

### 2. :root, var()

- :root는 전역 CSS 변수 사용 시 유용하게 사용합니다.
- :root로 선언 후 var()로 사용합니다.
  <br> \* CSS var() 함수는 사용자 지정 속성, 또는 "CSS 변수"의 값을 다른 속성의
  <br> 값으로 지정할 때 사용합니다.
  <br>
- 예제
  - :root{
    <br> --main-bg-color: red
    <br>}
    <br> body{
    <br> background-color: var(--main-bg-color)
    <br>}
    <br>
    <br>

### 3. css Component

- css 중 중복되는 클래스는 component에 분류해서 만들고 적용(효율성 증대)
- > 이번 프로젝트에서 중복 사용되는 클래스<br>: profile\_\_img, profile\_\_name, introducing 등

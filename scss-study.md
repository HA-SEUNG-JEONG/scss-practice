### Variable

scss에서 variable을 만드는 방법은 src/scss 폴더에 `_variables.scss` 파일을 생성하는 것이다.

이름은 어떻게 지어도 상관없지만 `_`는 꼭 필요한건데, 이것이 의미하는 것은 css로 변하지 않았으면 하는 것이다.

### Mixin

`_mixins.css`이라는 파일 생성 후에

`@mixin name`으로 작성하고, name은 어떤걸로 지어도 상관없다.

argument를 보낼 수도 있다.

### Extends

같은 코드를 중복하고 싶지 않을 때 사용

page에서 분리해야하는 element들이 많을 때 유용

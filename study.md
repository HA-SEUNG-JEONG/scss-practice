#1.

- div 같은 태그들은 기본적으로 display:block
- inline vs inline-block
  -inline은 box가 아닌 element, 유동적으로 변할 수 있기 때문에 width,height를 특정한 값으로 지정할 수 없고, 특정 값을 지정했을 경우 모든 block 속성을 잃어버린다.
- background와 background-color의 차이
  -background-color는 말 그대로 배경색만 지정할 수 있다.
  -background도 물론 색상 지정이 가능하지만 color 이외의 다른 옵션도 지정해서 사용 가능하다.

#2.

- flexbox에서는 children과 얘기하지 않는다.
- box를 옮기고 싶을 경우 flebox container를 box 바깥에 만든다.

```html
<div class="box">1</div>
<div class="box">2</div>
<div class="box">3</div>
```

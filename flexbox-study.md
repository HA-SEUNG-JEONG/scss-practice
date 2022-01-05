#1.

- div 같은 태그들은 기본적으로 display:block
- inline vs inline-block
  -inline은 box가 아닌 element, 유동적으로 변할 수 있기 때문에 width,height를 특정한 값으로 지정할 수 없고, 특정 값을 지정했을 경우 모든 block 속성을 잃어버린다.
- background와 background-color의 차이
  -background-color는 말 그대로 배경색만 지정할 수 있다.
  -background도 물론 색상 지정이 가능하지만 color 이외의 다른 옵션도 지정해서 사용 가능하다.

#2.

- flexbox에서는 children과 얘기하지 않는다.
- box를 옮기고 싶을 경우 flexbox container를 box 바깥에 만든다.

```html
<div class="box">1</div>
<div class="box">2</div>
<div class="box">3</div>
```

-자식에 붙어있는 부모만이 자식의 위치를 옮길 수 있다.

#3.

- space-around: box 옆 주변 공간을 같게 만든다.
- 기본 방향이 row면 수평 방향이 main-axis , 수직 방향이 cross-axis
- align-items:center는 가운데가 아님, 왜냐하면 wrapper의 높이와 box의 높이가 동일하기 때문

```html
<div class="wrapper">
  <div class="box">1</div>
  <div class="box">2</div>
  <div class="box">3</div>
</div>
```

- align-items:stretch의 경우 자식 요소에 높이가 없을 경우 전체 높이까지 쭉 뻗어서 채워진다.

#4.

- flex-direction: column 👉 main-axis: 수직, cross-axis: 수평
- flex-direction: row (default) 👉 main-axis: 수평, cross-axis: 수직

#5.

- align-self: cross-axis에서 움직이는데 특정한 child에 전달 가능 즉,cross axis 방향에 있는 item의 위치를 바꾼다.

- order: child에게만 줄 수 있는 속성, 기본값은 0 ,HTML에서는 바뀌지 않는다.

- align-self,order는 부모의 높이가 지정되어있어야 적용이 된다.

#6.

- flexbox는 item들이 같은 줄에 있도록 유지하며, width를 신경쓰지 않는다.

- flex-wrap

-기본값은 flex-wrap:nowrap
-wrap은 flexbox에게 child의 width를 유지하라고 이야기하는 것

- align-content

-justify-content와 비슷하지만 line에 대한 것,즉 line(cross-axis)을 변경한다.

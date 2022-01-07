#1.

- flexbox와 마찬가지로 grid로 father에서 일어난다.
- column-gap: column 사이 공간 크기
- row-gap:row 사이 공간 크기
- 더 이상 column 없다면 다음 줄로 넘어간다.

#2.

-grid-area를 이용하여 header,content,nav,footer를 구성한다.
-grid-area에 있는 이름과 grid-template-areas이 같아야 한다.
-grid-area를 지정할 때 string으로 하지 않도록 주의
-grid-template-areas를 4X4로 만들었다고 가정할 때 'auto 200px'는 2번째 grid에만 적용이 되고 나머지는 모두 auto로 적용이 되서 auto 200px auto auto로 된다.
-grid-templates-areas를 적용하지 않은 상태에서 auto 200px는 단순히 row가 2개이고, 첫 번째 grid의 width는 최대로 생기고 두번째 grid width는 200으로 고정

#3.

1)grid-column-start
2)grid-column-end
3)grid-row-start
4)grid-row-end

위 속성은 정수인 숫자가 들어가며 1부터 column(row)의 최대개수+1까지 사용 가능

#4.

-span은 시작점과 끝점을 적는걸 대신한다. 순서대로 몇 칸을 쓰겠다고 선언하는 것

#5.

fr은 높이가 없고, 기본적으로 가능한만큼의 공간을 차지한다. 즉 fr을 쓸 때는 height를 명시해주어야 한다.

repeat은 grid-template에서 적용되지 않는다.

#6.

justify-items, align-items: 부모에게 있는 property

justify-items의 기본값은 `stretch`
justify-content와의 차이점:
grid는 고정 grid 내 아이템만 이동

align-items의 기본값도 `stretch`

위 두가지를 대체할 수 있는 방법으로, `place-items`가 있다.

place-items : 수직 수평

#7.

align-content: 수직으로 grid를 움직임
grid-template에서 높이를 fr로 설정하고 align-content를 stretch로 하면 쭉 늘어난다.

place-content: 수직 수평

justify-content
align-content
place-content

이 3가지는 stretch가 먹히지 않는다. 이럴때는 height를 주고 각 cell에 fr을 쓰면 비슷하게 된다.

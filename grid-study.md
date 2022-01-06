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

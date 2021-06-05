# 카카오톡 클론코딩 Day6
+ 범위: 3.6 ~ 3.11

## 3.6 Paddings and IDs (10:39)
+ padding : box의 경계로부터 안쪽에 있는 공간
  + 경계와 안쪽의 컨텐츠 사이의 공간
+ id는 css에서 `#id`로 취급
  + id는 각각 1개만 있어야 한다.

## 3.7 Border
+ border: 경계면
  + `border: 굵기 종류 크기`
    + 종류는 보통 solid만 씀
  + inline, block 모두 적용됨
+ margin value는 inline에는 높이와 너비가 없으므로 위 아래는 margin을 가지지 못한다.

## 3.8 Classes
| |id|class|
|---|---|---|
|중복여부|하나의 이름만 사용가능|같은 이름의 class를 반복가능|

+ class는 `class = "a b c"`등으로 표현하며
이 때, 태그는 a b c라는 클래스 3개를 갖게된다.

## 3.9 Inline block
+ Inline은 width와 height를 가지면 표현되지 않는다.
  + inline-block은 가질 수 있다.(두가지 특징 모두)
    + 오래되어서 문제 많음 (Responsive design을 지원X -> 화면마다 다르게 표현됨)


## 3.10, 3.11 Flexbox
+ `display: flex;` 로 적용

+ Flexbox사용 규칙
  + 자식 엘리먼트에 아무것도 적지 않는다.
    + css문법을 적지않고 부모 el에 대해 적는다.
+ main axis와(가로) cross axis(세로)라는 축이 있다.
  + justify-content : main axis에 대해 적용
  + align-items : corss axis에 대해 적용
+ 부모가 height, weight가 없다면 바뀌지 않는다

+ `vh` : 단위중 하나로써, 화면의 크기에 따라 배정됨
+ flex-direction: 주축 교차축을 바꿈
+ 자식에 대해서도 flex를 적용할 수는 있다.

+ flexbox는 width,height를 초기값으로만 인식하고 바꾸는데 `flex-wrap : wrap` 을 사용하여 고정값으로 줄 수도 있다.

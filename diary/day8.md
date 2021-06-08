# 카카오톡 클론코딩 Day8
+ 범위: 3.12 ~ 3.16

## 3.12 Fixed, 3.13 Relative Absolute
+ `position`
  + static : 처음 위치에만 있는다.(기본값)
  + fixed : 커서를 움직이더라도 위치가 고정됨
    + top bottom left right중 하나라도 수정하면 고정되지 않은 요소보다 위에 위치함. (다른 레이어에 있다고 표현함)
  + relative: 시작점을 기준으로  top bot lef rig를 -값으로 줘서 이동이 요소 위치 이동이 가능함
  + absolute : 조상중의 relative한 조상을 골라 위치함 (`right: 0px` : 우측끝으로 이동)
    + 부모를 relative로 줘서 원하는 위치로 이동 원할히 함
+ `opacity` : 투명도 설정


**absolute는 자주 쓰이며, relative는 부모로 같이 쓰임**

## 3.14, 3.16 Pseudo Selectors
+ Pseudo SElectors: 다양한 방법으로 SElectors을 선정할 수 있게 해줌
  + tag:last-child : 태그 중 마지막 원소
  + tag:first-child : 태그 중 첫 번째  원소
  + tag:nth-child(n) : n번째 원소
    + even, odd : 홀 짝
    + an +b 꼴로 b번쨰부터 a번째 마다를 표현가능
  + `input required/optional` 에서 iinput:required/optional로 선택 가능

+ attribute selector : attributes를 이용해 선택가능
  + `tag[atrribute="value"] {}` 처럼 사용
    + `~="value"` : value, first value, last value 모두 선택 (띄워쓰기로 구분되야함)





## 3.15 Combinators
+ combinators: selectors간의 관계를 나타내게 해줌
  + `t1 t2 {}` : 조상태그(t1)안에 있는 자식태그(t2) 선택가능
  + `t1 > t2 {}` : 부모태그(t1)바로 밑에있는 자식태그(t2)을 선택함
  + `t1 + t2 {}` : t1 바로 다음에오는 태그 t2들를 선택
  + `t1 ~ t2 {}` : t1 다음에 있는 t2태그들을 선택

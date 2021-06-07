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

#

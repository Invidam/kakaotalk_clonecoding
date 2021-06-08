# 카카오톡 클론코딩 Day9
+ 범위: 3.17 ~ 4.4

## 3.17 States
+ `States`: button과 관련된 selectors
  + `tag:states` 로 사용함
  + `active` : 버튼을 눌렀을 때
  + `hover` : 버튼에 커서를 가져다 댔을 떄
  + `focus` : active에 키보드로 선택하는 경우가 추가됨
  + 위 동작들로 무언가를 바꾸면 border은 초기화 된다.
  + `focus-within`: 자식이 focus되었을 때
  + `form:hover input {}` : form이 hover되면 input에 대해 작동함

## 3.18 Recap
+ 추가적인 pseudo element
  + `tag::placeholder`: placeholder을 꾸밈
  + `tag::selection` : 드래그되었을 때
  + `tag::first-letter` : 첫글자
  + `tag::first-line` : 첫줄

## 3.19 Colors and Variables
### Colors
1. hexadecimal colors (#12e3r3)
2. RGB (rgb(5,1,2))
  + rgba(1,2,3,0.5)
3. name

### Variables(Custom property)
```
:root {
    --main-color:#fdc703;
}
```
: 변수 적을 공간 형성 (root는 docuemnt의 root라는 뜻)

+ 참조: var(--main-color);
+ 색상뿐만이 아니라 attribute value는 모두 저장이 가능하다.
  + attribute와 같게 동작한다.


## 4.0, 4.1 Transitions
+ 상태를 변화시키는 애니메이션
  + state가 아닌 변경 전 일반 태그에 적용시킨다.
  + `transition: 무엇을 얼마동안 ease-in-out`
    + 무엇을 에는 next state에 있는 요소가 들어가야 한다.
    + ex) `transition all 5s ease-in-out;`

+ https://matthewlein.com/tools/ceaser
  + 각 animation 실행 속도 비교
+ Easing : linear, ease-in-out, ease-out, ease-in 등이 있음.
  + easing 뜻 : 시간에 따른 매개변수의 변화율
+ cubiz-bezier : 자신만의 easing 만들 수 잇음.

## 4.2 Transformations
+ `rotateX,Y,Z(n deg)` : n deg만큼 회전
+ `scalex,Y,Z(n)` : n배반큼 키움
+ `translateX,Y,Z(n px)` : n px만큼 이동
  + 다른 sibiling은 이동X (box가 움직이는게 아니라 px차원에서 움직이기 때문

+ **transform + transition과 같이 쓰이면 강력하다.**


## 4.3, 4.4 Animations
```
@keyframes animationName {
  step1 {
    전 동작
  }
  strp2 {
    후 동작
  }
}
```
+ `animation animationName time easing`
  + 마지막에 infinite 추가 -> 무한반복

+ 동작을 3개로 나눠서 (돌리기 전) -> (돌린 후 ) -> (돌리기전으로 되돌아가는 과정) 으로 자연스런 표현 가능

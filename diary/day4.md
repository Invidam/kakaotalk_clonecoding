# 카카오톡 클론코딩 Day4
+ 범위: 2.8 ~ 2.10

## 2.8 Form Tags
+ `<form> </form>`
+ `<input>`
  + `placeholder ` : 무슨 자리인지 표시
  + `type` : text,button 등을 설정 (다른값은 받지 않음)
  + `required` : 입력X -> 제출X
  + `submit` : 제출버튼
  + `file` : 파일 입력
    + `accept ` : 특정 확장자만 가능

## 2.9 More Tags and IDs
```
<label for="abc"> text </label>
<input id="abc" />
```
: 라벨의 text를 누르면 input 태그가 실행된다.

+ ID : unique identify : elment당 1개의 id만 가질 수 있다.
  + 이 규칙을 어기면 작동이 안됨 (오류 검출은 안됨)

## 2.10 Semantic HTML
+ `<div> </div>` : 의미X, 구분 위한 코드
  + `<header></header>`, `<main></main>`, `<footer></footer>`, `<span></span>` : 각각 이름에 맞는 조금의 의미가 추가됨
    + footer : 꼬릿말을 위함
    + span : 짧은 글

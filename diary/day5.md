# 카카오톡 클론코딩 Day5
+ 범위: 3.0 ~ 3.5

## 3.0 How to Add CSS to HTML# 3
+ css를 추가할때에는 html파일에 추가하거나 독자적인 파일에 추가할수도 있다.
  + html파일에 추가 : `<style>` 태그 사용 [inline]
  + 독자적인 파일 추가: `<link rel = stylesheet />` [external]

##3.1 Writing Our First CSS Lines
```
[selector]
{
  [property]
}

```
+ selector : 가리키고자 하는 태그
+ property : 태그에 적용시킬 내용

## 3.2 What Does Cascading Mean
+ CSS : cascading style sheet
+ Cascading: (위에서부터 아래로 차례대로 읽는다는 뜻)
  + CSS, 마지막에 설정한 속정이 최종적으로 적용됨.

## 3.3 Blocks and Inlines

+ Blocks: 옆에 다른 요소가 못옴
  + ex) div, a
  + 높이 너비를 가짐
+ Inlines: 옆에 다른 요소가 올 수 있음
  + ex) span, code
  + 높이 너비가 없고 자기 크기만큼만 가짐

## 3.4, 3.5 Margin Part (1/2, 2/2)
+ `display` : block <-> inline을 변경가능
+ margin : box의 경계와 바깥간의 공간임. (경계밖의 공간)
    + `margin : (위아래 값) (좌우값)` : 편하게 줄 수 있음
    + `margin : ↑ → ↓ ← ` : 시계방향으로 줄 수도 있음.
+ Inspect
  + user agent stylesheet : 브라우저가 기본값을 주었다는 의미

+ collapse margins : elem의 경계가 body이랑 같으면 두 마진은 하나로 취급된다.

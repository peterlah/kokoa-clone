# 1. INTRODUCTION

# 1.3 Software Requirements

1. 구글 크롬 다운로드

2. vscode 다운로드

3. github desktop 다운로드

# 1.6 What is HTML

HTML is for Content.

# 1.7 What is CSS

CSS is for Design.

# 1.8 What is JavaScript

JavaScript is for Interactivity.

# 1.9 Recap

Markup Language

- HTML is for Content.

Style Language

- CSS is for Design.

Programming Language

- JavaScript is for Interactivity.

# 2.1 Setup and Errors

extensions

- Community Material Theme
- Material Icon Theme

# 2.7 More Tagse

- html tag search
  https://developer.mozilla.org/ko/docs/Web/HTML/Element
- 동시 변경 -> 영역 선택 -> ctrl(command) + d

# 2.10 Semantic HTML

- div -> division -> 그냥 박스
- 문서를 보기만해도 그 의미를 짐작할 수 있는 걸 sementic이라고 함
- header, main, footer

# 2.11 Recap

- 속성을 큰따움표로 사용하는것을 권장
- 태그는 검색해서 찾아서 붙여 넣기
- 자주 사용하는 것만 외우기, 모두 외울려고 하지말기.

# 3.0 How to Add CSS to HTML

- <style> 태그 사용하기
- <link> 태그를 사용해서 "style.css" 파일 임포트 하기
    <link href="styles.css" rel="stylesheet">
  ** href -> hypertext reference
  ** rel -> relationship

# 3.2 What Does Cascading Mean

- CSS 는 위에서 아래로 읽기 때문에 가장 하단에 있는 CSS 스타일이 최종적으로 적용됨

# 3.3 Blocks and Inlines

- Blocks - 한줄을 다 차지 : div, p, address 등등
- Inlines - 옆에 다른 요소가 올수 있음 : span, a, img 등등

# 3.4 Margin Part One

![Alt text](image.png)

# 3.5 Margin Part Two

- margin: top right bottom left
  top+bottom right+left
- collapsing margins : Blocks에만 있는 특이한 현상으로 위아래 마진이 중복되는 경우 더 큰값을 가진 쪽으로 병합 되는 현상

# 3.8 Classes

- id는 유니크해야함. 따라서 여러 요소에 동시에 스타일을 적용하고 싶은 경우 클래스를 통해 할당 가능
- id에 css를 적용하는 경우 "#"을 접두사로 사용 클래스를 사용하는 경우 "."을 접두사로 사용

# 3.10 Flexbox Part One

- flexbox를 사용하려면 자식요소에 사용하지 말고 부모 요소에 사용할 것
- justify-content : main-axis / horizantal
- alingn-item : cross-axis / vertical
- vh - viewport height : 스크린 크기를 나타냄 100을 주면 화면의 100%를 의미

# 3.11 Flexbox Part Two

- flex-direction : 컨턴츠를 수평으로 나타낼지, 수직으로 표현할지 결정 - 기본 수평
  - reverse 옵션으로 역순 정렬도 가능

# 3.12 Fixed

- position: fixed; - 화면에 컨텐츠가 고정 됨
- position은 일반적으로 레이아웃 보다는 위치를 아주 조금 움직이고 싶을때 사용
- position fixed를 이용하면 스크롤해도 항상 제자리에 머무른다.
- 처음 만들어진 자리에 고정 되어있다. 하지만 top, left, right, bottom 중 하나만 수정해도 서로 다른 레이어에 위치하게되어 원래 위치가 무시된다.
- positon fixed를 이용하면 가장 위에 위치하게 된다. (맨 앞)

# 3.13 Relative Absolute

- positon: static; (default)
- position: fixed; -> element가 처음 생성된 자리에 고정.
- position: relative; -> element가 '처음 생성된 위치'를 기준점으로, top bottom left right으로 위치를 조금씩 수정할 수 있음

```
position: relative;
top: -10px;
```

- position: absolute; -> 가장 가까운 relative 부모를 기준으로 이동 position:relative; 를 해주면 부모가 됨. 없으면 body가 부모.

# 3.14 Pseudo Selectors part One

- # : id
- . : class
  div:first-child {
  background-color: teal;
  }
  div:last-child {
  background-color: red;
  }
  span:nth-child(5n) {
  background-color: teal;
  } -> even, odd 등

# 3.15 Combinators

- div의 바로 밑 자식에서 span을 찾아서 그것만 효과를 주는 방법

```
// 1
div span {
text-decoration : underline;
}
이렇게하면 div밑에 있는 모든 span이 효과를 가진다
직접적인 부모가 아니어도 밑에있는 것들을 모두 css가 찾는다.

// 2
div > span {
text-decoration : underline;
}
이렇게하면 바로 밑!!! 을 찾게 되므로 바로 밑의 자식만 건들일수있게된다.
```

- 형제에게 효과를 주는방법

```
p + span {
color: black;
}
+ 를 사용하면 형제에게 영향을 끼칠 수 있다. cool
```

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

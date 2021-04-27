![image](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d5/CSS3_logo_and_wordmark.svg/330px-CSS3_logo_and_wordmark.svg.png)
# CSS *(Cascading Style Sheets)*
  - **마크업 언어**가 실제 표시되는 방법을 기술하는 언어
  - **HTML**와 **XHTML**에 주로 쓰이며, **XML**에서도 사용할 수 있다
  - **W3C**의 표준이며, 레이아웃과 스타일을 정의할 때의 자유도가 높다

## 기본 문법 예시

```css
p {
    font-size: 110%;
    font-family: garamond, sans-serif;
}
h2 {
    color: red;
    background: white;
}
.highlight {
    color: red;
    background: yellow;
    font-weight: bold;
}
#test_id {
    color: blue;
    background: white;
}
```


## - Selecter(선택자)
    스타일을 적용하고자 하는 HTML 요소를 선택하기 위해 CSS에서 제공하는 수단
![image](https://poiemaweb.com/img/css-syntax.png)

## - Property(속성)
    셀렉터로 HTML 요소를 선택하고 {} 내에 프로퍼티(속성)와 값을 지정하는 것으로 다양한 style을 정의할 수 있다.
    프로퍼티는 표준 스펙으로 이미 지정되어 있는 것을 사용하여야하며 사용자가 임의로 정의할 수 없다.
    여러 개의 프로퍼티를 연속해서 지정할 수 있으며 세미콜론(;)으로 구분

## - value(값)
    프로퍼티의 값은 해당 프로퍼티에 사용할 수 있는 값을 “키워드”나 “크기 단위” 또는 “색상 표현 단위” 등의 특정 단위로 지정하여야 한다.
    
----------------------------------------------------------------------------------------------

# HTML과 CSS의 연동

- Link style : HTML에서 외부에 있는 CSS 파일을 로드하는 방식이다. **가장 일반적으로 사용**
```html
[HTML]
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" href="css/style.css">
  </head>
  <body>
    <h1>Hello World</h1>
    <p>This is a web page.</p>
  </body>
</html>
```
```css
[CSS]
h1 { color: red; }
p  { background: blue; }
```
- Embedding style : HTML 내부에 CSS를 포함시키는 방식
```html
[예시]
<!DOCTYPE html>
<html>
  <head>
    <style>
      h1 { color: red; }
      p  { background: aqua; }
    </style>
  </head>
  <body>
    <h1>Hello World</h1>
    <p>This is a web page.</p>
  </body>
</html>
```
- Inline style : HTML요소의 style 프로퍼티에 CSS를 기술하는 방식
```html
[예시]
<!DOCTYPE html>
<html>
  <body>
    <h1 style="color: red">Hello World</h1>
    <p style="background: aqua">This is a web page.</p>
  </body>
</html>
```

![image](https://upload.wikimedia.org/wikipedia/commons/thumb/6/61/HTML5_logo_and_wordmark.svg/180px-HTML5_logo_and_wordmark.svg.png)
# HTML *(HyperText Markup Language)*
  - 웹페이지를 기술하기 위한 **마크업 언어**
  - 웹페이지의 **내용(CONTENT)**, **구조(STRUCTURE)** 를 담당하는 언어
--------------------------------------------------------------------

### 기본 구조 예시
```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <title>페이지 제목</title>
</head>
<body>
    <h1>글머리</h1>
    <p>문단</p>
</body>
</html>
```
--------------------------------------------------------------------
### 기본 문법 예시
![image](https://poiemaweb.com/img/tag.png)
- 요소(Element) : 시작 태그와 종료태그 그리고 그 태그 사이에 위치한 content로 구성
- 요소는 다른 요소 포함할 수 있다! (중첩 가능 -> 중첩된 요소는 시각적으로 파악하기 쉽게 들여쓰기를 활용해서 쓰는 것이 좋다)
- 빈요소(Empty Element) : content는 가질 수 없는(필요가 없는) 요소이며 Attribute만을 가질 수 있다.
- 빈요소 예시 :
    - br
    - hr
    - img
    - input
    - link
    - meta
![image](https://poiemaweb.com/img/html-attribute.png)
- 속성(Attribute): 요소의 성질, 특징을 정의하는 명세이다.<br> Element는 Attribute를 가질 수 있으며
  Attribute는 요소에 추가적 정보(ex.이미지 파일 경로, 크기 등)를 제공한다.<br> Attribute는 시작 태그에 위치해야 하며
  이름과 값의 쌍을 이룬다.

##### 주석
- 주석(Comment) : 주로 개발자에게 코드를 설명하기 위해 사용되며 브라우저는 주석을 화면에 표시하지 않는다.
```html
<!-- 주석은 화면에 표시되지 않음 -->
```

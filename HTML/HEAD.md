# HEAD

```html
<meta>
   - 헤더 내부에서 사용하는 태그
   - html문서가 가지고 있는 유용한 정보를 담아두는 곳
   - (문서 정보를 검색 엔진에 전달)
   
    [예시]
      <meta name="attribute-name(속성명)" content="attribute-value(속성내용)">
```

```html
<title></title>
    페이지 제목을 나타내는 태그

    [예시]
      <title>페이지 이름</title>
```

```html
<link>
    문서를 외부의 문서와 연결하기 위해 사용
    CSS파일이나 웹 폰트 사용 시 주로 연결

    [예시]
      <link rel="관련 속성" type="MIME" href="문서위치">
```
|속성||
|---|---|
|href|연결한 파일의 경로 지정|
|rel|링크가 형성하는 관계 지정|
|media|연결문서가 표시될 장치 또는 미디어 유형|
|type|MIME 타입 지정|

```html
<style></style>
    태그의 스타일을 지정해주는 태그로
    CSS속성을 HTML내에 직접 쓸 때 사용

    [예시]
      <style>CSS구문</style>
```

```html
<base>
    페이지의 링크가 상대 경로로 되었을 때 그 기준이 될 경로 지정
    링크를 어떻게 오픈할 것인지 결정

    [예시]
      <base href="경로" [target="키워드"]>
```
|target 키워드||
|---|---|
|_self|그 위치에서 열기|
|_parent|링크의 바로 상위페이지에서 열기|
|_top|최상위 페이지에서 열기|
|_blank|새창으로 열기|

# window객체와 BOM

## BOM(Browser Object Model)

![image](https://ko.javascript.info/article/browser-environment/windowObjects.svg)

### screen 객체
`client 운영체제 화면에 대한 속성 값을 가지는 객체`

- 속성

|속성|내용|
|---|---|
|height|화면 높이|
|width|화면 너비|
|availWidth|실제 화면에서 사용 가능한 너비|
|availHeight|실제 화면에서 사용 가능한 높이|
|colorDepth|사용 가능한 색상수|
|pixelDepth|한 픽셀 당 비트 수|

### location 객체

```
브라우저의 주소 표시줄(URL)과 관련된 객체로
프로토콜 종류, 호스트 이름, 문서 위치 등의 정보를 가짐
```

- 속성

|속성|내용|
|---|---|
|hash|앵커 이름(#~)|
|host|호스트 이름과 포트번호|
|hostname|호스트 이름|
|href|문서 URL주소|
|origin|호스트이름, 프로토콜, 포트번호|
|pathname|디렉토리 경로|
|port|포트번호|
|protocol|프로토콜의 종류|
|search|요청 매개변수(?~~)|

- 메소드

|메소드|내용|
|---|---|
|assign('주소')|새로운 페이지 로드 (*뒤로 가기 가능)|
|reload()|현재 문서를 다시 로드|
|replace('주소')|현재페이지를 새 페이지로 교체 (*뒤로 가기 불가)|

### navigator 객체

`브라우저에 대한 정보를 가지는 객체`

- 속성

|속성|내용|
|---|---|
|appCodeName|브라우저 코드명|
|appName|브라우저 이름|
|appVersion|브라우저 버전|
|platform|사용중인 운영체제|
|useAgent|브라우저 전체정보|
|cookieEnabled|쿠키가능성을 확인(true/false)|
|geolocation|위도와 경도를 출력|
|language|브라우저 언어|
|online|브라우저가 온라인/오프라인 환경인지 확인(true/false)|
|product|브라우저 엔진이름|

------------------------------------------------------------------------------------------------------------------------------------------

## window 객체

```javascript
브라우저 창에 대한 설정을 하는 객체로 자바스크립트에서의 최상위 객체
생성되는 모드 객체는 window객체 하위에 존재

  [예시]
    window.open('주소', '이름 또는 open방식', '형태');
```

- 형태옵션

![image](https://img1.daumcdn.net/thumb/R800x0/?scode=mtistory2&fname=https%3A%2F%2Ft1.daumcdn.net%2Fcfile%2Ftistory%2F996ABA345F57CA7902)

### window 객체 메소드

|메소드|내용|
|---|---|
|moveBy(x,y)|윈도우 위치조정(상대)|
|moveTo(x,y)|윈도우 위치조정(절대)|
|resizeBy(x,y)|윈도우 크기조정(상대)|
|resizeTo(x,y)|윈도우 크기조정(절대)|
|scrollBy(x,y)|스크롤 위치이동(상대)|
|scrollTo(x,y)|스크롤 위치이동(절대)|
|focus()|윈도우에 초점 맞춤|
|blur()|윈도우에 초점 제거|
|close()|윈도우 닫기|
|setTimeout(함수, 시간(ms))|일정시간 후 함수를 한번 실행 / id값 리턴|
|setInterval(함수, 시간(ms))|일정시간마다 함수를 반복 실행 / id값 리턴|
|clearTimeout(id)|setTimeout() 함수 실행 종료|
|clearInterval(id)|setInterval() 함수 종료|

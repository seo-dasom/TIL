![image](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=http%3A%2F%2Fcfile10.uf.tistory.com%2Fimage%2F2149683A58CA6BF31324DD)
# JavaScript
  - 웹 브라우저에서 동작하는 유일한 프로그래밍 언어
  - **인터프리터 언어(Interpreter language)**
  - 명령형(imperative), 함수형(functional), **프로토타입 기반(prototype-based) 객체지향 프로그래밍**을 지원하는 **멀티 패러다임 프로그래밍 언어**
-----------------------------------------------------------------------------------------------------------------------------------------------

### 기본 문법

##### 1. 변수

```javascript
값(value)을 저장(할당)하고 그 저장된 값을 참조하기 위해 사용한다.
한번 쓰고 버리는 값이 아닌 유지(캐싱)할 필요가 있는 값은 변수에 담아 사용한다.
또한 변수 이름을 통해 값의 의미를 명확히 할 수 있어 코드의 가독성이 좋아진다.
메모리 주소(Memory address)에 접근하기 위해 사람이 이해할 수 있는 언어로 지정한 식별자(identifier)이다.

var x;  // 변수의 선언
x = 6;  // 정수값의 할당
```

##### 2. 값

|용어|의미|
|---|---|
|데이터 타입(Data Type)|프로그래밍 언어에서 사용할 수 있는 값의 종류|
|변수(Variable)|값이 저장된 메모리 공간의 주소를 가리키는 식별자(identifier)|
|리터럴(literal)|소스코드 안에서 직접 만들어 낸 상수 값 자체를 말하며 값을 구성하는 최소 단위|

```javascript
프로그램에 의해 조작될 수 있는 대상을 말한다.
값은 다양한 방법으로 생성할 수 있다. 가장 간단한 방법은 리터럴 표기법(literal notation)을 사용하는 것이다.

모든 값은 데이터 타입을 갖는다.

  * 원시 타입(primitive data type)
    - number
    - string
    - boolean
    - null
    - undefined
    - symbol(New in ECMAScript6)
  * 객체 타입(Object data type)
    - object

변수에 할당된 값의 타입에 의해 동적으로 변수의 타입이 결정된다.
이를 동적 타이핑이라 하며 자바스크립트가 다른 프로그래밍 언어와 구별되는 특징 중 하나이다.
```

##### 3. 연산자

```javascript
하나 이상의 표현식을 대상으로 산술, 할당, 비교, 논리, 타입 연산 등을 수행해 하나의 값을 만든다. 이때 연산의 대상을 피연산자(Operand)라 한다.

  - 산술 연산자
  - 문자열 연결 연산자
  - 할당 연산자
  - 비교 연산자
  - 논리 연산자
  - 타입 연산자
  - 인스턴스 생성 연산자
  
피연산자의 타입은 반드시 일치할 필요는 없다. 이때 자바스크립트는 암묵적 타입 강제 변환을 통해 연산을 수행한다.
```

##### 4. 키워드

```javascript
키워드(keyword)는 수행할 동작을 규정한 것이다.

  // 변수의 선언
  var x = 5 + 6;
  
  // 함수의 선언
  function foo(arg) {
    // 함수 종료 및 값의 반환
    return ++arg;
  }
  
  var i = 0;
  // 반복문
  while (1) {
    if(i > 5) {
      // 반복문 탈출
      break;
    }
    console.log(i);
    i++;
  }
```

##### 5. 주석

```javascript
주석(Comment)은 작성된 코드이 의미를 설명하기 위해 사용한다.
(코드는 이해하기 쉽고 가독성이 좋아야 한다. 설명이 필요한 부분에 주석을 달아주는 것.. 과도한 주석은 오히려 방해!)

한줄 주석은 // 다음에 작성하며 여러줄 주석은 /* 과 */ 의 사이에 작성한다.
```

##### 6. 표현식

```javascript
표현식(Expression)은 하나의 값으로 평가(Evaluation)된다.
값(리터럴), 변수, 객체의 프로퍼티, 배열의 요소, 함수 호출, 메소드 호출, 피연산자와 연산자의 조합은 모두 표현식이며 하나의 값으로 평가(Evaluation)된다.
```

##### 7. 함수

```javascript
함수란 어떤 작업을 수행하기 위해 필요한 문(statement)들의 집합을 정의한 코드 블록이다.
이름과 매개변수를 갖으며 필요한 때에 호출하여 코드 블록에 담긴 문들을 일괄적으로 실행할 수 있다. 함수는 호출에 의해 실행되는데 한번만 호출할 수 있는 것이 아니라 여러번 호출할 수 있다.
```

##### 8. 객체

```javascript
자바스크립트는 객체(object) 기반의 스크립트 언어이며, 원시 타입(Primitives)을 제외한 나머지 값들(함수, 배열, 정규 표현식 등)은 모두 객체이다.
자바스크립트 객체는 키(이름)와 값으로 구성된 프로퍼티(property)의 집합이다.
프로퍼티의 값으로 자바 스크립트에서 사용할 수 있는 모든 값을 사용할 수 있다. 따라서 프로퍼티 값으로 함수를 사용할 수도 있으며 프로퍼티 값이 함수일 경우, 일반 함수와 구분하기 위해 메소드라 부른다.
객체지향의 상속을 구현하기 위해 "프로토타입"이라고 불리는 객체의 프로퍼티와 메소드를 상속받을 수 있다.
```

##### 9. 배열

```javascript
배열(array)은 1개의 변수에 여러 개의 값을 순차적으로 저장할 때 사용한다.
자바스크립트의 배열은 객체이며 유용한 내장 메소드를 포함하고 있다.
```

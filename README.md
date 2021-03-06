# Coding_Study
Coding Study with 2019 SDS Developers

## 2021/02/20

[장원용 스터디] <br/>
https://wonyong-jang.github.io/java/2021/01/04/Java-Interface.html <br/>
https://wonyong-jang.github.io/java/2020/11/08/Java-JVM.html <br/>

.class 를 Class Loader 가 JVM 메모리에 적재 <br/>
Execution Engine 이 실행 <br/>
javac 를 통해 컴파일 java 로 실행 <br/>
상위버전으로 컴파일후 낮은 버전으로 실행 시 에러 <br/>
javac -source 옵션으로 특정버전으로 컴파일 할 수 있음 <br/>
인텔리제이 shift 두번 바이트코드로 까볼수있음 <br/>
javap -c 로 바이트코드 볼수있음 <br/>
자바 8 부터 default static 메소드 추가 <br/>
인터페이스에서는 static final , abstract 을 명시하지 않으면 자동으로 붙여서 컴파일한다. <br/>
interface 도 상속을 받을 수 있다, 메소드 명이 같고 리턴타입이 다르면 에러가 난다. <br/>
default 메소드를 사용하면 구현하고 싶은 클래스에만 구현하면 되어서 하위 호환성을 유지할 수 있다. <br/>
인터페이스에서 static 은 오버라이딩 불가 <br/>
인터페이스 private 메소드도 캡슐화를 위해 나왔는데, private static 도 사용할 수 있다. <br/>
함수형 인터페이스의 경우 @FunctionalInterface 어노테이션을 붙여서 구현한다. <br/>
Constant Interface 상수만 리스트로해서 만드는 것은 안티패턴 <br/>

[송명진 스터디]
https://github.com/RumbleKAT/ReactStudy

Mosaic 브라우저가 브라우저의 시작 <br/>
동적인 웹브라우저를 만들기위해 스크립팅 언어를 만듦 <br/>
만들어진 동적인 언어 : Java Scheme 라는 언어 <br/>
LiveScript 가 JavaScript 로 명명이 됨 ( Java 를 그때 많이 쓴다고해서 ) <br/>
인터프리터 언어는 기계어가 아니라 소스코드를 바로바로 실행하는 방식, 중간에 잘못된게 있으면 에러를 그때그때 뱉는 방식이어서 컴파일러보다 더 빠르고 컴파일 단계가 필요없음 <br/>
넷스케이프에서 1995 부터 익스플로러를 많이 쓰게 되었는데, 브라우저에서는 버전에 따라 호환성이 달라서 해당을 살펴볼 필요가 있음 <br/>
Polyfill 은 크로스 브라우징을 지원하는 라이브러리이다. <br/>
Jscript 는 익스플로러사에서 쓰는 엔진이다. <br/>
학술단체에서 JS의 통합과 정리를 하고자 ECMAScript1 을 1997년에 정의함. <br/>
2000년 까지 인터넷 익스플로러가 대세이다가 2004년에 Firefox 가 ActionScript를 만들어서 출시했으나 모든 브라우저의 표준을 맞추지는 못함 <br/>
2015년 2014년까지 넷스케이프, 인터넷 익스플로러, Firefox 가 대세이다가 2004년에 AJAX가 만들어짐. <br/>
AJAX 는 웹페이지의 속도가 상승되고 비동기 처리가 가능하며 서버에서 데이터만 제공하면 되므로 전체적인 코드량이 줄어든다. <br/>
파싱으로 인한 화면 깜빡임이 있었는데 AJAX 로 인해 유저 경험이 상승되었다. <br/>
하지만 히스토리 관리가 안되고 연속 데이터 요청 시 서버부하 증가 등 단점이 있었다. <br/>
이후에 JQuery 가 생겼다. <br/>
2015년에 생긴 ECMAScript6 는 6년 밖에 안됐으며 클래스, 람다 등을 제공하게 되었다. <br/>
TypeScript 는 일종의 JavaScript 버전에 따라서 버전호환을 지원하는 스크립트이다. <br/>
TypeScript 는 타입을 붙여주는데, JavaScript 의 경우 Object 자료형이 많아서 타입변환 시 발생하는 Side effect 를 TypeScript 에서는 보완할 수 있다. <br/>
Babel 은 JavaScript 컴파일러인데, 브라우저 호환성을 맞춰줄 수 있는 컴파일러이다. <br/>
크롬은 C++ 기반 V8 Javascript 엔진을 쓴다. <br/>
create-react-app 을 사용해서 리액트 프로젝트를 자동으로 만들어줄 수 있다. <br/>
크롬 데브툴즈에서 리액트 프로젝트가 생겼는지 확인하는 플러그인이 있는데 각 엘리먼트들이 호출되는 시간, 성능을 검사할 수 있다. <br/>
SPA ( Single Page Application ) : App.js 랑 앱테스트소스, 렌더링하는 ReactDOM, index 가 있는데 리액트는 js로 렌더링하여 구성한다. <br/>
SPA 에는 React, Angular, Vue 등이 있는데 클라이언트 사이드 렌더링하여 반응이 빠르다. <br/>
Next.js 는 리액트를 Server Side Rendering 으로 사용하기 위해 만들어졌다. 이를 사용하여 자바스크립트로 추가된 엘리먼트를 뿌려줄 수 있다. <br/>
Gatsby 라이브러리는 서버 사이드 렌더링을 지원하는 라이브러리이다. <br/>
Nuxt.js 는 뷰에서 서버 사이드 렌더링을 제공해주는 라이브러리이다. <br/>
Call Stack : 자바스크립트는 1개의 동시성을 다루는, 즉 단일 콜스택을 갖는다. <br/>
자바스크립트에서는 함수 호출이 스택형태로 쌓인 뒤, 상단부터 하나씩 리턴하는 방식으로 실행된다. <br/>
자바스크립트 엔진이 구동되면서 변수, 함수같은 정보가 메모리 힙에 저장되며 바라보는 곳이 없을 경우 프리시킨다. <br/>
비동기 함수는 큐에 저장되며 콜스택이 모두 실행된 후에 이벤트 큐가 실행된다. <br/>
동시성 모델에서 자바스크립트는 Non blocking 언어여서 비동기로 처리할 수 있으면 동시성을 최대한 높일 수 있게 작동한다. <br/>
콜스택 CPU 바운드 쪽 작업을 한 후, 이벤트 큐 DB 바운드 등의 응답을 받아서 콜스택이 작동한다. <br/>
스프링의 경우, DB 에서 값을 불러오는 동안 블로킹된다. <br/>
async & await : Premise 의 업그레이드 버전으로 블로킹으로 작동할 수 있도록 해준다. <br/>
리액트 JSX : Javascript + XML 로 이루어진 자체적인 언어 <br/>
웹 브라우저에서 HTML 문서 렌더링 과정은 불러오기, 파싱, 렌더링 트리 만들기, CSS 결정, 레이아웃, 그리기 순서로 작동한다. <br/>
인덱스 트리에서 트리의 값이 바뀌면 자식 트리에 영향이 발생하는데, 리액트는 가상돔을 사용하여 자식 트리에 영향을 주지 않고 해당 변화점에만 연산이 생긴다. <br/>
자바스크립트에서는 === 까지 해야 자료형까지 비교하고 == 를 하면 값만 비교한다. <br/>
리액트 돔에서는 리액트 돔으로 한번 더 감싸서 XSS 공격을 방어할 수 있다. <br/>
리액트 돔 상에서는 엘리먼트끼리 깊은 비교가 아닌 얕은 비교를 하여 자식 트리와 비교를 하여 변화가 생겼는지 아닌지를 판단하여 연산이 빠르다. <br/>
리액트 라이프사이클 : 리액트 17 부터는 componentWillMount, componentWillUpdate, componentWillReceiveProps 라이프사이클이 deprecated 된다. <br/>
리액트 클래스 컴포넌트 : 헤더 컴포넌트를 만들때 컴포넌트를 상속받아 렌더 함수에서 태그를 리턴하는 방식이다. <br/>
최근 업무로 사용되는 Function 형태는 리액트 훅을 사용한다. <br/>
리액트 훅 : 예를 들어 변화를 주는 변수를 넣어서 새로운 상태 값을 정의하고 사용할 함수를 넣어서 표현한다. <br/>
원래같으면 클래스 컴포넌트 안에 Function 을 선언하고 setState 를 써서 코드가 길었는데, 함수형 리액트 훅을 사용하면 간결하게 표현이 가능하다. <br/>
이펙트 훅 : componentDidMount, componentDidUpdate 도 써야하는 것을 유즈 이펙트만 써서 컴포넌트를 가볍게 만들었다. <br/>
리듀서 : JS 기본 Function 중 배열에 있는 전체 값을 더해 새로운 value 로 리턴함. <br/>
리액트에서 리듀서는 이벤트 상태값과 액션들을 모아서, 액션의 타입 케이스 별로 상태 값을 리턴해준다. <br/>
리듀서를 사용할 것이라고 정의를 해놓으면 리듀서 안에서 상태 값을 바꿔서 전달을 해준다. <br/>
리듀서를 최근에 사용하는 이유는, 부모에서 자식으로 내려가는 데이터의 흐름 뿐만 아니라 자식에서 발생한 변화를 부모에게도 흘려주는 일괄적 관리를 위해 사용한다. <br/>
Redux 와 같은 역할이다. <br/>
리듀서는 Store 안에 있는 변수를 관리한다. <br/>
발행-구독 모델 : 카스카 등 비동기 메시징 패러다임이다. 구독을 누르고 나면 구독자에게 알림 메시지가 가는 것처럼 리듀스는 컴포넌트가 구독을 누르면 값이 변화했을때 구독자들에게 변화값을 전달해주는 것이다. <br/>
Redux-thunk : 디스패치 액션이 일어나고 끝났을 때 스토어에게 전달하는 비동기 과정을 도와줄 때 redux-thunk 를 사용한다 <br/>
Redux-saga : 미들웨어에서 API 를 호출하고 비동기의 후처리 등 부가적인 기능들을 제공한다. <br/>
React-Redux : 리액트에서 만들지는 않았지만 대중적으로 사용되는 라이브러리이다. <br/>
createStore : Store 를 만들어준다, createStore(reducer) 와 같은 형태로 구독을 만들어준다. <br/>
리액트에서 Provider 라는 객체를 만드는데 App 을 상속하는 자식 컴포넌트들도 Store 에 접근하여 이를 상속한 자식끼리 서로의 상태값에 접근할 수 있다. <br/>
userReducer : 리액트 17버전 정도 부터 리액트 내부적으로 지원해주는 기능이다. <br/>
create-react : Velopert gitbook > 벨로퍼트와 함께하는 모던 리액트 참고 <br/>

https://react.vlpt.us/
 <br/>
cf) Generator 문법, 유투브 라이브 강의 등 <br/>

## 2021/03/07

[김성민 스터디] https://www.notion.so/Effective-Java-3-E-6e8c1a05ab4c4ee08ccc6096ed919608
1. 생성자 대신 정적 팩터리 메서드를 고려하라

### 핵심 정리

정적 팩터리 메서드와 public 생성자는 각자의 쓰임새가 있으니 상대적인 장단점을 이해하고 사용하는 것이 좋다.
단, 정적 팩터리 메서드가 유리한 경우가 더 많으므로 무작정 public 생성자를 제공하던 습관을 고치자.

2. 생성자에 매개변수가 많다면 빌더를 고려하라

### 핵심 정리

- 생성자나 정적 팩터리가 처리해야 할 매개변수가 많다면 빌더 패턴을 선택하는 게 더 낫다.
- 매개변수 중 다수가 필수가 아니거나 같은 타입이면 특히 더 그렇다.
- 점층적 생성자보다 코드를 읽고 쓰기가 훨씬 간결하고, 자바빈즈보다 훨씬 안전하다.

3. private 생성자나 열거 타입으로 싱글턴임을 보증하라

### public static 멤버가 final 필드인 방식

private 생성자는 Cat.INSTANCE를 초기화할때 딱 한 번만 호출된다.

public이나 protected 생성자가 없으므로 Cat 클래스가 초기화될 때 만들어진 인스턴스가 전체 시스템에서 단 하나뿐임이 보장.

```java
public class Cat {
		public static final Cat INSTANCE = new Cat();
		private Cat(){}
}
```

AccessibleObject.setAccessible을 사용하면? → 생성자에서 예외를 처리한다.

```java
private Cat() {
    if(this.INSTANCE != null) {
        throw new RuntimeException("이미 생성된 싱글톤 객체가 존재합니다.");
    }
}
```

### 장점

- public static 필드가 final이니 절대로 다른 객체를 참조할 수 없다. * 명백하게 API에 싱글턴임이 드러난다.
- 간결하다.

### 정적 팩터리 방식

```java
public class Cat2 {
    public static final Cat2 INSTANCE = new Cat2();

    private Cat2() {}

    public static Cat2 getInstance() {
        return INSTANCE;
    }

    public String getName() {
        return "Bada2";
    }
}
```

Cat2.getInstance()는 항상 같은 객체의 참조를 반환하므로 제2의 Cat2 인스턴스란 결코 만들어지지 않는다.

(Reflection에 대한 예외는 똑같이 발생)

### 장점

- API를 바꾸지 않고도 싱글턴이 아니게 변경할 수 있다. (호출하는 스레드별로 다른 인스턴스를 넘겨주게 할 수 있다.)
- 정적 팩터리를 제네릭 싱글턴 팩터리로 만들 수 있다.
- 정적팩터리 메소드 참조를 공급자(supplier)로 사용할 수 있다.

```java
Supplier<Cat2> cat2Supplier = Cat2::getInstance;
```

두 방식 모두 직렬화시 인스턴스 필드를 transient로 선언하고 readResolve 메소드를 제공해야 한다.

### 원소가 하나뿐인 열거 타입 방식

```java
public enum Cat3 {
    INSATANCE;

    public String getName() {
        return "Bada3";
    }
}
```

장점이 강력하여 해당방법의 싱글턴을 만드는 게 가장 좋은 방법이다.

단, 만들려는 싱글턴이 Enum 외의 클래스를 상속해야 한다면 사용 불가능.

### 장점

- public 필드 방식과 비슷하지만, 더 간결하고 추가 노력없이 직렬화 가능
- 아주 복잡한 직렬화 상황이나 리플렉션 공격에도 제2의 인스턴스가 생기는 일을 완벽히 막아줌

## 2021/04/03,04
[이경진 스터디] 참고) Selenium Study & SQLP Study

[김성민 스터디]
https://www.notion.so/Effective-Java-3-E-6e8c1a05ab4c4ee08ccc6096ed919608


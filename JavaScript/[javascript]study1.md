# JavaScript Study1

## 자바스크립트?
- 웹페이지를 동적으로 or 프로그래밍 적으로 제어하기 위해 고안된 언어
- 웹 브라우저에서 유일하게 사용가능한 프로그래밍 언어

##### 자바스크립트를 굳이굳이 공부해야 하는 이유
- 사용자와 상호작용하는 웹 페이지를 만들기 위해
  - html로 웹 페이지 틀을 잡고 -> css로 꾸미고 -> js로 상호작용 가능!!
- ~~평화로운 졸작을 위하여...ㅋㅋㅋㅋㅋㅋㅋ~~
### Event(이벤트)?
- 웹브라우저 위에서 일어나는 모든 사건들.
- 자바스크립트가 사용자와 상호작용 하는데 핵심 적인 역할을 함.
- 이벤트의 속성값은 웹 브라우저가 기억하고 있다가 해당 이벤트가 실행될때 자바스크립트의 문법을 해석하여 동작함
- 종류는 겁나 다양함
  - onclick, onchange,onkeydown ... 외 on 으로 시작하는 속성들
~~~
<input type ="button" value="hi" onclick="alert(hi)">

onclick 의 속성값으로는 반드시 자바스크립트가 와야함
~~~  
### Data type
Boolean,Null,undefined,Number,String,Symbol + object
~~일단은 Number,String,Boolean 정도만 알면 다행..~~

### 변수 선언
~~~
var 변수이름 ;   // var를 쓰는 장,단점이 존재하지만 일단 쓰셈 안써도 되긴 하지만 걍 쓰셈
~~~
### 조건문
이건 걍 일반 프로그래밍 언어와 걍 같은 개념이기 때문에 배웠다 정도로 하고 넘어가겠음.

### 리펙토링 ,중복의 제거
- 비효울적인 코드들의 효율성을 높이고 중복을 제거하는 과정
  - this 이용
  - 변수를 선언하여 공통적인 코드를 제거하고 가독성을 높힘
### 오늘 자바스크립트를 공부하게 되면서 알게 된 것들
1. **element=tag**
~~element랑 tag가 뭔 줄 알았는데 이 두개가 같다는건 몰랐음 ㄹㅇ 모순 오지는 부분...ㅋㅋㅋㅋㅋㅋ~~

2. '...'부분이 자바스크립트 코드임을 웹 브라우저가 알 수 있게 해줌 .
~~~
<script>...</script>
 ~~~

 3. js를 이용하여 웹 페이지에 글씨 출력하려면?
 ~~~
 document.wirte('hello world');  //아주 기본적
 ~~~

4. 자바스크립트는 비교연산자가 '===' 임
5. document.querySelector(selectors);

### 참고
[생활코딩](https://opentutorials.org/course/3085)

#### 느낀점

제대로 공부하고 있는가 하는 의심이 든다. 얼른 지긋지긋한 개념공부를 끝내고 계산기를 만들어 보고싶다.
그리고 계산기 까지 성공한다면 꼭 실패했던 로또 프로그램도 만들고 싶다.
그리고 자바스크립트를 공부함과 별개로 가장 크게 느낀건 마크다운이거 진짜 짜증난다 이쁘게 하고 싶은데
나중에 좀 더 알아봐야겄다 열받음

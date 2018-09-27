#자바스크립트 두번째 공부...
~~자바시간에 배운거 내가 몰랐던 것이나 처음 알게 된 사실만 정리한 것.~~
## 1. 자바스크립트 코드의 위치

~~~ javascript
- HTML 태그의 이벤트 리스너 속성
- <script> </script> 태그에 작성
- 자바스크립트 file에 작성
 (<script>태그 없이 js코드만 저장)
- URL 부분에 작성
~~~

## 2. 식별자

- 자바스크립트 프로그램의 변수,상수(리터럴),함수의 이름
- 식별자 작성 규칙
   - 첫 번째 문자 : 알파벳, 언더바, $ 문자만 사용 가능
   - 두번째 이상 문자: 알파벳,언더바,0~9, $사용 가능
   - 대소문자 구분함
   - js예약어 사용 불가

## 3. 자바스크립트 문장
 - 문장과 문장을 구분하기 위해 세미콜론( ; ) 사용
 - 주석문
 ~~~
 // 한 라인의 주석 --> 라인의 끝까지 주석 처리 함
 /*
  여러 라인의 주석
  */
 ~~~
~~자바스크립트에는 문자타입 없음 모두 문자열 오 ..ㅋㅋ~~

## 4. 변수 : 자바스크립트 데이터 저장 공간

- 변수 선언 var,const,let 이용 (~~const,let은 최신문법 웹으로 진로 결정하면 최신문법도 알아야함~~)
- 자바스크립트에는 변수의 타입이 없엉
  - 변수 타입 선언 하지 않음 (var num ㅇㅇ int num ㄴㄴ)
  - 변수에 저장되는 값에 대한 재약 없음 (실수,문자열 다 저장 가능)

### 4-1. 지역변수와 전역변수

**지역 변수**
 - 함수 내에 var 키워드로 선언
 - 선언된 함수 내에서만 사용 가능

 **전역 변수**
  - 함수 밖에서 선언되거나 함수 내에 var 키워드 없이 선언된 변수
  - 프로그램 전역에서 사용  

  > *지역변수와 전역변수의 이름이 같으면 어떻게 구분하지?*
   this를 이용하여 전역변수에 접근하자 ===> this.전역변수

   ~~~ javascript
<script>
var x=100; // 전역변수

function a(){
  var x=1; // 지역 변수
  document.write(this.x) // 전역변수를 호출
}
</script>
   ~~~

## 함수
- 목적을 가지고 작성된 코드 블록
- 데이터 전달받아 처리한 후 결과를 돌려주는 코드 블록

#### 함수의 구성

~~~ js
function 함수이름(arg1,arg2...){
  ...my code...
  return result;
}
~~~

#### 함수의 호출
~~~ js
var n = 함수이름(arg1,arg2...);
~~~

###### 자바스크립트에서 제공하는 전역 함수

- eval(exp) -> exp의 자바스크립트 식을 계산하고 결과 리턴
- parseInt(str) -> str 문자열을 10진 정수로 변환하여 리턴
- parseInt(str,radix) -> str 문자열을 radix 진수로 해석하고, 10진 정수로 바꾸어 리턴
- paseFloat(str) -> str 문자열을 실수로 바꾸어 리턴
- isFinite(value) -> value가 숫자이면 return true;
- ifNaN(value) -> value가 숫자가 아니면 retrun true;
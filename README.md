WEB
=============

[생활코딩](https://opentutorials.org/course/3084) 을 보고

HTML, CSS, JavaScript, Ajax 기초다지기!


왜? 왜 기초부터 다시?
-------------
약 1년간의 육아휴직으로 머리가 굳지는 않았을까

기억이 제대로 날까 싶어 기초부터 다시 잡기로 다짐했다


효과는?
-------------
머리속은 하얘도 손이 멋대로 움직이더라

몸이 기억하고 있다는게 신기할따름

그래도 많이 썼던 class name들은 많이 살펴봐야할거 같다

생활코딩 덕분에 [github](https://opentutorials.org/course/3084/18891) 에 접하게 되었다



배운 목차
-------------
* WEB1 - HTML & Internet
  + 프로젝트의 동기
  + 기획
  + 코딩과 HTML
  + HTML 코딩 실습 환경 준비
  + 기본 문법 - 태그
  + 혁명적인 변화
  + 통계에 기반한 학습
  + 줄바꿈
  + HTML이 중요한 이유
  + 최후의 문법 속성과 img
  + 부모 자식과 목록
  + 문서의 구조와 슈퍼스타들
  + HTML 태그의 제왕
  + 웹사이트 완성
  + 원시웹
  + 인터넷을 여는 열쇠 : 서버와 클라이언트
  + 웹호스팅 (github pages)
  + 웹서버 운영하기
    - 웹서버 운영 : 윈도우
  + 수업을 마치며 1 ~ 3
  + 부록 : 코드의 힘
    - 부록 : 코드의 힘 - 동영상 삽입
    - 부록 : 코드의 힘 - 댓글 기능 추가
    - 부록 : 코드의 힘 - 채팅 기능 추가
    - 부록 : 코드의 힘 - 방문자 분석기
* WEB2 - CSS
  + CSS 등장 이전의 상황
  + CSS의 등장
  + 혁명적 변화
  + CSS 속성을 스스로 알아내는 방법
  + CSS 선택자를 스스로 알아내는 방법
  + 박스모델
  + 그리드
  + 반응형 디자인
  + CSS 코드의 재사용
  + 수업을 마치며
* WEB2 - JavaScript
  + 수업의 목적
  + HTML과 JavaScript의 만남 1 (script 태그)
  + HTML과 JavaScript의 만남 2 (이벤트)
  + HTML과 JavaScript의 만남 3 (콘솔)
  + 데이터타입 - 문자열과 숫자
  + 변수와 대입 연산자
  + 웹브라우저 제어
  + CSS 기초
  + 제어할 태그 선택하기
  + 프로그램, 프로그래밍, 프로그래머
  + 조건문 예고
  + 비교 연산자와 boolean 데이터 타입
  + 조건문
  + 조건문의 활용
  + 리팩토링(refactoring)
  + 반복문 예고
  + 배열
  + 반복문
  + 배열과 반복문
  + 배열과 반복문의 활용
  + 함수 예고
  + 함수
  + 함수의 활용
  + 객체 예고
  + 객체
  + 객체 활용
  + 파일로 쪼개서 정리 정돈하기
  + 라이브러리와 프레임워크
  + UI & API
  + 수업을 마치며
* WEB2 - Ajax
  + 수업의 목적
  + 실습환경 준비
  + fetch API
  + Ajax의 적용
  + 초기 페이지 구현
  + 글목록 ajax로 구현하기
  + fetch API polyfill
  + 수업을 마치며

* * *

다시 짚고 넘어가기
-----------------

**JavaScript**

method : 객체 내부에 들어가는 함수

UI : User가 목적 달성을 위해 마주하는 조작 체계. User Interface

API : 프로그래머의 개발을 돕기 위해 마련된 도구 및 환경. Application Programming Interface. 프로그래머와 컴퓨터의 소통을 돕는 것. 코드 Library는 API에 소속 되었다고 할 수 있다.

DOM : Document Object Model

순서가 있게 정보를 저장하는 것이 Array이라면 순서 없이 정보를 저장하는 것이 객체 Object. 배열은 [] , 객체는 {}

    ver coworkers = {warrior : egoing}
    //               key값 : value 값 = property 속성값
    
    var Object = {
      key : value,
      key1 : value1,
      key2 : value2,
      ["ke y3"] : value3 // 띄워쓰기가 있을 경우
    }
    document.write(Object.key1);      // "." : 엑세스오퍼레이터. 객체에 접근하기 위한 것
    document.write(Object["ke y3"]);  // 띄어쓰기가 되어 있는 것은 오브젝트 오퍼레이터로 못불러오고 array와 비슷하게 불러온다

객체 내부에서 모든 데이터를 뽑아내야 할때 반복문을 이용해서 생산적으로 데이터를 꺼내자

    var coworkers = {
      "programmer" : "egoing",
      "designer" : "leezche"
    };
    for(var key in coworkers){
      document.write(key + ' : ' + coworker[key] + '<br>');
    }

* 객체 ([다른 사이트 추가 참고 함](https://www.zerocho.com/category/JavaScript/post/572c6f759a5f1c4db2481ee3))
  + 함수 Function
  + 배열 Array
  + 함수도 배열도 아닌 객체

객체 안에 객체가 속성값으로 들어갈수 있음

    var zero = {
      body : {
        width: 66,
        height: 100
      }
    }
    zero.body.height;   // 100

객체의 속성을 삭제할 수도 있음
    
    delete zero.body.height;
    zero.body;  // {width:66}

'new'라는 키워드로 객체를 생성할수 있다. 그러나 그냥 바로 {} 대괄호를 사용한 객체 생성을 권장하고 있다. 이것이 객체 리터럴(literal)

이유 : 가독성이 좋아짐, 속도가 더 빠름, 오버라이딩에 따른 예방

    var zero = new boject();
    zero.firstname = 'zero';
    zero.lastname = 'Lee';
    
    var zeroLiteral = {
      firstname : 'zero',
      lastname : 'Lee'
    }

**Ajax**

Asynchronous Javascript And Xml (비동기 자바스크립트와 XML)

    fetch('javascript')
    client -> server


* * *

추가로 [마크다운사용법](https://gist.github.com/ihoneymon/652be052a0727ad59601) 을 보며 익히기

앞으로는 마크다운에 정리해서 올리기로 했다

사실 배운 목차도 생활코딩에 연결해놔서 안써도 되는듯 했지만 마크다운에 리스트를 적용해보고자 써봤다 _히히_

# web-programming-study
web-programming-study 공부용 레포지토리 입니다.
<br>https://kimsfamily.kr/ 을 참조하였습니다.
<br>
<br>*데모 사이트 만드는 곳
<br>https://app.netlify.com/drop
<br>
<br>*예제용 홈페이지
<ol>
  <li>기본 html적용</li>https://practical-davinci-a046ec.netlify.app/
  <li>css적용</li>https://gifted-liskov-6bbece.netlify.app/
  <li>javascript적용</li>https://app.netlify.com/sites/naughty-bardeen-303e92/overview
</ol>
*정리

  ```html```
  ```
  <br> 줄바꿈
  <p> </p> 단락 바꿈, 옵션 추가 가능
  ex) style = "margin-top:45px;"
  <img src="이미지 소스파일"> : 이미지사용, width로 폭 조정 가능
  <ol> : 목록 자동화하는 부모 태그
  <li> : 목록 추가하는 자식 태그
  <meta charset="utf-8"> : UTF-8 문서포맷 설정(한글깨짐방지)
  <head> : 문서의 제목, 정보 등을 분류
  <body> : 본문의 모든 내용 기술
  <a href="주소" target="_blank" title="하이퍼링크이름"> 표시될글씨</a> //_blank는 클릭 시 새창에서 페이지가 열리게 하는 옵션
  <font color="red">내용</font> : 내용 부분의 글씨를 빨간색으로 바꿈
  ```
    
  ```css```
  ```
    <style> 바꿀 스타일 </style> : 웹브라우저가 문서를 읽을 때, css문법에 맞게 해석하도록 처리함
    선택자(selector) : 선택할 부분 ex) a: 모든 부분 선택
    속성(property) : 선택된 부분의 어떤 것을 바꾼건지 ex) color
    값(value) : 속성을 어떻게 바꿀건지 ex) red
    a{ color:red } : 해당 부분 전부 색 빨간색으로 바꿈
    <style="color:red">내용 : 내용 부분 글씨 빨간색으로 바꿈
    text-decoration:none; : 밑줄 지우기
    text-decoration:underline; : 밑줄 추가
    font-size:40px; : 폰트 사이즈 변경
    text-align:center; : 가운데 정렬
    border-width : 테두리의 두께 -> border:5px 으로 사용가능
    border-color : 테두리의 색깔 -> border-color없이 red만 사용가능(값만 사용가능)
    border-style : 테두리의 종류 //solid : 단선 -> border-style없이 solid만 사용가능(값만 사용가능)
    padding:20px : 외부와의 간격(20픽셀)
    margin:5px : 요소 사이의 간격
    display:block : (디폴트값) -> width 속성을 통해서 100px로 조정하거나 기타 수치로 조정 시 block레벨이 아닌 inline 레벨로 변경됨
    class="saw" : 링크 방문 유무 //"saw active" 처럼 띄어쓰기로 클래스 여러가지 부여 가능(잘못된 사용 방법) -> 우선순위로 처리
    올바른 사용 : class="saw" id="active" //id에 해당하는 것은 #으로 사용 ex) #active
    style 태그에 .saw { 속성:값 } : 지정한 saw 클래스의 속성에 해당하는 값 변경
    *class 우선순위
      1. ID 선택자 : #active
      2. 클래스 선택자 : .saw
      3. 태그 선택자 : a, h1 등
    <div>태그 : 디자인을 위해서 작성하는 태그 //block level elements
    display:grid : display에 grid를 사용
    grid-template-columns:150px 1fr; : 하나의 컬럼에서 배치하고, 첫 번째 컬럼은 150px로 지정해주고, 두 번째 컬럼은 나머지 공간을 다 사용한다는 뜻
    media 쿼리 : 화면에 반응하는 반응형 웹페이지 만드는 문법
    @media(min-width:800px) { div { display:none; } } : 가로 사이즈가 800px 이상이면 화면에서 div 태그를 표시하지 마라
    <link rel="stylesheet" href="style.css"> : style.css 파일을 이용해 모든 파일에 style을 일괄적용시키기 위한 문법
  ```
    
  ```javascript```
  ```
    html과의 차이 : <script> </script> 안에 작성함
    document.write('ex') : ex라고 화면에 출력함
    *html과의 차이점
      1. html은 단순히 표시된 것만 출력함(정적표현) ex) 1+1 -> 1+1로 출력
      2. javascript는 입력된 것을 연산해서 출력(동적표현) ex) 1+1 -> 2로 출력
    <input type="button" value="hi"> : hi라고 적힌 button을 생성
    (input 안에) onclick="alert('hi)" : 버튼 클릭 시 hi가 적힌 경고창을 발생시켜줌
    //onclick : 마우스가 해당버튼을 클릭했을 때 이벤트를 발생시킴(뒤에 자바스크립트 함수만 올 수 있음), alert : 경고창을 발생시켜줌
    (input 안에) onchange="alert('changed') : 해당 창 안에 변화 발생 시 'changed'라고 적힌 경고창을 발생시켜줌
    (input 안에) onkeydown="alert('keydown') : 키보드에서 문자가 입력되면 'keydown'이라고 적힌 경고창을 발생시켜줌(키 인식 이벤트)
    *데이터 타입
      1. number : 숫자데이터, 산술연산 가능
      2. string : 문자열, ''나 ""로 사용, 함수 : .length - 문자열 길이, .toUpperCase() - 문자열 대문자화, .indexOf() - 문자열에서 해당 문자 찾음
      3. 변수 : 바뀔 수 있는 어떤 값 ex) var x = 1; //var 태그는 변수를 정의할 때 사용
      4. 배열 : 같은 타입(구조)의 자료형들로 이루어진 집합 ex) var coworkers = ["park", "kim"];
      //배열함수 push(끝에항목추가), pop(끝항목제거), shift(처음항목제거), unshift(앞에항목추가), indexOf(인덱스검색), splice(위치항목제거), slice(복사), length(길이) 등
    *연산
      - 비교연산자(boolean) : ===, <, >
    *반복문
      - 일반 프로그래밍 언어의 반복문과 유사
    *함수
      - 동일한 기능을 여러번 쓰기 편하게 해줌
      - 매개변수 : 함수에 이용할 변수
      - 리턴 : 함수가 결과값을 반환함
      ex) function sum_Red(left, right) { document.write('<div style = "color:red"> + (left+right)+'</div><br>'); }
    var el = document.querySelector(".myclass") : 문서에서 myclass라는 클래스를 사용하는 첫 번째 요소를 반환함
    .style : style 속성을 포함한 css 선언을 담은 객체를 반환
    .backgroundColor="red" : 배경색을 red로 지정
    조건문 : 일반적인 언어의 조건문과 유사 //if(조건){코드}else{코드}
    *원하는 버튼의 value 값 가져오기(id이용)
      var value = document.getElementById(id).value;
    *버튼 클릭 시 이벤트 넣기 : 한 버튼을 클릭하면 상태를 받아 변화시킴
    ex) <input id="day_status" type="button" name="status" value="change night" onclick="
        if(document.querySelector('#day_status').value === 'change night'){
          document.querySelector('body').style.backgroundColor = 'black';
          document.querySelector('body').style.color = 'white';
          document.querySelector('#day_status').value = 'change day';
        } else {
          document.querySelector('body').style.backgroundColor = 'white';
          document.querySelector('body').style.color = 'black';
          document.querySelector('#day_status').value = 'change night';
        }">
    리팩토링 : 코드에 중복을 제거하고 가독성을 높이는 것
    this : this 키워드 태그로 묶여진 코드 안에 있는걸 가리키는 키워드
    객체 : 여러 속성을 하나의 변수에 저장할 수 있는 데이터 타입
    *객체 특징 (참조 : https://velog.io/@surim014)
      1. 객체는 변수이다. 그러나 객체에는 많은 값이 포함될 수 있다.
      2.(자바스크립트 변수처럼 단일 값을 포함 할 수 있다.)
      3. 객체는 중괄호 표기를 이용하여 만들 수 있다.
      4. 객체는 각각의 key/value에 대한 정보를 나열할 수 있다.
      5. Key는 문자열 또는 기호여야 한다.
      6. Value는 모든 유형이 될 수 있다.
      7. 객체는 한 쌍의 key/value 뒤에 쉼표를 이용하여 그 뒤에 오는 key/value와 구분해주어야 한다.
      8. 객체에서 명명된 값을 Properties라고 한다.
      9. 변수는 예약어의 이름을 가질 수 없지만 객체는 어떠한 이름이어도 상관없다.
      10. 객체 변수를 복사하면 참조가 복사되고 객체가 복제되지 않는다.
    객체에 변수 담기 : ex) var coworkers = { "programmer":"daniel", "designer":"kim" };
    객체 변수에 접근 : ex) coworkers.programmer; or coworkers["programmer"]; == "daniel"
    객체 추가하기 : ex) coworkers.bookkeeper = "david"; or coworkers["bookkeeper"] = "david";
    객체 불러오기(반복문) : ex) for(var key in coworkers) { coworkers[key] }
    객체에 함수 담기 : ex) coworkers.함수이름 = function() { for(var key in this) { this[key] } //coworkers.함수이름()으로 실행
    color 를 지정하는 js 파일을 따로 만들고 <script src="파일이름.js"></script> 형식으로 불러와 쓸 수 있음
    라이브러리 : 자주 사용하는 코드들을 재사용할 수 있는 형태로 가공해서 프로그래밍 효율을 높여주는 코드들
    JQuery : 엘리먼트를 선택하는 강력한 방법과 선택된 엘리먼트들을 효율적으로 제어할 수 있는 다양한 수단을 제공하는 자바스크립트 라이브러리
    구글의 자바스크립트 라이브러리 사용
    head 태그 안에 추가-> <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    *사용
      1. $('a') : 모든 a태그를 선택
      2. .css(propertyName, value) : .css로 선택한 요소의 css 속성값을 가져오거나 속성을 추가함
  ```

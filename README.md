# web-programming-study
web-programming-study 공부용 레포지토리 입니다.
<br>kimsfamily.kr을 참조하였습니다.
<br>
<br>데모 사이트 만드는 곳
<br>https://app.netlify.com/drop
<br>예제용 홈페이지
<ol>
  <li>기본 html적용</li>https://practical-davinci-a046ec.netlify.app/
  <li>css적용</li>https://gifted-liskov-6bbece.netlify.app/
</ol>
  <li><strong>html basic</strong></li>

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
    
  <li><strong>css basic</strong></li>
    
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

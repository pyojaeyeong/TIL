# HTML5 태그 



## 블록 레벨 요소 (block-level)

태그를 사용해 요소를 삽입했을 때 혼자 한 줄을 차지하는 요소로 화면의 가로폭 100%를 차지하여 다음 요소가 붙을 공간이 없어 자연스럽게 줄 넘김이 일어난다

## 인라인 레벨 요소 (inline-level)

줄을 차지하지 않는 요소로 콘텐츠만큼 영역을 차지하고 한 줄에 여러개의 인라인 레벨 요소를 표시하는 것이 가능하다



## div 태그

HTML 문서에서 구분 또는 정의

HTML 요소의 컨테이너

class 또는 id 속성을 사용하여 스타일을 지정

div를 활용한 html

```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
 		<title>div예제</title>
</head>
<body>
    <div>
        <p>안녕하세요 xe 그룹 인턴 표재영 입니다.</p>
    </div>
</body>
</html>
```



## span 태그

div 태그와 매우 유사하지만 블록 레벨 요소가 아닌 인라인 레벨 요소로 줄 바꿈이 되지 않는다.

span을 활용한 html

<!DOCTYPE html>
<html lang="ko">
 <head>
     <meta charset="UTF-8">
     <title>span 예제</title>
 </head>
 <body>
     <span>
         <a href="https://www.pxd.co.kr/" target="_blank">PXD 홈페이지 입니다.</a>
     </span>
 </body>
</html>



## li 태그

목록 항목을 정의

정렬된 목록(<ol>), 정렬되지 않은 목록(<ul>) 및 메뉴(<menu>) 내부에서 사용된다

ul 및 menu에서 목록 항목은 글머리 기호로 표시

ol 에서 목록 항목은 숫자나 문자로 표시



## button 태그

클릭할 수 있는 버튼을 정의

<button> 요소 안에는 텍스트나 이미지와 같은 콘텐츠를 삽입할 수 있지만, <input> 요소를 사용한 버튼에는 이와 같은 콘텐츠를 삽입할 수 없다

button에 type을 꼭 명시해야할 이유

button type

* submit : 버튼이 서버로 양식 데이터를 제출. 지정하지 않은 경우 기본값
* reset : 모든 컨트롤을 초깃값으로 되돌린다
* button : 기본 행동이 없어 클릭했을 때 아무것도 하지 않는다 

<button></button>    ===<button type = "submit"></button>



## input 태그

사용자로부터 입력을 받을 수 있는 입력 필드를 정의 -> 입력 필드를 선언하기 위해 <form> 태그 내부에서 사용

입력 필드는 type 속성 유형에 따라 다양하게 화면에 표시할 수 있다

input 태그를 활용한 html



<!DOCTYPE html>
<html lang="ko">
 <head>
     <meta charset="UTF-8">
     <title>input 유형</title>
 </head>
 <body>
     <div>
         <p>
             성별
             <label for="man">남자</label>
             <input type="radio" id="man" value="man" checked>
             <label for="women">여자</label>
             <input type="radio" id="women" value="women">
         </p>
     </div>
     <div>
         <p>
             음식
             <label for="chicken">치킨</label>
             <input type="checkbox" id="chicken">
             <label for="pizza">피자</label>
             <input type="checkbox" id="pizza">
         </p>
     </div>
     <div>
         <label for="colors">colors</label>
         <input type="color" id="colors" value="#e66465">
     </div>
     <br>
     <div>
         <label for="start">date</label>
         <input
             type="date"
             id="start"
             value="2018-07-22"
             min="2018-01-01"
             max="2022-12-31">
     </div>
     <br>
     <div>
         <label for="volume">Volume</label>
         <input type="range" id="volume" min="0" max="11">
     </div>
 </body>
</html>



label은 체크박스나 라디오버튼 등의 속성을 설명하는 문서를 삽입할때 사용하는 태그인데 for를 안붙이면 작은 버튼을 직접 클릭해야 하는 불편함이 있는데 for를 붙이면 label과 id가 일치하면 텍스트 부분을 클릭해도 체크박스 부분이 클릭된다



## form 태그

사용자가 입력한 데이터를 수집하기 위해 사용 

위에 있는 input, button 등의 입력 양식 태그를 포함할 수 있다

form 태그를 활용한 html

<!DOCTYPE html>
<html lang="ko">
 <head>
     <meta charset="UTF-8">
     <title>form 예제</title>
 </head>
 <body>
     <form action="" method="get">
         <label for="name">이름을 입력하세요 :
         </label>
         <input type="text" id="name" required>
         <br>
         <label for="email">이메일을 입력하세요 :
         </label>
         <input type="text" id="email" required>
         <br>
         <input type="submit" value="확인">
     </form>
 </body>
</html>
# 웹 퍼블리시 

용어

<!-- 여는 태그, 속성, 속성값, 닫는 태그 -->
엘리먼트(element) : html 문서를 구성하는 요소를 의미한다 일반적으로 시작 태그, 내용, 종료 태그로 구성

애트리뷰트(attribute) : 엘리먼트에 부여할 수 있는 속성을 의미한다 기본값으로 설정되어 있으나 애트리뷰트를 선언하여 다른 값으로 설정할 수 있다

<!-- html 요소의 css 스타일을 지정하는 역할 -->
선택자(seletor) : 엘리먼트에 CSS 스타일을 적용하기 위한 패턴

속성(property) : 엘리먼트에 부여할 CSS 스타일 속성을 의미한다 기본값이 설정되어 있으나 선언하여 다른 값을 설정할 수 있다 각 속성 단위는 세미 콜론(;)으로 구분한다

속성 값(value) : 속성에 부여하는 값으로 콜론(:) 으로 구분하여 설정



 파일/폴더 규칙

<!-- 브라우저 마다 다른 기본값으로 스타일이 적용되있다
동일한 css 스타일을 보여주기 위해 초기화 -->
reset.css : 브라우저 Style 초기화

<!-- 공통적으로 적용되는 스타일 -->
common.css : 공통(Layout, Commponent) CSS Style

style.css : Page style

library1.css : Library CSS

ui_script.js : UI Javascript

library1.js : Library JS


인코딩
CSS 첫 코드를 @charset "utf-8";
나중에 복잡한 코드를 사용할 때 기계가 이해하기 쉽도록 사용


표준 규칙

HTML 

lang 속성 : 검색 엔진이 웹 페이지를 탐색할 때 해당 웹 페이지가 어떠한 언어로 만들어져 있는지 쉽게 인식하게 만듬

viewport

<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0, user-scalable=no" />

width : 뷰포트의 너비를 설정 [device-width]

initial-scale : 뷰포트의 초기 배율을 설정 1이 기본값이며 1보다 작으면 축소 값, 1보다 크면 확대값으로 설정

minimum-scale : 뷰포트의 최소 축소 비율을 설정 기본값 0.25

maximum-scale : 뷰포트의 최대 확대 비율을 설정 기본값 5.0

user-scale : 뷰포트의 확대 또는 축소 여부를 설정 yes or no 



* initial-scale : 뷰포트의 초기 배율(곱하는 수로서 1.0, 0.75 등으로 작성)
* minimum-scale : 뷰포트의 최소 배율값(기본값은 0.25이며, 범위는 0 ~ 10.0)
* maximum-scale :뷰포트의 최대 배율값(기본값은 5.0이며, 범위는 0 ~ 10.0)
* user-scale : 사용자가 화면을 확대/축소 할 수 있는지 여부를 결정



javascript import

<script src="../ui_script.js" charset="utf-8"></script>

javascript의 경우 성능 및 브라우저 렌더링 처리 순서 등을 고려하여 body 태그 마지막에 import 할 것을 지향



앵커 : 웹 표준을 지키면서 이동하지 않는 a 태그를 만들 때는 href 속성에 #, 혹은 javascript:; 을 입력

#으로 지정해주면 다른 페이지로 연결되지 않고 클릭시 top으로 이동 되므로 없는 아이디를 부여

empty href : "#" 의 맨 위로 이동 효과 방지

[속성~=문자열] : 속성값에 문자열이 포함되어 있으면 선택(단어 기준)

[속성|=문자열] : 속성값이 문자열과 같거나 문자열-(하이픈)으로 시작하면 선택

[속성^=문자열] : 속성값이 문자열로 시작하면 선택

[속성$=문자열] : 속성값이 문자열로 끝나면 선택

[속성*=문자열] : 속성값에 문자열이 포함되면 선택



구조적 가상 클래스 선택자

nth-child(n) : 요소가 부모 요소의 자식 요소 중 n번째 순서가 맞으면 선택

nth-last-child(n) : 요소가 부모 요소의 자식 요소 중 마지막에서 n번째 순서가 맞으면 선택

nth-of-type(n) : 부모 요소의 자식 요소 중 n번째로 등장하는 요소를 선택

nth-last-of-type(n) : 부모 요소의 자식 요소 중 마지막에서 n번째로 등장하는 요소를 선택

first-of-type : 부모 요소의 자식 요소 중 첫 번째로 등장하는 요소를 선택

last-of-type : 부모 요소의 자식 요소 중 마지막으로 등장하는 요소를 선택



링크 선택자

::selection : 선택자 영역에서 사용자가 드래그한 글자를 선택



문자 선택자

::first-letter : 선택자의 첫 번째 글자 선택

::first-line : 선택자의 첫 번째 줄 선택



부정 선택자 

선택자A:not(선택자 B) : 선택자A 태그 전체 중에서 선택자B를 제외하고 선택
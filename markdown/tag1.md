# meta 태그 : 메타데이터를 정의

문자 집합(charset)을 정의하는 메타데이터 태그

<meta http-equiv="X-UA-Compatible" content="IE=edge">

: 인터넷 익스플로러(이하 IE)의 렌더링 엔진을 강제로 최신 렌더링 엔진으로 지정


<meta name="viewport" content="width=device-width, initial-scale=1.0">

:기기의 화면 너비에 맞추기 위해 사용하는 메타데이터 태그


뷰포트(viewport)는 웹 페이지에 접속했을 때 보이는 화면 영역을 의미한다

width=device-width부분은 장치의 화면 너비를 따르도록 페이지 너비를 설정한다

html 문서의 너비(width)를 기기의 너비(device-width)로 설정

initial-scale=1.0부분은 브라우저에서 페이지를 처음 로드할 때 초기 확대 / 축소 수준을 설정한다


blockquote 태그 : 출처에서 인용한 문단 단위의 텍스트를 작성할 때 사용한다

이때 출처가 확실한 인용문은 cite속성으로 출처 경로를 명시한다

fieldset 태그 : form 태그 안에 상호작용 요소를 fieldset 태그를 사용해 그룹 지을 수 있다

legend 태그 : 그룹에 이름을 붙일 수 있다

textarea 태그 : 여러 줄의 입력 요소를 생성할 때 사용한다

select 태그 : 콤보박스(combobox)를 생성할 수 있다


# 속성

size : 콤보박스에서 화면에 노출되는 항목 갯수를 지정할 수 있다

multiple : 여러 항목을 동시에 선택할 수 있다

selected : 콤보박스는 첫 번째 option 태그의 값이 기본 상태로 표시되는데 기본 선택 항목을 변경할 수 있다


option 태그 : 항목을 추가할 때 사용한다

optgroup 태그 : 항목을 그룹으로 묶을 때 사용한다


# 폼 관련 태그에서 공통으로 사용할 수 있는 속성

disabled : 상호작용 요소를 비활성화 한다

readonly : 상호작용 요소를 읽기 전용으로 변경한다

maxlength : 입력할 수 있는 글자 수를 제한한다

placeholder : 입력 요소에 어떠한 값을 입력하면 되는지 힌트를 적는 용도로 사용한다


# 시맨틱 태그

aside 태그 : 웹 페이지에서 주력 내용이나 독립적인 내용으로 보기 어려워서 article 태그나 section 태그로 영역을 구분할 수 없을 때 사용

footer 태그 : 웹 페이지에서 푸터 영역을 구분할 때 사용한다 저작권 정보, 연락처, 사이트 맵 등의 요소들을 포함한다


css 

# 가상 요소 선택자

::before : 콘텐츠 앞의 공간을 선택한다

::after : 콘텐츠 뒤의 공간을 선택한다


# 입력 요소 가상 클래스 선택자

:focus : 입력 요소에 커서가 활성화되면 선택자로 지정한다

:checked : 체크박스가 표시되어 있으면 선택자로 지정한다

:disabled : 상호작용 요소가 비활성되면(disabled 속성이 사용되면) 선택자로 지정한다

:enabled : 상호작용 요소가 활성화되면(disabled 속성이 사용되지 않은 상태면) 선택자로 지정한다

위에 :disabled 와 :enabled 속성은 자바 스크립트 change 이벤트를 사용해 활성화/비활성화를 전환할 수 있다고 한다


# 구조적 가상 클래스 선택자

:first-child : 요소의 첫 번째 자식 요소를 선택자로 지정한다

:lask-child : 요소의 마지막 자식 요소를 선택자로 지정한다



# 위치 속성으로 HTML 요소 배치

position 속성

static : 요소를 기본 흐름에 따라 배치한다

기본값으로 아무 변화가 없다 좌표 지정을 할 수 없다

relative : 요소를 기본 흐름에 따라 좌표 속성에 배치 할 수 있다

absolute  : 요소를 기본 흐름에서 벗어나 절대적인 좌표 위치에 따라 배치한다

relative는 기준점이 요소의 왼쪽 위 모서리지만 absolute일때는 웹 브라우저의 왼쪽 위 모서리이다

absolute 값일 때는 요소를 움직이면 요소가 원래 있던 공간은 빈 공간으로 인식된다

flxed : absolute와 같이 요소를 기본 흐름에서 벗어나 절대적인 좌표 위치에 따라 배치한다 단 스크롤 해도 해당 위치에 고정되있다

sticky : 스크롤하는 중에 일정 지점이 되면 요소가 fixed 값처럼 작동한다

z-index 속성 : position 속성으로 배치한 요소의 z축 위치를 결정할 수 있다

float 속성 : 요소를 공중에 띄워 다음에 오는 요소를 주변에 자연스럽게 배치할 수 있다
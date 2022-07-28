플렉스 박스 레이아웃

## 구성요소
* 주축(main axis) : 플렉스 박스의 진행 방향과 수평한 축
* 교차축(cross axis) : 주축과 수직한 축
* 플렉스 컨테이너(flex container) : display 속성값으로 flex나 inline-flex가 적용된 요소
* 플렉스 아이템(flex item) : 플렉스 컨테이너와 자식 관계를 이루는 태그 구성 요소

## 기본 속성

### display 속성

형식 - display:flex; /*inline-flex*/

### flex-direction 속성 - 주축 방향 결정

형식 - flex-direction:<속성값>;

속성값
row : 왼쪽에서 오른쪽
row-reverse : 오른쪽에서 왼쪽
column : 위에서 아래쪽
column-reverse : 아래쪽에서 위쪽

### flex-wrap 속성 - 플렉스 아이템이 플렉스 컨테이너 영역을 벗어날 때 어떻게 처리할지를 결정(기본값 nowrap)

형식 - flex-wrap:<속성값>;

속성값
nowrap : 플렉스 아이템이 플렉스 컨테이너를 벗어나도 무시한다
wrap : 플렉스 아이템이 플렉스 컨테이너를 벗어나면 줄 바꿈한다
wrap-reverse : 플렉스 아이템이 플렉스 컨테이너를 벗어나면 wrap의 역박향으로 줄 바꿈한다

### flex-flow 속성 - 단축 속성

형식 - flex-flow:<flex-direction> <flex-wrap>;

## 플렉스 박스 레이아웃 정렬 속성

### justify-content 속성 - 주축 방향으로 정렬

형식 - justify-content:<속성값>;

속성값
flex-start : 주축 방향의 시작을 기준으로 정렬
flex-end : 주축 방향의 끝을 기준으로 정렬
center : 주축 방향의 중앙에 정렬
space-between : 플렉스 아이템 사이의 간격이 균일하도록 정렬
space-around : 플렉스 아이템의 둘레(around)가 균일하도록 정렬
space-evenly : 플렉스 아이템 사이와 양끝의 간격이 균일하도록 정렬

## align-items, align-content, align-self 속성 - 플렉스 아이템을 교차축 방향으로 정렬

형식 - align-items:<속성값>;

속성값
stretch : 교차축 방향으로 플렉스 아이템의 너비나 높이가 늘어난다
flex-start : 교차축 방향의 시작을 기준으로 정렬
flex-end : 교차축 방향의 끝을 기준으로 정렬
center : 교차축 방향의 중앙을 기준으로 정렬
baseline : 플렉스 아이템의 baseline을 기준으로 정렬

* align-content - flex-wrap 속성으로 두 줄 이상이 됐을 때만 사용
* align-self - 플렉스 아이템을 각각 정렬
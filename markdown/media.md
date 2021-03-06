반응형 웹 - 미디어 쿼리

기본 문법
@media <not|only> <mediatype> and (<media feature>) <and|or|not> (<media feature>) {}

not|only
* not 뒤에 오는 모든 조건을 부정
* only 미디어 쿼리를 지원하는 기기만 미디어 쿼리를 해석하라는 의미

mediatype
미디어 쿼리가 적용될 미디어 타입을 명시.(생략 가능)
* all 모든기기
* print 인쇄 장치
* screen 컴퓨터 화면 장치 또는 스마트 기기
* speech 스크린 리더기 같은 보조 프로그램으로 웹 페이지를 소리 내어 읽어 주는 장치

사용하지 않는 미디어 유형 : CSS2.1과 Media Queries 3 모듈은 여러가지 추가 유형(tty, tv, projection, handheld, braille, embossed, aural)을 정의했으나 Media Queries 4에서 제거되어 사용해선 안된다

<!-- aural은 유사한 유형인 speech로 대체 -->
@media aural{
    .class {}
}

media feature
미디어 쿼리가 적용될 미디어 조건
min-width:<화면 너비> | 미디어 쿼리가 적용될 최소 너비
max-width:<화면 너비> | 미디어 쿼리가 적용될 최대 너비
orientation:portrait | 세로모드. 뷰포트의 세로 높이가 가로 너비보다 큰 경우
orientation:landscape | 가로 모드. 뷰포트의 가로 너비가 세로 높이보다 큰 경우

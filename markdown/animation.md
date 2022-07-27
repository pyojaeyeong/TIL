애니메이션 속성

# 키 프레임 정의
* 애니메이션이 진행되는 과정에서 특정 시점에서 발생해야 하는 여러 작업을 정의하는 문법
* 시작과 종료에 해당하는 최소 2개 시점에 대한 스타일을 정의

형식
@keyframes <키 프레임명>{
	0%{CSS 코드}
	100%{CSS 코드}
}

## animation-name 속성 - 특정 요소에서 적용할 키 프레임명을 지정

형식 - animation-name:<키 프레임명>;

## animation-duration 속성 - 애니메이션을 지속할 시간을 설정

형식 - animation-duration:<지속 시간(s)>;

## animation-delay 속성 - 애니메이션 실행을 지연

형식 - animation-delay:<지연 시간(s)>;

## animation-fill-mode 속성 - 애니메이션이 실헹되기 전과 후의 스타일을 지정

none | 실행 전 : 시작 지점(0%,from)의 스타일을 적용하지 않고 대기
     | 실행 후 : 실행되기 전의 스타일 적용

forwards | 실행 전 : 시작 지점(0%, from)의 스타일을 적용하지 않고 대기
         | 실행 후 : 키 프레임에 정의된 종료 시점(100%, to)의 스타일을 적용

backwards | 실행 전 : 키 프레임에 정의된 시작 지점(0%, from)의 스타일을 적용
          | 실행 후 : 실행되기 전의 스타일 적용

both | 실행 전 : 키 프레임에 정의된 시작 지점(0%, from)의 스타일을 적용
     | 실행 후 : 키 프레임에 정의된 종료 지점(100%, to)의 스타일을 적용


## animation-iterator-count 속성 - 애니메이션 실행 횟수 지정

형식 - animation-iterator-count:<횟수>; \\무한반복 infinite

## animation-play-state 속성 - 애니메이션의 재생 상태 지정

paused | 일시 정지
running | 실행
<!-- 순수 HTML과 CSS코드만으로는 불가능 자바스크립트를 함께 사용해야한다 -->

## animation-direction 속성 - 애니메이션 진행 방향 지정

형식 - animation-direction:<속성 값>;

normal | 키 프레임에 정의된 시간 순서대로 진행
reverse | 키 프레임에 정의된 시간 역순
alternate | 홀수 번째는 normal, 짝수 번째는 reverse로 진행
alternate | 홀수 번째는 reverse, 짝수 번째는 normal로 진행

## animation 속성 한번에 지정

형식
animation:<name> <duration> <timing-function> <delay> <iteration-count> <direction> <fill-mode> <play-state>;
전환 효과 속성

# 전환(transition)

CSS에서 한 요소에 적용된 스타일 속성값을 다른 속성값으로 변하게 하는 것

## transition-property 속성

형식 - transition-property:<속성값>;

none | 전환 효과 속성을 지정하지 않습니다
all	| 모든 속성을 전환 효과 대상으로 지정합니다

## transition-duration 속성 : 전환 효과의 지속 시간

형식 - transition-duration:<시간(s)>;

## transition-delay 속성 : 전환 효과의 발생 지연

형식 - transition-delay:<시간(s)>;

## transition-timing-function 속성 : 전환 효과의 진행 속도 지정

형식 - transition-timing-function:<속성값>;

linear | 처음 속도와 마지막 속도가 일정
ease | 처음에는 속도가 점점 빨라지다 중간부터 점점 느려짐
ease-in | 처음에는 속도가 느리지만 완료될 때까지 점점 빨라짐
ease-out | 처음에는 속도가 빠르지만 완료될 때까지 점점 느려짐
ease-in-out | 처음에는 속도가 느리지만 점점 빨라지다가 다시 점점 느려짐
cubic-bezier(p1, p2, p3, p4) | 사용자가 정의한 속도로 진행


transition 속성 한번에 지정

형식 - transition:<property>, <duraction>, <timing-function>, <delay>;
# Kokoa Coding

첫번째 메모 memo.html 파일로 옮기기 완료(너무 길어서..)
두번째 메모 시작(Pseudo Selectors part One부터)

2021/10/09
pseudo selectors: 좀 더 세부적으로 요소를 선택해주는거
이때까지 요소를 선택한 방법: 태그를 직접 선택, id를 선택, class를 선택 - 3가지

사용방법
태그: 설정함수{
속성
}
설정함수 종류
last-child: 해당 태그 중 마지막 요소
first-chile: 해당 태그 중 첫번째 요소
nth-child(n): 해당 태그 중 n번째 요소(n에 even, odd, 2n + 1, 3n + 1 등등 다 적을 수 있음)

p span{
. . .
}
이렇게 작성하면 p태그 안에 있는 span에만 적용됨
div p span도 가능

div > span{
. . .
}
이렇게 적으면 div 태그의 직접적인 자식span에만 적용
p + span{
. . .
}
이렇게 하면 p태그의 형재 span 태그에만 적용(p 바로 다음에 오는 span에만 적용됨)
p ~ span{
. . .
}
이렇게 하면 p 바로 다음에 span이 오지 않더라도 적용됨(p 바로 다음에 안오는 형제 span도 가능)

input[type="password"]{
. . .
}
이렇게 하면 input 중에 type이 password인 것만 설정 가능
input[placeholder~="name"]{
. . .
}
이렇게 하면 input 중에 placeholder의 속성값으로 name을 포함한 모든 input에 적용 가능
속성$="속성값" 이건 end로 끝나는 속성값을 가진 속성을 가진 모든 태그에 적용

상태(active(활성화 상태), hover(마우스가 위에 있을 때), focus(키보드로 선택했을 때), visited(링크를 방문했을 때), focus-within(focused인 상태인 자식을 가진 부모에 적용, 부모에 선언))

form:hover input{
. . .
}
이렇게 하면 form이 hover 상태이면 input에 적용
form:hover input:focus{
. . .
}
form이 hover 상태이고 input이 focus이면 적용

input::placeholder{
. . .
}
이렇게 하면 placeholde를 스타일링 할 수 있음
p::selection, p::first-letter, p::first-line 등등 많음


Colors and Variables
color
16진수 컬러
RGB 컬러/ rgba(a는 투명도)

:root, 변수(var(변수 이름))
변수는 --로 시작

color picker(크롬 익스텐션)
css custom properties


2021/10/16Transition
transition은 state가 없는 요소에 붙여야함
cubic-bezier: 변화하는 정도를 커스텀 할 수 있음

transform: 요소를 변형할 수 있음(회전, 늘리기, 옮기기), 같은 box 안의 다른 요소들을 변형시키지 않음

애니메이션을 만드는법: 
<style></style> 안에 생성
@keyframes (애니메이션 이름){
    from{
    ...
    }
    to{
    ...
    }
}
또는
@keyframes(애니메이션 이름){
    0%{
    ...
    }
    50%{
    ...
    }
    100%{
    ...
    }
}


2021/10/17

Media Queries: 사용자의 스크린의 크기로  css를 변형시켜줌
마찬가지로 style 태그에 적용
@media screen and (max-width: 400px):
{
    div{
    ...
    }
}
=> 스크린 너비가 400px보다 작을 때 적용
min-width, max-width로 범위 적용가능
한마디로 media의 내용이 참이면 실행


**이론 파트 완료**
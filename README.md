# Kokoa Coding

Start! 2021/09/30~

label 태그는 input과 같이 사용
label에 for이라는 attr, input에 id라는 attr을 똑같이 작성하면 됨
그러면 label 클릭 시 label의 for와 같은 id를 가진 input이 실행 됨

id는 body 안에 어떤 태그에든 넣을 수 있음
왜냐, id는 고유식별자이기 때문
태그 하나 당 id 하나만 가질 수 있음 즉, 고유해야 함
두 태그의 id의 값이 같으면 안됨
만약 같다면 실행되지 않음
css가 id를 통해 동작함

div 태그 => 박스라고 생각
div는 위아래로 배치 됨
header라는 태그는 div와 기능은 같지만 웹사이트의 헤더라는 의미가 있음
main과 footer도 마찬가지(메인 내용, 꼬리말)
header와 main, footer는 자료를 이해하는 데 도움을 줌
=>semantic
짧은 글은 span태그가 적당
span은 div랑 비슷하게 기능은 있지만 문서적인 의미는 없음

보편적인 태그 구성
<tagname attrName="value">내용</tagname>
value는 항상 큰따옴표로 열고 닫기

태그 종류들을 외우려고 하지 말기!

2021/10/03 css 시작

css가 지켜야 할 문법
속성:값; <= 이 형식을 지켜야댐
띄어쓰기, 밑줄, 슬래쉬 쓸 수 없음

브라우저는 css코드를 위에서부터 읽음
block: 세로로 배열되는 거. 옆에 아무것도 올 수 없음
inline: 가로로도 배열할 수 있는 거. 옆에 뭔가 올 수 있음ex) span, a, image


2021/10/04
span의 display 속성: 속성 값으로 inline, block을 가지고 있음.
속성값으로 inlilne 또는 block을 정할 수 있음

inline 요소는 높이와 너비가 없음. 따라서 div 요소에 내용이 없고 높이와 너비만 있다면 inline으로 바꿨을 때 보이지 않음

block의 특징 3가지 margin, padding, border
***중요 margin:은 box의 border(경계)의 바깥에 있는 공간***

margin: 20px 는 위, 아래, 왼, 오 네 방향 모두 적용
margin: 20px 15px 는 순서대로 상하, 좌우에 적용
margin: 20px 5px 12px 9px 는 순서대로 위, 오, 아래, 왼에 적용(시계방향)

div와 body의 위아래 경계가 같다면 위아래의 margin이 하나가 됨.(좌우는 해당 안댐) = collapsing margins

***padding은 box의 경계로 부터 안에 있는 공간***

태그 기반이 아닌 id 기반으로 css 적용하는 법:
# id{} <!--<= 이렇게 적으면 됨-->

***border은 box의 경계***
border: 2px solid black
border: 굵기 border-style 색
*{

} <=이 말은 모든 요소에 적용, 즉 block뿐만 아니라 inline에도 적용
모든 요소에 적용하고 하나에만 다른 style을 적용하려면 border: border-style만 적용함







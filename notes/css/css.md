## CSS
+ Cascading Style Sheet의 약자로 웹페이지의 스타일을 정의하는데 사용됨 
+ 개발자도구에서 위에있는것이 아래것을 덮어 씀
+ 이름이 같다면 나중에 쓰인 것이 우선
+ 선택자 명시도에 따라 우선순위 다름
+ 명시도는 아이디 개수, 클래스 개수, 요소 개수를 순서대로 숫자를 나열해서 점수를 매김
<br>

## SCSS
+ CSS의 확장 버전
+ 변수, 중첩, 믹스인 기능 사용하여 좀 더 효율적으로 사용 가능 

## box model이란?
+ 모든 HTML은 박스 모양으로 구성되며 이것을 box model이라 함 
+ content, border, border의 안쪽 여백인 padding, 바깥 여백 margin으로 이루어져 있음

## box-sizing: border-box
+ 크기의 값이 content, padding, border의 합이 되게 해줌
<br>

## margin과 padding
+ box model에서 border 안쪽 여백은 padding, border 바깥 여백은 margin
<br>

## 마진 상쇄
+ 인접해있는 요소들끼리의 마진은 상쇄될 수 있음
+ inline 요소를 가져 마진상쇄가 일어나지 않는 inline-block을 사용해 마진 상쇄 해결
<br>

## RGBA
+ RGB 표기에다가 불투명도(Alpha)를 추가한 것
+ 불투명도는 0 ~ 1 사이의 소수점 숫자
<br>

## background-image: linear-gradient(rgba(), rgba())
+ 앞의 색에서 뒤의 색으로 기본설정인 위에서 아래로 색이 바뀌는것으로 설정
<br>

## em과 rem
+ 1em은 부모 태그의 font-size
+ 1rem은 최상위 태그(html 태그)의 font-size   
<br>

## block
+ 가로영역을 모두 채움
+ width, height 속성 지정 가능
  
## inline
+ 줄바꿈이 되지 않음
+ width, height 지정 불가능
<br>

## inline-block
+ 줄바꿈이 되지 않지만, 크기 지정가능
<br>

## %
+ %의 기준은 면, 예를 들면 left: 50% 일때 왼쪽 면이 화면의 중간에 위치 
<br>

## float 속성
+ 부모 요소를 기준으로 기존 구조에서 벗어나 원하는 곳에 배치 가능
+ 문서의 흐름에서 벗어나지 않아 다른 요소들에 영향을 미침 
<br>

## letter-spacing, word-spacing
+ 글자 사이의 간격 조정할때는 letter-spacing: px; 로 사용
+ 단어 사이의 간격 조정 시 word-spacing 사용
<br>

## z-index
+ 숫자가 클 수록 위에 위치
+ 쌓임맥락으로 인해 부모의 z-index가 1이고 자식의 z-index가 3이어도 밑에 있는 태그의 z-index가 2라면 부모와 자식 둘 다 우선순위가 낮음 즉 부모의 z-index를 따라감
<br>

## position
+ static: 기본값, 일반적인 글의 흐름을 따름
+ relative: static의 위치를 기준으로 움직임, 원래 위치는 비어져 있음
+ absolute: 포지셔닝된 가장 가까운 조상요소를 기준으로 움직임, 원래 위치에 자리를 차지하지 않음 inset:0은 top, right, bottom, left 모두 0으로 설정
+ fixed: 스크롤해도 지정한 위치에 고정, 원래 위치의 자리를 차지하지 않음, 크기 지정해줘야 함
+ sticky: 부모 요소에 속해 원래 자리에 있다가 지정한 위치에 닿으면 fixed처럼 고정됨 
<br>

## >(자식 결합자)와 ' '(자손결합자)
+ 클래스의 이름이 겹칠 때 구분 짓기 위해 사용
+ 부모 클래스 > 자식 클래스 .parent > .son
+ 부모 클래스 ' ' 자손 클래스 ex) .parent .son
<br>

## flex-box
+ 공간 배분과 정렬기능을 제공해주는 1차원 레이아웃 모델
+ display: flex;
+ 기본값: row 즉 가로로 겹겹이 쌓임
+ flex-direction: row, row-reverse, column, column-reverse
+ justify-content: 기본축의 간격 및 위치 설정
+ align-items: 교차축의 간격 및 위치 설장
+ flex-wrap: wrap; 넘치는 요소를 다음줄에 보여줌
+ flex-grow: 1, flex-shrink: 0
<br>

## grid 
+ 2차원 레이아웃 모델 
+ grid-template-columns: 100px 300px 100px; : 각 컬럼의 너비
+ grid-template-rows: 200px 200px 100px : 각 row의 높이
+ repeat(3, minmax(200px, 300px)) 3번 200px에서 300px까지 늘어남
+ rid-auto-rows/colums : 자동으로 행이나 열의 크기 지정 
<br>

## border
+ border-collapse, border-spacing 차이

1. CSS
```
- DIV, A : 모든 Div, a 태그에 적용하겠다.
- Div a  : div 하위의 태그에 적용하겠다.
- font-family : 글꼴
- font-weight : 글꼴 형태 (normal, bold)
- 태그이름.클래스이름 : 해당 태그의 클래스에만 적용
- .클래스이름 : 해당 클래스에만 적용 (전역클래스)
- #태그아이디 : 해당 id에만 적용
```
2. 선택자
```
- 기타 선택자
  > input[type=text]
      { background:pink }
    input[type=password]
      { background:yellow }
- 문자열에 대한 속성 선택
  > [속성 ~= 값]:속성값이 특정값을 포함 
  > [속성 != 값]:속성값이 특정값을 포함하지않음
  > [속성 ^= 값]:특정값으로 시작하는 태그 선택
  > [속성 $= 값]:특정값으로 끝나는 태그 선택
  > [속성 *= 값]:특정값을 포함하는 태그선택
- 반응 선택자
  > :active : 마우스로 클릭한 태그를 선택한다.
  > :hover : 마우스를 가져다 댄 태그를 선택한다.
  > A:link{ color:green;text-decoration : none }
  > A:active{ color:yellow;text-decoration : none }
  > A:visited{ color:skyblue;text-decoration : none }
  > A:hover{ color:red;text-decoration :underline}
  ex) 
  input:hover
   { background:pink }
  input:active
   { background:yellow }
- 상태 선택자
  > checked : 체크된 곳의 input태그 선택
  > focus : 초점이 선택이 된 input태그 선택 
  > enabled : 사용가능한 input태그 선택 
  > disabled : 사용 불가능한 input태그 선택 
```
3. 글꼴
```
- 폰트 글꼴 (font-family)
  > 사용 할 글꼴(font 종류)를 지정 한다. 
  > 콤마(,)로 예비 글꼴을 지정 할 수 있고, 앞에서부터 우선 적용된다. 
  > 사용자가 확실히 갖고 있을 글꼴을 사용하는 것이 좋다. 
  > 글꼴의 종류 : 굴림, 굴림체, 궁서, 궁서체,…..등등
- 폰트 스타일 (font-style) 
  > italics : 기울임 꼴로 만들어줍니다
  > oblique : 기울임 꼴로 만들어줍니다
  > normal : 기본값이며, 평범한문자 형태입니다.
  > inherit(상속): 부모의 스타일 상속받고자 할 때 사용하는 속성값입니다.
- 폰트 굵기 (font-weight)
  > font의 굵기에 대한 정의로  두껍게 혹은 얇게 또는 수치로 지정 한다.
  > font-weight: 다음에 올 속성은 normal, bold, bolder, lighter, 길이(숫자) 등이 있다.
    * normal : 숫자 400을 넣은 것과 같음
    * bold : 숫자 700을 넣은 것과 같음
    * bolder : 숫자 900을 넣은 것과 같음(글꼴에 의존되므로 보통 700과 같게 나온다)
    * lighter : 숫자 100을 넣은 것과 같음(글꼴에 의존되므로 보통 400과 같게 나온다) 
- 폰트 크기 (font-size)
  > font 크기를 절대 크기(absolute size)로 지정한다.
    xx-small, x-small, small, medium, large, x-large, xx-large등으로 지정할 수 있다.
  > font 크기를 상대 크기(relative size)로 지정한다.
    larger, smaller 등으로 지정 한다.
  > font 크기를 길이(숫자)로 지정한다.
  > font 크기를 백분율로 지정한다.
    : 백분율 크기(percentage: %)로 지정한다.
  > 기본 값은 medium 이다.
- 폰트 복합 명령 : font
  > 간략하게 폰트의 여러 특성을  한 번에 지정 할 수 있다.
  > 지정하는 순서는 바뀌면 안되고  순서는
    font{font-style font-variant font-weight font-size/line-height font-family ;}이다.
  > 각 속성은 빈칸으로 구분 되고  값은 생략 될 수 있다.
  <예> 
    P {font : italic nomal bold 12pt/14pt 궁서,'Courier New';}
    .font9 {font: bold 12pt/14pt Helvetica,sans-serif;}
```
4. 여백, 테두리
```
- 바깥 여백지정
  > Margin은 문자가 입력되는 테두리와 테두리사이의 여백을 정의합니다.
  > margin-left, margin-right, margin-top, margin-bottom 처럼 4방향을 다르게 정의할 수도 있습니다.
- 안쪽 여백 지정
  > Padding은 글이 입력되는 테두리와 문자사이의 여백을 정의합니다.
  > Padding -left, Padding -right, Padding -top, Padding -bottom 처럼 4방향을 다르게 정의할 수도 있습니다.
- 테두리 스타일 (border-style)
  > 테두리 스타일에 대해 정의합니다.
  > 종류
    * solid : 실선
    * dotted : 점선
    * dashed : 파선 (dotted보다 약간 길다)
    * double : 복선 (두줄)
    * groove , ridge, inset, outset
  > border-radius
    상자 모서리 부분을 부드럽게 처리할 수 있는 속성이 추가되었다.
  > border-color
    테두리 색을 정의, 영문이름이나 RGB값
  > border-with
    * 테두리 두꼐를 정의
    * 한꺼번에 정의할 수도 있고 서로다르게 정의할수 도 있습니다(순서는 top right bottom left입니다)
  > border
    * 테두리에 대한 4방향 모두 각각에 대한 정의를 할 수 있습니다.
    * border-top, border-right, border-bottom, border-left에 대해 style, color, width에 대해 자세히 정의 할 수 있습니다.
  > box-shadow
    * 그래픽 프로그램을 이용하지 않고도 그림자 효과를 추가할 수 있다.
    * CSS3의 새로운 box-shadow 속성은 4개의 값을 가지며 최소 3개 이상의 값을 유지 해야한다.
    예)가로오프셋,세로오프셋,그림자번지는정도,그림자색
       box-shadow : 3px -3px 5px #ccc
```
5. 폰트
```
- EOT/WOFF/TTF/OTF
```
8. 기타
```
- contain : 채운다.
- cover : 감싼다. (반응형 웹을 할때 cover를 사용한다.)
- ol, dl, li
  > ol (ordered list)
    * 순위나 레시피 등 순서가 있는 부분을 나타냄
    * ol 요소안에는 오직 li 요소만 올수 있다.
      단, li 요소 안에는 ol요소가 중첩되어 들어갈 수 있다.
    * start, reversed 속성이 있다.
  > ul (un-ordered list)
    * 순서가 없는 목록
    * 자식 요소로는 li만 포함 할 수 있다.
    * start, reversed 와 같은 속성은 없다.
  > dl (description list)
    * 개념과 정의로 이루어진 목록
    * 개념은 dt(인라인 요소), 정의는 dd(블럭요소)
      단, dl은 dt와 dd 요소만을 자식으로 둘 수 있다.
    * dt와 dd는 1:1 뿐만 아니라, 
  > li (list)
```
9. 참고
```
- CSS Reset
  http://www.cssreset.com

- CSS3 transform-style Property
  http://www.w3schools.com/cssref/css3_pr_transform-style.asp
  https://www.zerocho.com/category/CSS/post/5864f3b59f1dc000182d3ea1
- web site 참고
  http://jcstyle.net/blog/?p=1404
  http://design-addicted.de/about/
  http://www.caseybritt.com/
  http://www.webdesignlab.net/
  http://fitzfitzpatrick.com/
  http://vefstofan.is/
  http://www.andypatrickdesign.com/
  https://www.myresponsee.com/responsive-website-templates/
  http://www.awwwards.com/
  http://www.thefwa.com/
  http://www.cssdesignawards.com/
  http://www.dbcut.com/
  http://www.gdweb.co.kr

```
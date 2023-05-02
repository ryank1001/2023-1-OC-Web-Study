# WIL5
## HTML5

html 요소는 시작태그(start tag), 종료태그(end tag), 그리고 content로 구성된다
또한 빈 요소란 content를 따로 가질 필요 없이 attribute만 가지는 요소를 말한다
대표적인 빈 요소로는 br, hr, input, link, meta가 있다


attribute는 요소의 성질, 특징을 정의하는 명세로 요소에 추가적 정보를 제공한다.
attribute는 시작태그에 위치하며 이름과 값의 한 쌍을 필요로 한다

global attribute는 모든 html에 공통적으로 사용할 수 있는 어트리뷰트로 
id: 요소에 고유한 id를 할당한다
class: 요소에 class를 할당한다
hidden: 브라우저에 노출되지 않게 숨긴다
lang: 요소의 언어를 지정한다
style: 인라인 스타일을 지정한다
tabindex: 키보드로 네비게이션시 순서를 할당한다
title: 요소에 관한 제목을 지정한다

주석을 한번 써볼거다
<!--이건 주석이다. 화면에 안 나오지롱 키키-->
써봤다.

### semantic element

브라우저, 검색엔진, 개발자 모두에게 콘텐츠의 의미를 정확하게 전달하기 위한 목적으로 사용하며,
이를 통해 컴퓨터가 html의 요소를 보다 명확하게 해석하고 활용할 수 있게 도와준다.

시멘틱 웹 (semantic web)이란 웹페이지에게 메타데이터를 부과하여 기존의 웹페이지를 거대한 데이터베이스로 구축하려는 발상이다.
non-semantic element : div: 가상의 레이아웃을 만든다, span: 기본적으로 div와 비슷하나 줄바꿈을 하지 않고 수평으로 출력한다.
semantic element : form, table, img

### 각종 태그들
title : 문서의 제목을 정하며 브라우저 탭에 표시된다
link : 외부 리소스와의 연계에 사용한다. 주로 외부 css와의 연계
meta tag : 각종 메타데이터 정의에 사용되며 주로 브라우저, 검색엔진이 이용한다.
           keywords : seo를 위한 키워드를 설정한다
           description : 문서에 대한 설명이다
           author : 문서의 저자를 명시한다
           refresh : 페이지를 정해진 주기마다 새로고침한다

b = strong : 볼드체
i = em : italic체
small : 작은 글씨
mark : 형광펜
del : 글자에 줄 찍
ins : 글자에 밑줄
sub : 아래에 조그만 글자
sup : 위에 조그만 글자
pre : 형식화된 글을 그대로 브라우저 상에 표현한다.

hr : 수평줄을 삽입한다
q, blockquote : 각각 작은 인용문, 박스 인용문을 삽입한다.


## CSS

Css : Cascading Style Sheet
### Selector
--> 스타일을 적용하고자 하는 html요소를 선택한다
> h1 {color:red;fontsize:12px;}
위와 같은 구문을 Rule Set이라 하며 이러한 Rule Set의 집합을 Style Sheet라 한다.

### Property
셀렉터로 html요소를 선택한 부분에 대해서 다양한 style을 정의할 수 있다. 사용자가 임의로 정의 불가
1. 키워드
   각 프로퍼티에 따라 사용할 수 있는 키워드가 다르다.
   ex. display - block, inline, none
2. 크기 단위
    1. px - 이미지 조정 
    2. em - 배수 설정
    3. % - 상대적 크기 설정 를 사용한다
    4. rem - em의 경우 상속의 영향을 받을 수 있기 때문에 root를 기준
    5. viewport 단위의 경우 부모의 영향을 받지 않기 위해 사용
3. 색상 표현
    1. hex코드
    2. rgb (red green blue)
    3. rgba (red green blue alpha/투명도)
    4. hsl (hue/색상 saturation/채도 lightness/명도)
    5. hsla (hue saturation lightness alpha)
4. 폰트
    1. font-size : default font size로 초깃값 설정
    2. font-family : 폰트를 지정하나 컴퓨터에 설치되어 있어야함
       --> 여러개 지정 가능
    3. font-style : 이탤릭체의 지정
    4. font-weight : 굵기 지정
    5. line-height : 띄움 정도 조정
    6. letter-spacing : 띄어쓰기 간격 조정
    7. text-align : 정렬 방식의 선택
    8. text-decoration : 말 그대로
    9. white-space : 공백의 정의
    10. text-overflow : 줄바꿈이 되지 않은 텍스트의 처리방법    정의, width의 정의, nowrap, visible 이외의 값의 정의 필요
    11. word-wrap : 딘어의 길이가 길어 부모영역을 벗어난 텍스트의 처리
    12. word-break : 위와 역할은 동일, 더 강제적
5.  위치
    1. position : 요소의 위치를 정의한다
    2. 
   
    

### Value
프로퍼티의 값으로 키워드나 크기 단위 또는 색상 표현 단위등의 특정 단위로 표현해야한다.

### html와 css의 연동
link style - 가장 일반적인 방식
embedding style - html내에 css를 포함시키는 방식이다
inline style -  html내 style 프로퍼티에 css를 기술하는 방식이다

### 박스
렌더링의 단위

콘텐트(content) - 텍스트나 이미지가 실제 위치하는 영역
패딩(padding) - 요소의 내부 여백 영역으로 프로퍼티 값은 두께, 요소에 적용된 컬러와 이미지는 패딩까지 적용된다
테두리(border) - 테두리 영역으로 프로퍼티 값은 두께를 의미한다
                border에서 프로퍼티의 값은 위 오른쪽 아래 왼쪽 순으로 작성할 수 있다
마진(margin) - 요소 외부의 여백 영역으로 프로퍼티 값은 두께를 의미한다
# WEB2_CSS
CSS

-01/14  

        CSS 소개

        태초의 웹언어인 HTML에서 디자인적 요소가 필요해서 <font>태그와 같은 디자인 담당 태그를 만들었지만 웹이 거대해지면서 난잡해지는 문제가 발생.
        그래서 웹개발자들은 HTML을 정보를 담는 그릇으로서 전념하게 하고 디자인적 요소는 따로 빼내서 하나의 새로운 언어를 만들게 되는데 그것이 CSS.
        CSS를 만들면서 생기는 장점 : HTML의 정보로서의 가치가 올라간다. / 중복의 제거



        실습환경





        HTML과 CSS가 만나는 법


         style 태그 html문법
        h2{color:blue} 가 css 문법

        <h1 style="color:red"> hello world </h1>
        여기서 color:red 가 css 문법임.





-01/16




        선택자와 선언

        CSS 기본적인 문법
        - CSS를 적용하고자 하는 태그(선택자)
        - 선택자에 적용할 디자인(선언)
        ex) <style>
        li(선택자) {color:red;}(선언)
        </style>
        *선언하는 내용 끝에 세미콜론 붙이는 것을 습관화하는게 좋다




        
        선택자의 종류

        id값이 select인 것에 효과를 준다.
        샵을 붙여준다. #select


        클래스 선택자는 . (점)


        아이디: 학생 한명 한명 식별, 한번만 등장 ...
        클래스: 1반 2반 3반 ..대상을 관리하기 쉽도록 그룹핑







-01/19




        부모 자식 선택자

        '>'를 이용해서 부모자식 선택자를 이용할 수 있다.
        태그의 id 속성지정으로 직계자손만 효과를 적용하게 할 수도 있다.


















        




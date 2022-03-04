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


        
        
        
        선택자 공부 팁

        http://flukeout.github.io/ 

        css 선택자를 게임의 형식을 통해서 익힐 수 있는 사이트 


        

        속성을 공부하는 방법

        가장 빈도수가 높은  css의 속성 순으로 공부 빈도가 낮은것을은 그런 것이 있다는 정도만 확인
        필요핼 때 검색, 질문 등 이용



        타이포그래피 



        font-size

        폰트 사이즈 단위 3가지 : px, em, rem
        - px는 절대적이고 em&rem은 상대적이다.(브라우저의 글꼴 크기를 변경할시, 전체 줌할때X)
        - 오늘날 사용자가 디자인을 변경할 권리를 부여하기 위해 rem이 권장된다.







-01/20




        color

        컬러를 표현하는 세 가지 방법
        1. color name
        2. hex(16진수 ex #FF0000)
        3. RGB(빨,초,파 ex rgb(256, 0, 0)



        



        text-align


        text-align의 4가지 속성값
        1. left : 왼쪽 정렬
        2. right : 오른쪽 정렬
        3. center : 가운데 정렬
        4. justify : 양쪽 정렬







        font


        font속성 정리
        1. font-family : 글꼴 설정(사용자 컴퓨터에 글꼴이 없는 경우 대비 여러 개를 써주는게 좋다/
        끝에 serif or sans-serif(장식 O or 장식 X)와 monospace(고정폭 or 가변폭)을 정해준다.
        2. font-weight : 굵게와 같은 것을 설정
        3. line-height : 문장 사이에 간격(px같이 절대적인 단위 사용 안하는게 좋다)
        4. font : 위에 것들과 같은 것 한 번에 쓸 수 있는 속성(대신 순서 지키는 것이 좋다)



        서채



        웹폰트 


        웹폰트 : 개발자가 선정한 폰트를 사용자가 가지고 있지 않을 때를 대비해 서버에서 해당 폰트를 다운받을 수 있게 하는 것
        - 구글 폰트를 사용하면 공짜로 웹폰트 사용 가능
        - 내가 가지고 있는 폰트를 웹폰트로 만들 때 web font generator를 사용하면 된다.


        
        조화




-01/21




        상속

        상속 : 부모 엘리먼트의 속성을 자식 엘리먼트들도 물려 받는 것
        - 일괄적으로 어떤 속성을 적용할 때 일일이 자식들에 속성을 적용하는 것보다 부모 엘리먼트 하나에 적용시키는
        것이 더 효율적이다.
        - 상속되는 속성이 있고 안 되는 속성이 있음.






-01/22  





        Stylish

        stylish : 크롬 플러그인 다른 사람들이 올려놓은 웹사이트의 새로운 디자인을 적용하거나
        내가 직접 디자인할 수 있게 도와주는 툴.


        
        
        
        
        
        캐스케이딩
        Style attribute -> id selector -> class selector -> tag selector 우선적인(구체적인) 태그 순서km
        우선순위가 낮아도 !important를 붙여주면 가장 우선적인 태그가 될 수 있음






-01/23





        레이아웃




        인라인vs 블럭레벨

        태그들 중 화면 전체를 차지하는(한 줄을 차지하는)태그는 블럭레벨 엘리먼트
        화면 일부를 차지하는(딱 자기 크기만큼 차지하는)태그는 인라인 엘리먼트라고 한다.
        각 태그마다 지정되있는 속성이 있는데 이것은 <style>태그에서 display속성을 바꿔주면 변경할 수 있다.



        







        박스 모델(box model)


        각 태그들이 웹 페이지에 표현될 때
        사각형의 형태(box)로 그 태그의 부피감을 결정한다

        박스모델 관련 속성들
        width, height, margin, padding, display, border ...

        - margin : 태그와 태그 사이의 여백.
        - padding : 태그와 내부 컨텐츠 사이의 여백
        border: width style color; 순서로 값 지정
        * inline element는 width, height 값이 무시된다.




        
        
        
        
        마진 겹침 현상


        
        마진겹침현상 세 가지
        1. 위,아래 엘리먼트들의 마진이 겹칠시 둘 중 마진이 큰게 둘 사이의 마진이 된다.
        2. 위,아래 엘리먼트들의 마진이 겹치고, 한 엘리먼트의 시각적 요소가 없어지면, 시각적 요소가 없어진 엘리먼트 마진의 top-bottom과/ left-right은 큰값으로 합쳐져 계산된다.
        3. 부모,자식 엘리먼트 사이에서 부모의 시각적 요소가 없어지면 부모,자식 마진 중 마진이 큰 쪽이 자식 마진처럼 사용된다.









-01/24




        포지션





        position 속성

        엘리먼트의 위치를 지정하는 방법 (static, relative, absolute, fixed)

        position속성 미지정시 기본값은 static
        static - 원래 있어야 되는 위치에 정적으로 위치함(offset 무시)
                위치 설정이 되지 않은 상태

        top, bottom, left, right(offset)을 적용하고 싶을 경우
        position의 값을 static외의 값으로 지정해야 한다.
        (bottom, right < top, left 적용)

        *position을 지정해도 offset값을 지정하지 않을경우
        static처럼 원래 있어야 할 위치에 있게된다

        relative - 원래의 위치에서 상대적으로 위치를 변경

        absolute - html element를 기준으로 절대적인 위치로 변경

        **부모-자식 관계에 놓인 태그의 경우
        1) 자식태그가 absolute인 경우 부모태그는 자신의 크기만 가진다.
        이 때 자식태그는 block태그여도 inline태그처럼 컨텐츠만한 크기로 변한다.
        width와 height 값을 지정하면 크기 변경이 가능하다.
        (★fixed도 같은 효과)

        2) 여러 부모태그 중 absolute인 자식태그는
        position이 relative인 부모태그안에서 절대적으로 위치를 변경한다.

        fixed - 화면의 위치에 고정시켜 스크롤으로부터 독립되게 한다.







        float



        Float는 편집 디자인에서 이미지를 삽화로 삽입할 때 사용하는 기법입니다. 또한 레이아웃을 잡을 때도 사용하는 기능이다.




-01/25





        box-sizing


        width값은 border 안의 element의 크기를 지정한다.
        box-sizing: border-box; 명령을 내리면
        width값은 border 테두리까지의 크기를 의미하게 된다.



        그래픽 




        배경(backgraound)

        background : 엘리먼트의 배경에 이미지나 색깔 등을 지정할 수 있는 속성

        background-color : 색깔 지정 

        background-image : 이미지 지정(배경이 투명한 이미지를 쓰면 color와 같이 쓸수있음)

        background-repeat : 반복에 관한 설정

        background -attachment : 스크롤 내릴 때 배경도 같이 내릴지 안내릴지

        background-size : 크기에 관한 설정(cover, contain : 손실있어도 꽉차게, 꽉안차도 손실없게)

        background-position : 위치 결정

        축약형:background:tomato url('run.png') no-repeat fixed center;





        Filter(필터)

        filter : 기존에 포토샵 등을 통해서 이미지나 텍스트에 필터효과를 줬던 것을 코드화한 기능







-01/26





        혼합(blend)


        blend : 이미지와 이미지를 혼합하는 기능
        - background-blend-mode : 배경과 배경(이미지, 색깔 등)을 혼합
        * rgba(a는 투명도 0~1 지정), hover등과 조합 가능
        - mix-blend-mode : 컨텐트와 배경을 혼합




        
        
        
        변형(transform)

        transform : 엘리먼트 크기, 비틀기, 회전 등 포토샵에서 가능했던 작업들을 코드화한 기능
        - 2차원, 3차원이 있다
        - 여러 속성을 쓰고 싶으면 한 줄에 이어서 쓴다
        - transform-origin : 중심축을 중앙이 아닌 곳으로 변경하고 transform한다
        * 여러가지 transform library를 활용해보는 것도 좋다.







-01/27  





        SGV

        .svg : 벡터 이미지를 저장하는 포멧
        - vector vs bitmap : 확대했을때 깨지지 않음 vs 깨짐(.svg , .png)



       

       전환(transition)


       transition : 장면 전환은 부드럽게 할 수 있는 기능
        -property : 어떤 속성에 transiton을 적용할 것인지(all or 특정 속성(transform, font-size 등)
        -duration : 몇 초에 걸쳐 전환할 것인지
        transition : 위의 두 개의 속성의 축약형(transform 1s, font-size 2s 이렇게 두 개 나눠서 적용도 가능)
        -delay : 처음에 시간차를 두고 전환
        -timing-function : 장면전환속도를 균일하지 않게(ceaser 사이트 참고)








-01/28 




        유지보수




        link와 import


        link, import : 중복의 제거를 위해 css파일을 외부로 빼는 기능
        - 중복이 일어나면 : 유지보수가 어렵고 / 코드이해도가 낮아지고 / 사용자와 개발자의 비용이 증가하는등의문제
        - 방법 : <link> 태그 혹은 <style> 태그 안에 @import로 css파일 삽입







        코드 경량화(minify)

        
        minify : 웹사이트의 규모가 커졌을 때 코드를 경량화하기 위한 기술
        -cleancss같은 사이트 이용
        -보통 경량화한 파일에는 ~~~.min.확장자 같이 .min이 들어감










-02/04




        CSS 뛰어넘기(preprocessor)

        preprocesser : 표준화된 css문법은 아니지만 더 편리하게 개인이 커스터마이징한 기능들을 쓸 수 있고 그것을 css표준문법으로 변환해주는 기술




        fontello

        fontello : 아이콘을 폰트의 형태로 바꿔서 사용할 수 있게 하는 기술
        - 사용법 : <i class="해당 폰트 이름"></i>







-03/03



        
        W3school로 공부하기.


































        



















        



















        





















        




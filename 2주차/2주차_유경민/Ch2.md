[# 뷰의 속성](#1.-뷰의속성)

[# 뷰 레이아웃 종류](#2.-레이아웃-종류)

## 1. 뷰의속성
# 텍스트 뷰
* autoLink 속성     </br>
  오토링크는 텍스트 뷰를 링크화 한것이다. 속성값으로는 web,email,phone등이 있다.
  linksClickable 속성은 기본값이 true이지만, false로 바꾸면 링크 형식의 문자열을 가지나 해당 링크를 타고 어딘가로 넘어가진 않는다.(힝 속았지?)
       
  <img width="423" alt="스크린샷 2023-09-15 오후 9 25 34" src="https://github.com/youkm1/Kotlin_ANS.Study/assets/77780624/86d80be8-c34d-4aa6-8fcb-70f351da06b9">
     
  그렇다면 다음과 같이 나타난다. 
     
  <img width="213" alt="스크린샷 2023-09-15 오후 9 30 10" src="https://github.com/youkm1/Kotlin_ANS.Study/assets/77780624/673ef868-6189-41f9-bc31-0d58c049a9e8">

  줄이 너무 길어서 보기 이상하다. 그렇다면..
  

  <뷰 클래스 복습. 레이아웃 중첩을 사용해보았다.>
  
  <img width="1270" alt="스크린샷 2023-09-16 오전 12 35 53" src="https://github.com/youkm1/Kotlin_ANS.Study/assets/77780624/7713b914-a64a-494c-9431-8291e97fcdfa">

* autoText 속성 </br>
  자동수정 기능이다.
  
* ellipsize 속성
  말이 길어지면 줄임표(...)을 대신 넣어준다.



# 컴파운드 버튼
* 버튼/체크박스/라디오
  버튼은 사용자 이벤트를 처리, 체크박스는 다중 선택, 라디오버튼은 단일 선택을 제공한다.

  ## 라디오 버튼
    안드로이드 문서에 따르면, 사용자에게 여러 옵션을 보여주며 한 가지를 선택하도록 하는 기능이다.
    이때, 여러 옵션은 상호 배타적인 관계로(RadioGroup 내부에서 함께 그룹화하는 방식) 그려내어야 하며,
    만약 다중 선택을 일일히 다 보여줄 필요가 없다면 드롭다운 형식으로 표현하기 위하여 Spinner 객체를 활용한다.</br>
    
    <img width="1112" alt="스크린샷 2023-09-16 오후 8 08 41" src="https://github.com/youkm1/Kotlin_ANS.Study/assets/77780624/25750263-b0cf-4cf7-a4f2-a8c9edcffb95">

# 에디트 텍스트
## 사용자가 글을 입력하는 뷰이다.
* lines, maxLines 속성
  전자는 입력할 수 있는 맥시멈을 제한할 수 있고 후자는 보이는 문장을 제한하는 것이다. (후자는   더 입력할 수 있음)
* inputType 속성
  입력 속성을 정한다. 속성값은 다음과 같다.
  </br>
  ![image](https://github.com/youkm1/Kotlin_ANS.Study/assets/77780624/2f40f6f9-520b-4f17-a5a4-8c9b555936a2)

# view binding    
## 레이아웃 XML에 선언한 뷰 객체를 코드에서 쉽게 이용하는 방법이다.    

</tr>
자바에서도 findViewByUd() 함수를 써서 객체를 불러왔을 것이다. 
뷰 바인딩은 각 객체의 id를 주어서 메인액티비티에 불러오는 것을 뜻한다. 
xml에서 버튼 객체의 id를 부여하고, A 버튼을 누르면 good이 출력되게 하였다.
  

<img width="1152" alt="스크린샷 2023-09-16 오후 8 23 39" src="https://github.com/youkm1/Kotlin_ANS.Study/assets/77780624/76746f6c-8841-49fc-b282-826b41a6ab04">


<img width="189" alt="스크린샷 2023-09-16 오후 8 24 17" src="https://github.com/youkm1/Kotlin_ANS.Study/assets/77780624/1e500990-cc74-4e1c-83f6-e3b7f3d58bb4">

*Good..*

## 2. 레이아웃 종류 
* 1. LinearLayout  2. RelativeLayout 3. FrameLayout 4. GridLayout 5. ConstraintLayout

### LinearLayout
  뷰를 가로,세로 방향으로 나열하는 레이아웃 클래스. 
  </br>
### RelativeLayout
  상대 뷰에 따라 유동적으로 정렬하는 레이아웃 클래스. 화면에 출력된 특정 뷰를 기준으로 함.
  </br>
### FrameLayout
  뷰 객체를 카드 쌓듯 겹치고 겹처서 계속 출력하는 레이아웃 클래스.
  쓸 일이 없어보이지만 하단 탭 버튼 등을 구현할 때 사용한다. (이제 모바일은 하단 탭 버튼 등   이 없어지는 추세 같은데 계속 사용할까?)
  </br>
### GridLayout
  LinearLayout과 비슷하지만 줄바꿈을 자동으로 해주는! 레이아웃 클래스. 
  </br>
### ConstraintLayout
  레이아웃 편집기에서 제일 잘 활용할 수 있는 레이아웃 클래스.
  객체마다 제약을 둔다. 


# 컴포넌트 기반인 안드로이드 앱
## 액티비티, 서비스, 브로드캐스트 리시버, 콘텐츠 프로바이더 etc.

액티비티는 화면. 필요치 않은 앱이라면 액티비티는 없어도 된다.
만약 화면이 10개라면, 액티비티 10개 대신 액티비티 1개에 </U>fragment 이용하면 된다.


### 화면 구성하는 방법
1. 액티비티 코드
   다음은 MainActivity.kt에서 화면 구성하는 코드 예시이다.
   <img width="884" alt="스크린샷 2023-09-14 오후 5 53 02" src="https://github.com/youkm1/Kotlin_ANS.Study/assets/77780624/5884a20a-7426-4c16-aef2-c9b5961665cf">
    XML 따위 간단히 지워버려도 된다. 
    Empty Activity 말고 No Activity 선택할 때 좋을 것 같다.
    </br>
3. 레이아웃 XML
   다음은 activity_main.xml에서 화면 구성하는 코드 예시이다.
   <img width="667" alt="스크린샷 2023-09-14 오후 8 17 52" src="https://github.com/youkm1/Kotlin_ANS.Study/assets/77780624/d30696d9-1283-47d4-b3d7-c17562cbd176">


**뷰 클래스**

----
<img width="624" alt="스크린샷 2023-09-14 오후 8 36 33" src="https://github.com/youkm1/Kotlin_ANS.Study/assets/77780624/96441fdc-96a2-437c-a456-85f8670d8122">


레이아웃 속 레이아웃이다. 

참고로 객체 하나에 id를 부여하면 main.kt에서 findViewById()함수로 뷰 객체를 가져올 수 있다.
```kotlin
setContentView(R.layout.activity_main)
val txtView1  =  findViewById<TextView>(R.id.txt1)
```

> 뷰의 간격 설정
> > 뷰의 간격은 margin 과 padding 속성으로 설정한다.

> 뷰의 표시 여부 설정
> > visibility/invisible/gone이 있다.
> > > invisible은 화면에 보이지 않지만 차리를 차지하며 gone은 자리조차 ❌
 

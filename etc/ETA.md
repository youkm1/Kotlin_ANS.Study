# 안드로이드 어플의 4가지 컴포넌트가 있다.
## 액티비티(Activity), 서비스(Service), 브로드 캐스터(BroadCast Receiver), 콘텐츠 제공자(Content Provider). 

서비스에서는 foreground/background/bind가 있다.  </br>
foreground는 사용자가 보이는(카메라,달리기,심박수 등등은 permission이 필요할 것), 반대로 background는 사용자가 보이지 않아도 이용되는 서비스이다. </br>
서비스를 호출할 때는 startActivity()로 호출한다. 다음과 같은 함수는 또한, 타 화면으로 전환하는데도 쓰인다. </tr>[startActivity()|startActivityForeResult() 참조]

<tr></tr>
<br>
<br>
🍿
Dialog와 Toast, Sncakbar의 차이와 각각의 용도를 정리한 것을 보았다. 아주 유용한 것 같다. 
<img width="702" alt="스크린샷 2023-10-22 오전 1 46 56" src="https://github.com/youkm1/Kotlin_ANS.Study/assets/77780624/a57747e7-be15-4300-9bce-6c4c93a35158">

출처: https://brunch.co.kr/@oemilk/91


# ANR오류 해결을 위한 코루틴
ANR오류를 들어보셨습니까?
이것은 어플이 멈춰서 두들기고 두들기면 결국 마주하는 슬픈 오류입디다.
</br>
<img width="228" alt="스크린샷 2023-10-29 오전 12 08 00" src="https://github.com/youkm1/Kotlin_ANS.Study/assets/77780624/16eed3f7-84f1-4db0-a844-61f7abb636f4">
</br>
ANR은 긴 런타임으로 인해 일어난다. 이것을 해결하기 위해 동시에 처리 가능한 수행이 필요하고 그 수행 기능은 쓰레드에서 코루틴으로 발전한다.

## 쓰레드 ➡️ 코루틴 
</br>
코루틴을 사용하려면 scope가 필요하다
종류에는,
</br>
- GlobalScope
- ActorScope
- ProducerScope
</br>

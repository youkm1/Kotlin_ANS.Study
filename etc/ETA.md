안드로이드 어플의 4가지 컴포넌트가 있다.
액티비티(Activity), 서비스(Service), 브로드 캐스터(BroadCast Receiver), 콘텐츠 제공자(Content Provider). 

서비스에서는 foreground/background/bind가 있다.
foreground는 사용자가 보이는(카메라,달리기,심박수 등등은 permission이 필요할 것), 반대로 background는 사용자가 보이지 않아도 이용되는 서비스이다.
서비스를 호출할 때는 startActivity()로 호출한다. 다음과 같은 함수는 또한, 타 화면으로 전환하는데도 쓰인다. [startActivity()|startActivityForeResult() 참조]

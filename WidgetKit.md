![img](https://blog.kakaocdn.net/dn/bHTsBO/btqF2RJHD2z/2OmkRbdDs9qUH2uJmYSQwk/img.png)



이게 위젯

위젯은 일반적인 프로젝트가 아니하 타겟으로 되어있슴



![img](https://blog.kakaocdn.net/dn/bnKX2h/btqF3aCjqMx/GNFT7H4wO6ITCkJQpX1Xh0/img.png)

그럼 이런게 만들어짐



야기 코드를 보면요...

![img](https://blog.kakaocdn.net/dn/4CQqR/btqF4TzEMeV/UNBXi3QUjv1D3Fw4hB2cf1/img.png)

이딴 무서운게 나옵니다. 

뭔가 무서운 스위프뜨 유아이 코드가 막 나옵니다. 

천천히 알아보면요..

.![img](https://blog.kakaocdn.net/dn/rTqHB/btqF2SPtHFI/Do440iDE5LAE31Xq2mREyk/img.png)![img](https://blog.kakaocdn.net/dn/bHWuXq/btqF3TNGcSE/qLMN7X0gIneA7OM5zVbaX1/img.png)

![img](https://blog.kakaocdn.net/dn/D2W8b/btqF2SBYq6H/O3VwA8GXMXY8ioWxklVov0/img.png)

이렇게 세게의 주요 코드가 있습니다. 

**1. Configuration. 위젯을 식별하며, 위젯의 Content를 표시하면 SwiftUI View를 정의.**

**2. Timeline provider. 시간이 지남에 따라 위젯 View를 업데이트하는 프로세스를 주도.** 

**3. SwiftUI View. WidgetKit에서 위젯을 표시하는데 사용하는 View.**



## **WidgetConfiguration**

![img](https://blog.kakaocdn.net/dn/ux2Oq/btqGfswX0fE/8YymHaRxqqC7cIobZz7I90/img.png)

일단 Widget에서 사용 할 수 있는 Configuration은 2가지가 있슴다.

**[StaticConfiguration](https://developer.apple.com/documentation/widgetkit/staticconfiguration)**

**[IntentConfiguration](https://developer.apple.com/documentation/widgetkit/intentconfiguration)**

StaticConfiguration은 사용자가 구성 할 수 있는 프로퍼티(ser-configurable properties)가 없는 위젯입니다

IntentConfiguration은 사용자가 구성 할 수 있는 프로퍼티(user-configurable properties)가 있는 위젯입니다



**provider** : 위젯을 새로고침할 타임라인을 결정하는 객체

![img](https://blog.kakaocdn.net/dn/bFSY4u/btqH8dirLTC/Xw2ZIvbwZjdCuM6wlD8XU1/img.png)

이거가 시간 설정하는 코드임.. 암튼 그럼

**content** : 이 closure에는 WidgetKit이 Widget을 렌더링하는데 필요한 SwiftUI View가 포함되있슴

![img](https://blog.kakaocdn.net/dn/cOIktK/btqGh42Zery/7tyrZoreY6C5IrKNTevtm1/img.png)

우리가 익히 알던 스위쁘트유아이임 모르는 사람은 꼭 배워보새요 ^^ 



아 글고

![img](https://blog.kakaocdn.net/dn/dht9ZJ/btqGiJRzmHx/l1607mHSNPFc6zBifNlKok/img.png)

요거 Configuration 밑에 삽입합니다.

![img](https://blog.kakaocdn.net/dn/pN9fF/btqGdRKjZ3M/NRjdqcT5VzVaiancSFtJf1/img.png)

그러면 저 타이틀과 서브타이틀이 설정되게 됩니다. 

더 배워보고 싶다면 배워봐도 좋아요... 하지만 전 포기했습니다. 일단 외국 문서도 별로 없고(한국 문서는 그럼 거의 없겠죠??) 암튼 여차저차 이유로 제대로 못해봤습니다. 이상

# Let's deep dive into Xcode 🦦

## Intro
**1. Xcode를 학습하여 앱의 품질과 생산성을 개선할 수 있는 다양한 방법들을 연구합니다.**

**2. Xcode 내 코딩 외적인 부분에서의 생산성을 저하시키는 문제들을 방지하고자 합니다.**

훌륭한 요리(Product)를 만들기 위해 레시피를 연구하는 것도 좋지만 좋은 조리도구를 잘 활용하면 도움이 되는 것처럼, 훌륭한 앱을 만들기 위해서 Xcode를 잘 사용할 줄 알면 좋으니까요. 그리고 도구를 잘못 사용하여 벌어질 수 있는 문제들을 사전에 예방할 수 있구요.

**중단기적인 목표**로 앱 개발, 배포 과정에서 Xcode를 통해 이루어지는 코딩 외적인 부분들을 이해하는 것입니다.
지금 생각나는 것들로는... Xcode의 빌드 시스템, Build Scheme, instrument 사용, Derived Data 분석, Static과 Dynamic Library, Linker, Framework embed와 not embed, Nested Framework, XCFramework, bitcode, arm64와 x86_64 아키텍처 간 빌드 차이 등등이 있겠습니다. 안써있는게 아직 엄청 많죠...? 일단 패스.

**장기적인 목표**로는 Xcode의 업데이트 버전들의 release note를 꾸준히 추적하고 이해하는 것입니다.

~~중단기 목표 달성을 위한 스터디를 **5월 중**으로 모집할 예정입니다. 혹시 이 글을 읽고 관심이 있으신 분들은 미리 제게 연락을 남겨주시면 감사하겠습니다. 코딩 외적인 부분이기도 하고 제 기준엔 내용이 어렵고 양도 많아서 꽤나 지루하고 오~래 걸릴 것으로 예상됩니다. 감안하시고, 천천히 오래 함께 하실 분 연락 주세요. 일단 제가 너무 빡세게 하긴 싫어요ㅜㅜ~~  
**이직+여행 때문에 8월에 시작하는 것으로 연기합니다.. 😅** 


> 이 내용들이 흥미롭다면 or 학습의 필요성을 느낀다면 🤗   
> 일단 저는 하나도 안봤고 흥미, 필요성만 느낀 상태입니닷 ㅎㅎ;  
> [Building Faster in Xcode - WWDC18](https://developer.apple.com/videos/play/wwdc2018/408/)  
> [Behind the Scenes of the Xcode Build Process - WWDC18](https://developer.apple.com/videos/play/wwdc2018/415/)  
> [Binary Frameworks in Swift - WWDC19](https://developer.apple.com/videos/play/wwdc2019/416/)  
> [Getting Started with Instruments - WWDC19](https://developer.apple.com/videos/play/wwdc2019/411/)  
> [Binary Framework(XCFramework)를 Swift Package로 배포하기 - 민소네님 블로그](http://minsone.github.io/programming/distributing-binary-frameworks-as-swift-packages-2)  
> [SwiftPM로 RxSwift 사용할 때 RxBlocking, RxTest를 유닛테스트에서 사용하기 - 민소네님 블로그](http://minsone.github.io/ios/mac/ios-swiftpm-rxblocking-rxtest-on-unit-test)  
